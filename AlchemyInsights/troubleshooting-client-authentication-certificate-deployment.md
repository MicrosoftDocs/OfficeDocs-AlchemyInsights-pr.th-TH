---
title: การแก้ไขปัญหาการปรับใช้ใบรับรองการรับรองความถูกต้องของไคลเอ็นต์
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: 698329d7705af320c9f679b92532b58ac84e6624
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555807"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>การแก้ไขปัญหาการปรับใช้ใบรับรองการรับรองความถูกต้องของไคลเอ็นต์

โปรไฟล์ใบรับรองลูกค้า Intunes NDES/ SCEP และ PKCS/PFX มักใช้ร่วมกับโปรไฟล์ประเภทอื่น ๆ เช่น Wifi, VPN และอีเมลเพื่อให้ผู้ใช้สามารถตรวจสอบสิทธิ์ไปยังทรัพยากรขององค์กรได้ เมื่อชนิดโพรไฟล์เหล่านั้นถูกเชื่อมโยงกับส่วนกําหนดค่าใบรับรองไคลเอ็นต์จะขึ้นอยู่กับการปรับใช้ส่วนกําหนดค่าที่ประสบความสําเร็จ

การตั้งค่าโครงสร้างพื้นฐานเริ่มต้นและการกําหนดค่าที่เกี่ยวข้องของส่วนกําหนดค่าใบรับรองไคลเอ็นต์มักต้องการการแก้ไขปัญหา สําหรับคําแนะนําทีละขั้นตอนการตั้งค่าตัวเชื่อมต่อ NDES ที่สําเร็จ และคําแนะนําในการแก้ไขปัญหาเพื่อแยกปัญหาเกี่ยวกับการปรับใช้ใบรับรอง ให้ดูที่: 

- [กําหนดค่าโครงสร้างพื้นฐานเพื่อสนับสนุน SCEP ด้วย Intun](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [ภาพรวมสําหรับการแก้ไขปัญหาโพรไฟล์ใบรับรอง SCEP กับ Microsoft Intun](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

ใช้สคริปต์ PowerShell อ้างอิงเพื่อช่วยในการตรวจสอบการกําหนดค่าของคุณ สําหรับข้อมูลเพิ่มเติม ให้ดูที่[สคริปต์การตรวจสอบตัวเชื่อมต่อ Intunณี Certificate](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority)

  
**ปัญหาทั่วไปอื่นๆ**

**เมื่อฉันพยายามที่จะติดตั้งตัวเชื่อมต่อใบรับรอง Intund บนเซิร์ฟเวอร์ตัวเชื่อมต่อ NDES ฉันได้รับข้อความ "รหัสผ่านในการร้องขอใบรับรองไม่สามารถตรวจสอบ มันอาจจะถูกใช้แล้ว ขอรับรหัสผ่านใหม่เพื่อส่งคําขอนี้"**  

ข้อความนี้หมายความว่า คุณจําเป็นต้องเรียกใช้การติดตั้งตัวเชื่อมต่อใบรับรองในฐานะผู้ดูแลระบบ

ในบางสภาพแวดล้อม เซิร์ฟเวอร์ที่ Intuny Certificate รันต้องใช้พร็อกซีเซิร์ฟเวอร์เพื่อเชื่อมต่อกับ Intun ณี และดังนั้นตัวเชื่อมต่อใบรับรองต้องใช้พร็อกซี ในบางสถานการณ์ ตัวเชื่อมต่อ NDES ละเว้นการตั้งค่าพร็อกซีที่กําหนดค่า ไว้ และอาจจําเป็นต้องกําหนดค่าการตั้งค่าพร็อกซีขณะทํางานในบริบทความปลอดภัยของ LocalSystem 
 
โซลูชันคือการเรียกใช้ Internet Explorer เป็นระบบ และกําหนดค่าพร็อกซีใน IE หลังจากเริ่มการทํางานของบริการตัวเชื่อมต่อ Intun

**อุปกรณ์ของผู้ใช้จะไม่ได้รับใบรับรอง SCEP จาก NDES อีกต่อไป**

เป็นไปได้ว่า ใบรับรองการรับรองความถูกต้องของไคลเอ็นต์ที่ออกไปยังเซิร์ฟเวอร์ NDES และระบุในระหว่างการติดตั้งตัวเชื่อมต่อ NDES หมดอายุหรือหายไป เมื่อต้องการแก้ไข: 
 
1. ถอนการติดตั้งตัวเชื่อมต่อ NDES  
2. ใช้รายละเอียดเหล่านี้เพื่อร้องขอการรับรองความถูกต้องของไคลเอ็นต์ใหม่หรือใบรับรองการรับรองความถูกต้องของเซิร์ฟเวอร์: 
 
    - ชื่อเรื่อง: CN =fqdn ภายนอก  
    - ชื่ออื่นของชื่อเรื่อง (ทั้งสองต้อง): DNS = fqdn ภายนอก DNS = fqdn ภายใน 
 
3. ติดตั้งตัวเชื่อมต่อ NDES ด้วยใบรับรองใหม่
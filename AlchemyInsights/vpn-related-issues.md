---
title: ปัญหาที่เกี่ยวข้องกับ VPN
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1545"
- "9000076"
ms.openlocfilehash: 3c031725c92f5d7af7c0dd0c37ea34fecf4792c8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47726110"
---
# <a name="vpn-related-issues"></a>ปัญหาที่เกี่ยวข้องกับ VPN

การดำเนินการที่ประสบความสำเร็จของการเชื่อมต่อ VPN สำหรับไคลเอ็นต์ MDM ขึ้นอยู่กับโปรไฟล์ที่ปรับใช้ซึ่งแสดงความต้องการของโครงสร้างพื้นฐานของ VPN อย่างถูกต้อง สำหรับการตั้งค่าที่เหมาะสมสำหรับแพลตฟอร์มไคลเอ็นต์ที่คุณกำลังตรวจสอบให้ดูที่: 

[การตั้งค่าอุปกรณ์ windows 10 และ Windows ที่ใช้งานโฮโลแกรมเพื่อเพิ่มการเชื่อมต่อ VPN โดยใช้ Intune](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[เพิ่มการตั้งค่า VPN บนอุปกรณ์ iOS และ iPadOS ใน Microsoft Intune](https://docs.microsoft.com/intune/vpn-settings-ios)  
[การตั้งค่าอุปกรณ์ Android เพื่อกำหนดค่า VPN ใน Intune](https://docs.microsoft.com/intune/vpn-settings-android)  
[เพิ่มการตั้งค่า VPN บนอุปกรณ์ macOS ใน Microsoft Intune](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

ถ้าโปรไฟล์ VPN ของคุณใช้การรับรองความถูกต้องโดยใช้ใบรับรองตรวจสอบให้แน่ใจว่าโปรไฟล์ใบรับรองหลักและใบรับรองการรับรองความถูกต้องของไคลเอ็นต์ที่ลิงก์ไปยังโปรไฟล์ VPN ถูกปรับใช้เสร็จเรียบร้อยแล้ว

**ปัญหาทั่วไป**

**ฉันจัดวางโปรไฟล์ VPN ไปยังอุปกรณ์ Intune จะแสดงว่าเสร็จเรียบร้อยแล้วแต่อุปกรณ์ไม่ได้เชื่อมต่อกับ VPN**

สถานะที่เสร็จสมบูรณ์หมายความว่า Intune ได้ปรับใช้โปรไฟล์ตามที่ได้รับการกำหนดค่าเรียบร้อยแล้ว อย่างไรก็ตามการกำหนดค่าเหล่านี้อาจไม่ตรงกับความต้องการของเครือข่ายและ/หรือการรับรองความถูกต้องของคุณ ตรวจทานบันทึกในบริการโครงสร้างพื้นฐานและการรับรองความถูกต้อง (บนเซิร์ฟเวอร์ VPN และเซิร์ฟเวอร์ NPS/Radius) สำหรับรายละเอียดเพิ่มเติมเกี่ยวกับการเชื่อมต่อที่พยายาม คุณอาจจำเป็นต้องทำงานกับทีมโครงสร้างพื้นฐานของเครือข่ายของคุณหรือผู้จำหน่าย VPN ของบริษัทอื่นเพื่อรวบรวมและตรวจทานบันทึก

**เมื่อฉันกำหนดค่า VPN แบบกำหนดเองสำหรับ iOS ฟีเจอร์ VPN สำหรับแต่ละแอปจะไม่พร้อมใช้งาน**

สำหรับอุปกรณ์ iOS สำหรับอุปกรณ์ iOS ใน Intune จะพร้อมใช้งานสำหรับรายการของผู้ให้บริการและคู่ค้าที่เฉพาะเจาะจงซึ่งจะต้องตรงตามข้อกำหนดเบื้องต้นของใบรับรองก่อนที่จะกำหนดค่า VPN สำหรับแต่ละแอป สำหรับข้อมูลเพิ่มเติมให้ดูที่[ตั้งค่าเครือข่ายส่วนตัวเสมือนสำหรับแอป (VPN) สำหรับอุปกรณ์ iOS/iPadOS ใน Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app) 

สำหรับข้อมูลเพิ่มเติมเกี่ยวกับชนิดการเชื่อมต่อ VPN ทั้งหมดใน Intune ให้ดู[ที่สร้างโปรไฟล์ vpn เพื่อเชื่อมต่อกับเซิร์ฟเวอร์ vpn ใน Intune](https://docs.microsoft.com/intune/vpn-settings-configure)  

**VPN ตามความต้องการของ iOS จะไม่ถูกเรียกเมื่อมีการเข้าถึงโดเมนที่กำหนดค่าไว้**

เมื่อต้องการทดสอบการตั้งค่า VPN อัตโนมัติให้ตั้งค่าต่อไปนี้:

ฉันต้องการดำเนินการดังต่อไปนี้: **ประเมินความพยายามในการเชื่อมต่อแต่ละรายการ** 

เลือกว่าจะเชื่อมต่อหรือไม่: **เชื่อมต่อถ้าจำเป็น**

เมื่อผู้ใช้เข้าถึงโดเมนเหล่านี้:*ชื่อโดเมน***เป้าหมาย**

ถ้าการกำหนดค่าด้านบนไม่สำเร็จให้เพิ่มองค์ประกอบต่อไปนี้:

เมื่อ URL นี้ไม่สามารถเข้าถึงให้บังคับเชื่อมต่อ VPN: **BADURL**
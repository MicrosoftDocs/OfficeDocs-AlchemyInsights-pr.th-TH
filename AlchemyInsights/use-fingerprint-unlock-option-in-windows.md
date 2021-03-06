---
title: ใช้ตัวเลือกปลดล็อกลายนิ้วมือใน Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: 99f037f62748c06d77b526e35f67b711885c4a1e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47795263"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>ใช้ตัวเลือกปลดล็อกลายนิ้วมือใน Windows 10

**เปิดใช้งาน Windows สวัสดีลายนิ้วมือ**

เมื่อต้องการปลดล็อก Windows 10 โดยใช้ลายนิ้วมือของคุณคุณจำเป็นต้องตั้งค่า Windows สวัสดีลายนิ้วมือโดยการเพิ่ม (ให้ Windows เรียนรู้ที่จะจดจำ) อย่างน้อยหนึ่งนิ้ว 

1. ไปที่ **การตั้งค่า > บัญชีผู้ใช้ > ตัวเลือกการลงชื่อเข้าใช้** (หรือคลิก [ที่นี่](ms-settings:signinoptions?activationSource=GetHelp)) ตัวเลือกการลงชื่อเข้าใช้ที่พร้อมใช้งานจะแสดงอยู่ในรายการ ตัวอย่างเช่น:

    ![ตัวเลือกการลงชื่อเข้าใช้](media/sign-in-options.png)

2. คลิกหรือแตะที่**Windows สวัสดีลายนิ้วมือ**แล้วคลิก**ตั้งค่า** ในหน้าต่างการตั้งค่า Windows Hello ให้คลิก **เริ่มต้น**ใช้งาน เซนเซอร์ลายนิ้วมือจะเปิดใช้งานและคุณจะถูกขอให้วางนิ้วของคุณบนเซนเซอร์:

   ![เซนเซอร์ลายนิ้วมือ](media/fingerprint-sensor.png)

3. ทำตามคำแนะนำซึ่งจะขอให้คุณสแกนนิ้วของคุณซ้ำๆ เมื่อการดำเนินการนี้เสร็จสิ้นคุณจะมีตัวเลือกในการเพิ่มนิ้วอื่นๆที่คุณอาจต้องการใช้สำหรับการลงชื่อเข้าใช้ ในครั้งถัดไปที่คุณลงชื่อเข้าใช้ Windows 10 คุณจะมีตัวเลือกในการใช้ลายนิ้วมือของคุณเพื่อทำเช่นนั้น

**Windows สวัสดีลายนิ้วมือไม่พร้อมใช้งานเป็นตัวเลือกการลงชื่อเข้าใช้**

ถ้า Windows สวัสดีลายนิ้วมือไม่แสดงเป็นตัวเลือกใน **ตัวเลือกการลงชื่อเข้าใช้**หมายความว่า windows ไม่ทราบตัวอ่านลายนิ้วมือ/สแกนเนอร์ที่แนบมากับพีซีของคุณหรือนโยบายของระบบจะป้องกันไม่ให้มีการใช้ (ตัวอย่างเช่นพีซีของคุณได้รับการจัดการโดยที่ทำงานของคุณ) เมื่อต้องการแก้ไขปัญหา: 

1. เลือกปุ่ม**เริ่ม**ในแถบงานและค้นหา**ตัวจัดการอุปกรณ์**

2. คลิกหรือแตะเพื่อเปิด**ตัวจัดการอุปกรณ์**

3. ในตัวจัดการอุปกรณ์ให้ขยายอุปกรณ์ทางชีวมาตรโดยการคลิกเครื่องหมายบั้ง

   ![อุปกรณ์ทางชีวมาตร](media/biometric-devices.png)

4. สแกนเนอร์ลายนิ้วมือของคุณควรจะแสดงเป็นอุปกรณ์ชีวมาตรเช่นเครื่องสแกนเนอร์ Synaptics WBDI:

   ![อุปกรณ์ทางชีวมาตร](media/biometric-devices-expanded.png)

5. ถ้าสแกนเนอร์ลายนิ้วมือของคุณไม่แสดงขึ้นและเครื่องสแกนเนอร์รวมอยู่ในพีซีของคุณให้ไปที่เว็บไซต์ของผู้ผลิตพีซี ในส่วนการสนับสนุนทางเทคนิคสำหรับรุ่นพีซีของคุณให้ค้นหาโปรแกรมควบคุม Windows 10 สำหรับสแกนเนอร์ที่คุณสามารถติดตั้งได้

6. ถ้าสแกนเนอร์ถูกแยกออกจากพีซี (ที่แนบมาผ่าน USB) ให้ไปที่เว็บไซต์ของผู้ผลิตสแกนเนอร์เพื่อค้นหาและติดตั้งซอฟต์แวร์โปรแกรมควบคุมอุปกรณ์ Windows 10 สำหรับรุ่นสแกนเนอร์ที่คุณมี

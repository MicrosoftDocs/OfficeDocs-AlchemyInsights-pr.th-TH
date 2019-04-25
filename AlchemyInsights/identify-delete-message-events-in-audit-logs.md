---
title: ระบุเหตุการณ์ข้อความลบในบันทึกการตรวจสอบ
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1370
ms.assetid: ''
ms.openlocfilehash: 93f8a192af6e689e2b2d04013f35b8da2b69e607
ms.sourcegitcommit: ffe2f489b1ac3aae62aa784c959da6a41c3261eb
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/17/2019
ms.locfileid: "31909621"
---
# <a name="audit-logs-for-deleted-email-messages"></a>บันทึกการตรวจสอบสำหรับข้อความอีเมลที่ถูกลบ

เริ่มต้นในเดือน 2019 มกราคม Microsoft มีการเปิดใช้งานการเข้าสู่ระบบ โดยค่าเริ่มต้นการตรวจสอบกล่องจดหมาย มิฉะนั้น เพื่อทบทวนเหตุการณ์ข้อความลบสำหรับผู้ใช้ที่ระบุ คุณจำเป็นต้องเปิดใช้งานการดำเนินการลบสำหรับการตรวจสอบได้ด้วยตนเอง ถ้ากล่องจดหมายการตรวจสอบ บันทึกแล้วเปิดใช้งาน สำหรับองค์กรของคุณ หรือผู้ใช้เฉพาะ ให้ทำตามขั้นตอนด้านล่างนี้

1. เข้าสู่ระบบไปยัง[ศูนย์ปฏิบัติตามกฎระเบียบ & 365 ความปลอดภัยของ Office](https://protection.office.com/)

2. คลิก**ค้นหาและการตรวจสอบ**และ**ค้นหาแฟ้มบันทึกการตรวจสอบบัญชี**ที่เลือก

3. เลือกช่วงวันที่ในฟิลด์**วันเริ่มต้น**และ**วันสิ้นสุด** ระบุชื่อผู้ใช้สำหรับผู้ใช้ที่คุณต้องการตรวจสอบ (ผู้ใช้ที่ลบรายการ) ในฟิลด์**กิจกรรม**เลือก**ข้อความที่ถูกลบจากโฟลเดอร์รายการที่ถูกลบ**และ**Moved ข้อความไปยังโฟลเดอร์รายการที่ถูกลบ**

4. คลิก**ค้นหา**

ในผลลัพธ์ เลือกบันทึกการตรวจสอบ ในเมนูลอยขึ้นรายละเอียด คลิ**กข้อมูลเพิ่มเติม** ข้อมูลเพิ่มเติมเกี่ยวกับรายการถูกลบไปแล้ว (ตัวอย่างเช่น บรรทัดชื่อเรื่องและตำแหน่งที่ตั้งของสินค้าเมื่อถูกลบ) จะแสดงในเขตข้อมูล**AffectedItems** คุณสมบัติ**ClientInfoString**จะแสดงถ้าการลบเกิดขึ้นใน Outlook, Outlook บนเว็บ (ซึ่งเดิมเรียกว่า Outlook Web App), หรืออุปกรณ์อื่น ๆ

สำหรับข้อมูลเพิ่มเติม ดู[Determining ที่ติดตั้งอีเมลที่ส่งต่อสำหรับกล่องจดหมาย](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items)

**หมายเหตุ**: คุณไม่สามารถเรียกใช้คุณลักษณะแฟ้มบันทึกการตรวจสอบรายการที่ถูกลบได้ เมื่อต้องการเรียกข้อความที่ถูกลบใน Outlook บนเว็บ ดู[กู้คืนรายการใน Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4)
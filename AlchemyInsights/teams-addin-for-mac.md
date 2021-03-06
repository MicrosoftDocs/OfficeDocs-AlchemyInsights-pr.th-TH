---
title: Add-in ของทีมสำหรับ Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "9003233"
ms.openlocfilehash: 1e5f6d66386398ad8600f9383f9f7a1dcf0ce69f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670347"
---
# <a name="teams-add-in-for-mac"></a>Add-in ของทีมสำหรับ Mac

เมื่อต้องการแก้ไขปัญหาสำหรับผู้ใช้ระบบปฏิบัติการของระบบปฏิบัติการของ Mac ที่ขาดหายไปให้ทำตามขั้นตอนต่อไปนี้:

**ขั้นตอนที่ 1:** ถ้าคุณมี Exchange แบบไฮบริดในองค์กร (๒๐๑๖ CU3 หรือใหม่กว่าที่จำเป็น) ให้ใช้เครื่องมือ Test-HMA.ps1 เพื่อยืนยันว่าการรับรองความถูกต้องแบบไฮบริดที่ทันสมัยถูกกำหนดค่าอย่างถูกต้อง สำหรับข้อมูลเพิ่มเติมให้ดูที่การ[ตรวจสอบการตั้งค่าการรับรองความถูกต้องแบบไฮบริดที่ทันสมัยสำหรับ Outlook สำหรับ iOS และ Android](https://aka.ms/AA980zq)  

**หมายเหตุ:** ใช้รูปแบบที่อยู่ UPN (ตัวอย่างเช่น [username@contoso.com](mailto:username@contoso.com)), not domain\username. ให้ทำสิ่งนี้แม้แต่สำหรับผู้ใช้ที่มีกล่องจดหมาย Exchange Online

**ขั้นตอนที่ 2:** มีผู้ใช้ไปที่**บัญชีเครื่องมือ**  >  **Accounts**... ใน Outlook for Mac และค้นหาและเลือกบัญชีผู้ใช้ ยืนยันชื่อผู้ใช้ที่แสดงอยู่ในรูปแบบ UPN (ตัวอย่างเช่น [username@contoso.com](mailto:username@contoso.com))

**ขั้นตอนที่ 3:** ยืนยันผู้ใช้เป็นผู้ใช้ Microsoft team ที่ได้รับสิทธิ์การใช้งาน ผู้ใช้ต้องใช้การสมัครใช้งาน Office ๓๖๕ for Mac เวอร์ชันผลิตภัณฑ์๑๖.๒๔หรือเวอร์ชันที่ใหม่กว่า
---
title: เครื่องมือส่งออก eDiscovery
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
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: 67e59182a5053111a08f5fb2be814931a1aa815d
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277920"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>ไม่สามารถติดตั้งหรือเรียกใช้เครื่องมือส่งออก eDiscovery ได้ใช่หรือไม่

ถ้าคุณไม่สามารถติดตั้งหรือเรียกใช้เครื่องมือส่งออก eDiscovery เพื่อดาวน์โหลดผลลัพธ์การค้นหาให้ตรวจสอบสิ่งต่อไปนี้:
  
- คอมพิวเตอร์ที่คุณกำลังใช้ตรงกับ requisites เหล่านี้:

  - Windows 7 เวอร์ชัน๓๒หรือ๖๔บิตและเวอร์ชันที่ใหม่กว่า

  - Microsoft .NET Framework 4.7

  - เบราว์เซอร์ที่ได้รับการสนับสนุน:

  - Microsoft Edge

    หรือ

  - Internet Explorer 10 และเวอร์ชันที่ใหม่กว่า

    เบราว์เซอร์อื่นๆเช่น Google Chrome และ Mozilla Firefox จะไม่ได้รับการสนับสนุน

- องค์กรของคุณสามารถเชื่อมต่อกับจุดสิ้นสุดใน Azure ซึ่งเป็น** \* blob.core.windows.net** (อักขระตัวแทนจะแสดงตัวระบุที่ไม่ซ้ำกันสำหรับงานส่งออกของคุณ)

- คุณได้รับมอบหมายบทบาทการส่งออกใน &amp; ศูนย์การปฏิบัติตามนโยบายด้านความปลอดภัยของ Microsoft ๓๖๕ ตามค่าเริ่มต้นบทบาทนี้จะได้รับการกำหนดให้กับกลุ่มบทบาทผู้จัดการ eDiscovery เท่านั้น ให้ดูที่[กำหนดสิทธิ์ eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)

สำหรับข้อมูลเพิ่มเติมให้ดูที่[ส่งออกผลลัพธ์การค้นหาเนื้อหา](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)

ถ้าคุณกำลังส่งออกกล่องจดหมายมากกว่า100K คุณจะต้องใช้ Powershell ต่อไปนี้เพื่อดาวน์โหลดผลลัพธ์การส่งออก:[ส่งออกผลลัพธ์จากกล่องจดหมายมากกว่า 100k](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)
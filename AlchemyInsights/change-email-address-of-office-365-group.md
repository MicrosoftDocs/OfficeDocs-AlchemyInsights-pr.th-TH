---
title: เปลี่ยนที่อยู่อีเมลของกลุ่ม Microsoft ๓๖๕
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: a2605bcd66f61de811ebb6e273e4ef1cff2b0119
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47733706"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>เปลี่ยนที่อยู่อีเมลของกลุ่ม Microsoft ๓๖๕

คุณสามารถเปลี่ยนที่อยู่อีเมลของกลุ่ม Microsoft ๓๖๕โดยใช้ศูนย์การจัดการ เพียงเลือกกลุ่มแล้วเลือก @edit อีเมลแอดเดรส

นอกจากนี้คุณยังสามารถใช้คำสั่ง EXO PowerShell เพื่อเปลี่ยนที่อยู่ SMTP หลักของกลุ่ม Microsoft ๓๖๕ได้ดังนี้

ตั้งค่า-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

ตัวอย่าง

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```

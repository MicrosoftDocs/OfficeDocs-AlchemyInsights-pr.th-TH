---
title: จัดการผู้ใช้ที่ซิงโครไนซ์
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
- "9000609"
- "2444"
ms.openlocfilehash: 7bf7d3f00308ff6bc973cd52e09ca51c5fd0f45b
ms.sourcegitcommit: 1fb324fd156008e77b7e2008af4b3dc1c0d0ea3e
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/13/2020
ms.locfileid: "48451419"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>ไม่สามารถตั้งค่าที่อยู่อีเมลหลักเปลี่ยนแอตทริบิวต์ของผู้ใช้หรือลบ/ลบผู้ใช้ที่ซิงโครไนซ์ได้

ถ้ามีการเปิดใช้งานการซิงโครไนซ์ไดเรกทอรีสำหรับสภาพแวดล้อมของคุณคุณจะไม่สามารถเปลี่ยนแอตทริบิวต์บางอย่างของผู้ใช้หรือวัตถุได้โดยใช้ศูนย์การจัดการ Microsoft ๓๖๕

เมื่อต้องการจัดการผู้ใช้ที่ซิงโครไนซ์และแอตทริบิวต์ทั้งหมดโดยสมบูรณ์ให้ใช้ผู้ใช้ของไดเรกทอรีที่ใช้งานอยู่ภายในเครื่องของคุณและคอนโซลการจัดการกลุ่ม (adsiedit. msc)  

อีกวิธีหนึ่งคือคุณสามารถเปลี่ยนผู้ใช้แต่ละรายหรือแอตทริบิวต์สำหรับผู้ใช้ที่ทำข้อมูลให้ตรงกันโดยใช้ powershell เช่นที่แสดงในตัวอย่างทั่วไปเหล่านี้:

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`

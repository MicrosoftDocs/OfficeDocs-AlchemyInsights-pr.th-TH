---
title: การเปลี่ยนการตั้งค่าการควบคุมปริมาณ EWS
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
- "9000752"
- "5653"
- "5760"
ms.openlocfilehash: 4f0bea884153dc1ed8699ce12e0d017d18f5e57c
ms.sourcegitcommit: 53e5caab697ebfb434ccef3ef98b8f2bee579b41
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/02/2021
ms.locfileid: "50075916"
---
# <a name="changing-ews-throttling-settings"></a>การเปลี่ยนการตั้งค่าการควบคุมปริมาณ EWS

โปรดเรียกใช้การทดสอบอัตโนมัติของเราซึ่งจะช่วยให้คุณปรับเปลี่ยนนโยบายการควบคุมปริมาณ EWS ในช่วงระยะเวลาการโยกย้ายของคุณ โปรดทราบว่า แม้หลังจากเรียกใช้การนําเข้า EWS จะยังคงถูกจํากัดที่ 150mb ต่อ 5 นาทีต่อกล่องจดหมาย เพื่อให้ได้รับความเร็วในการโยกย้ายที่สูงขึ้น โปรดโยกย้ายผู้ใช้พร้อมกันมากขึ้น

โปรดทราบว่าการเปลี่ยนแปลงนโยบายการควบคุมปริมาณ EWS จะไม่มีผลต่อชนิดการโยกย้ายต่อไปนี้ (โดยใช้เครื่องมือของ Microsoft): ไฮบริด, แบบไฮบริด, แบบเคลื่อนย้าย/แบบเป็นขั้นตอน (RPC/HTTP), IMAP, G Suite, โฟลเดอร์สาธารณะหรือบริการการนําเข้า PST
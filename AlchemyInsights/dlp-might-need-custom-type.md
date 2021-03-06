---
title: DLP อาจจำเป็นต้องมีชนิดแบบกำหนดเอง
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 72b16d437f97de27cbdc364f022c3e2059b31ef0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712203"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP อาจจำเป็นต้องมีชนิดแบบกำหนดเอง

**สำคัญ**: ในช่วงเวลาที่เป็นประวัติการณ์เหล่านี้เราจะดำเนินการตามขั้นตอนเพื่อให้แน่ใจว่าบริการ sharepoint Online และ OneDrive ยังคงพร้อมใช้งานอย่างมาก–โปรดไปที่การ [ปรับปรุงฟีเจอร์ชั่วคราวของ sharepoint Online](https://aka.ms/ODSPAdjustments) สำหรับข้อมูลเพิ่มเติม

**DLP อาจจำเป็นต้องมีชนิดข้อมูลแบบกำหนดเอง**

ด้วยนโยบายการป้องกันการสูญหายของข้อมูล (DLP) คุณสามารถระบุและป้องกันข้อมูลที่สำคัญในองค์กรของคุณได้ ในบางสถานการณ์คุณอาจจำเป็นต้องสร้างชนิดข้อมูลที่ละเอียดอ่อน **แบบกำหนดเอง** ของคุณเองเพื่อป้องกันข้อมูลขององค์กรของคุณ

ตัวอย่างเช่นองค์กรของคุณอาจจำเป็นต้องระบุและป้องกัน Id ของพนักงานหรือข้อมูลอื่นๆในรูปแบบบางอย่างที่เฉพาะเจาะจงสำหรับองค์กรของคุณ ถ้าเป็นเช่นนั้นให้ดูบทความต่อไปนี้สำหรับข้อมูลเพิ่มเติม
  
 **การกำหนดชนิดข้อมูลที่เป็นความลับที่มีอยู่แล้วภายใน**
  
ถ้าชนิดข้อมูลที่เป็นความลับที่มีอยู่แล้วภายในจะตอบสนองความต้องการของคุณได้ด้วยการปรับแต่งเพียงไม่กี่ครั้งคุณสามารถ [กำหนดชนิดข้อมูลที่เป็นความลับที่มีอยู่แล้วภายใน](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type)ได้ ตัวอย่างเช่นคุณสามารถเพิ่มหรือลบคำสำคัญหรือเพิ่มหรือเอาหลักฐานสนับสนุนออกเช่นวันที่หรือที่อยู่
  
 **การสร้างชนิดข้อมูลที่เป็นความลับแบบกำหนดเอง**
  
แต่ถ้าคุณต้องการระบุและป้องกันชนิดของข้อมูลที่เป็นความลับที่แตกต่างกันทั้งหมดคุณสามารถ [สร้างชนิดข้อมูลที่สำคัญที่กำหนดเอง](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) ใน UI ของศูนย์การปฏิบัติตามนโยบายการรักษาความปลอดภัย &
  
**การสร้างชนิดข้อมูลที่มีความสำคัญแบบกำหนดเองในการรักษาความปลอดภัย & ศูนย์การปฏิบัติตามนโยบายของ PowerShell**

สุดท้ายถ้า UI ไม่มีตัวเลือกทั้งหมดที่คุณต้องการคุณสามารถ[สร้างชนิดข้อมูลที่สำคัญที่กำหนดเองได้ในศูนย์การรักษาความปลอดภัย & การปฏิบัติตามนโยบายศูนย์การปฏิบัติตามนโยบาย](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell) โดยเริ่มต้นด้วยไฟล์ XML คุณสามารถใช้ตัวเลือกทั้งหมดที่พร้อมใช้งานได้

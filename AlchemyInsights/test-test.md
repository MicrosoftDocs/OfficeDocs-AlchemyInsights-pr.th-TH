---
title: เงื่อนไขที่หายไปจากที่เก็บคำของ SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 06711c289365c0fcdf71cf9cccf3cfc53511495a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750470"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>การเปิดใช้งานการเข้ารหัสลับ Bitlocker ด้วย Intune

นโยบายการป้องกันจุดสิ้นสุดของ Intune สามารถใช้ในการกำหนดค่าการตั้งค่าการเข้ารหัสลับ Boitlocker สำหรับอุปกรณ์ Windows ตามที่อธิบายไว้ใน: Windows10 (และใหม่กว่า) การตั้งค่าเพื่อป้องกันอุปกรณ์โดยใช้ Intune

คุณควรทราบว่าอุปกรณ์รุ่นใหม่จำนวนมากที่ใช้ Windows 10 สนับสนุนการเข้ารหัสลับด้วย bitlocker โดยอัตโนมัติที่ทริกเกอร์โดยไม่มีแอปพลิเคชันของนโยบาย MDM การทำเช่นนี้อาจส่งผลกระทบต่อการใช้นโยบายถ้าการตั้งค่าที่ไม่ใช่ค่าเริ่มต้นถูกกำหนดค่า ดูคำถามที่ถามบ่อยสำหรับรายละเอียดเพิ่มเติม


คำถามที่ถามบ่อย   : คำถามที่ถามบ่อย: Windows สนับสนุนการเข้ารหัสลับอุปกรณ์โดยใช้นโยบายการป้องกันจุดสิ้นสุดหรือไม่
 A: การตั้งค่าในนโยบายการป้องกันจุดสิ้นสุดของ Intune จะถูกนำไปใช้โดยใช้ CSP ของ Bitlockerไม่ใช่เวอร์ชันทั้งหมดหรือรุ่นของ Windows สนับสนุน Bitlocker CSP 
      ในตอนนี้ Windows รุ่น: Enterprise; การศึกษา, โทรศัพท์มือถือ, องค์กรมือถือและมืออาชีพ (จากรุ่น๑๘๐๙เป็นต้นไป) ได้รับการสนับสนุน




Q: ถ้าอุปกรณ์ถูกเข้ารหัสลับด้วย Bitlocker โดยใช้การตั้งค่าเริ่มต้นของระบบปฏิบัติการสำหรับการเข้ารหัสลับและความแรงของการเข้ารหัส (XTS-AES-๑๒๘) จะนำนโยบายที่มีการตั้งค่าที่แตกต่างกันโดยอัตโนมัติทริกเกอร์การเข้ารหัสลับของไดรฟ์ด้วยการตั้งค่าใหม่อีกครั้ง

A: ไม่ใช่ เมื่อต้องการนำการตั้งค่าการเข้ารหัสใหม่ไปใช้ก่อนที่คุณจะต้องถอดรหัสลับไดรฟ์ออกก่อน

หมายเหตุสำหรับอุปกรณ์ที่ลงทะเบียนด้วย Autopilot การเข้ารหัสลับอัตโนมัติที่จะเกิดขึ้นระหว่าง OOBE จะไม่ทริกเกอร์จนกว่าจะมีการประเมินนโยบายของ Intune จนกว่าจะมีการประเมินนโยบายของ Intune ที่อนุญาตให้ใช้การตั้งค่านโยบายที่จะใช้แทนที่ค่าเริ่มต้นของระบบปฏิบัติการ




Q ถ้าอุปกรณ์ถูกเข้ารหัสลับเป็นผลลัพธ์ของแอปพลิเคชันของ Intune ของ Intune จะถูกถอดรหัสลับเมื่อนโยบายนั้นถูกเอาออกหรือไม่

A: การลบนโยบายที่เกี่ยวข้องกับการเข้ารหัสลับไม่ทำให้เกิดการถอดรหัสลับของไดรฟ์ที่ได้รับการกำหนดค่า




Q: เหตุใดนโยบายการปฏิบัติตามนโยบายของ intune ของ intune จึงแสดงว่าอุปกรณ์ของฉันไม่มี "Bitlocker เปิดใช้งาน" แต่จะเป็นอย่างไร

A: การตั้งค่า "เปิดใช้งาน Bitlocker" ในนโยบายการปฏิบัติตามนโยบายของ intune ใช้ไคลเอ็นต์ Windows อุปกรณ์สถานภาพรับรอง (DHA) ไคลเอ็นต์นี้จะวัดสถานะอุปกรณ์ในเวลาเริ่มต้นเท่านั้น ดังนั้นถ้าอุปกรณ์ยังไม่ได้รับการรีบูตเนื่องจากการเข้ารหัสลับด้วย bitlocker เสร็จสมบูรณ์บริการไคลเอ็นต์ของ DHA จะไม่รายงาน bitlocker เป็นการใช้งานอยู่
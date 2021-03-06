---
title: 'ข้อผิดพลาดการลงทะเบียนองค์กรของ Android: การตรวจสอบการตั้งค่า MGP'
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000652"
- "8340"
ms.openlocfilehash: 6ac90611bbe626e7f11b817965fd2d3c7fbf98c1
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/05/2021
ms.locfileid: "50508572"
---
# <a name="android-enterprise-enrollment-error-mgp-set-up-detection"></a><span data-ttu-id="7ead4-102">ข้อผิดพลาดการลงทะเบียนองค์กรของ Android: การตรวจสอบการตั้งค่า MGP</span><span class="sxs-lookup"><span data-stu-id="7ead4-102">Android Enterprise enrollment error: MGP set-up detection</span></span>

<span data-ttu-id="7ead4-103">เราตรวจพบว่า Managed Google Play ไม่ได้ตั้งค่าหรือยกเลิกการเชื่อมต่อในบัญชีของคุณ</span><span class="sxs-lookup"><span data-stu-id="7ead4-103">We have detected that Managed Google Play is not set up or disconnected for your account.</span></span> <span data-ttu-id="7ead4-104">ซึ่งสามารถทําให้ไม่สามารถลงทะเบียนอุปกรณ์ในสถานการณ์ของ Android Enterprise ที่ต้องใช้การเชื่อมต่อ Google Play ที่จัดการ</span><span class="sxs-lookup"><span data-stu-id="7ead4-104">This can cause failure to enroll devices in Android Enterprise scenarios where a Managed Google Play connection is required.</span></span>

<span data-ttu-id="7ead4-105">คุณสามารถตรวจสอบสถานะการเชื่อมต่อของ Google Play ที่จัดการในคอนโซล MEM ภายใต้การดูแลผู้เช่า > สถานะผู้เช่า **> สถานะ** ตัวเชื่อมต่อ และตรวจสอบเอกสารประกอบต่อไปนี้เพื่อเรียนรู้เกี่ยวกับวิธีการเชื่อมต่อบัญชี Intuned กับบัญชี Google ที่จัดการของคุณ: เชื่อมต่อบัญชี **[Intuned](https://docs.microsoft.com/mem/intune/enrollment/connect-intune-android-enterprise)** กับบัญชี Google Play ที่จัดการของคุณ</span><span class="sxs-lookup"><span data-stu-id="7ead4-105">You can check Managed Google Play Connection status in the MEM console under **Tenant Administration > Tenant status > Connector status** and review the following documentation to learn about how to connect your Intune account to your Managed Google account: **[Connect your Intune account to your Managed Google Play account](https://docs.microsoft.com/mem/intune/enrollment/connect-intune-android-enterprise)**.</span></span>

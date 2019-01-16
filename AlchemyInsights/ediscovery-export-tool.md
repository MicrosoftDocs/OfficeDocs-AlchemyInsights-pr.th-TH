---
title: เครื่องมือส่ง eDiscovery
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 8/3/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: f3c184cb19f61d8d294cef4f4c06fd972d2fda8c
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/15/2019
ms.locfileid: "28315973"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="e78a0-102">ไม่สามารถติดตั้ง หรือเรียกใช้ eDiscovery เครื่องมือการส่งออกหรือไม่</span><span class="sxs-lookup"><span data-stu-id="e78a0-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="e78a0-103">ถ้าคุณไม่สามารถติดตั้ง หรือเรียกใช้ eDiscovery Office 365 ส่งออกเครื่องมือการดาวน์โหลดผลลัพธ์การค้นหา ตรวจสอบสิ่งต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="e78a0-103">If you can't install or run the Office 365 eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="e78a0-104">คุณกำลังใช้คอมพิวเตอร์ตรงตามเบื้องต้นเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="e78a0-104">The computer you're using meets these pre-requisites:</span></span>
    
  - <span data-ttu-id="e78a0-105">รุ่น 32 หรือ 64 บิตของ Windows 7 และรุ่นที่ใหม่กว่า</span><span class="sxs-lookup"><span data-stu-id="e78a0-105">32- or 64-bit versions of Windows 7 and later versions</span></span>
    
  - <span data-ttu-id="e78a0-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="e78a0-106">Microsoft .NET Framework 4.7</span></span>
    
  - <span data-ttu-id="e78a0-107">เบราว์เซอร์ที่สนับสนุน:</span><span class="sxs-lookup"><span data-stu-id="e78a0-107">A supported browser:</span></span>
    
  - <span data-ttu-id="e78a0-108">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="e78a0-108">Microsoft Edge</span></span>
    
    <span data-ttu-id="e78a0-109">หรือ</span><span class="sxs-lookup"><span data-stu-id="e78a0-109">Or</span></span>
    
  - <span data-ttu-id="e78a0-110">Internet Explorer 10 และรุ่นที่ใหม่กว่า</span><span class="sxs-lookup"><span data-stu-id="e78a0-110">Internet Explorer 10 and later versions</span></span>
    
    <span data-ttu-id="e78a0-111">เบราว์เซอร์อื่น เช่น Google โครเมียมและ Mozilla Firefox จะไม่ได้รับการสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="e78a0-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>
    
- <span data-ttu-id="e78a0-112">องค์กรของคุณสามารถเชื่อมต่อกับปลายทางใน Azure ซึ่งก็คือ**\*ได้ blob.core.windows.net** (สัญลักษณ์ตัวแทนแสดงถึงตัวระบุเฉพาะสำหรับงานการส่งออกของคุณ) ได้</span><span class="sxs-lookup"><span data-stu-id="e78a0-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span> 
    
- <span data-ttu-id="e78a0-p101">คุณได้รับมอบหมายบทบาทส่งออกในการรักษาความปลอดภัยใน Office 365&amp;ศูนย์ปฏิบัติตามกฎระเบียบ โดยค่าเริ่มต้น บทบาทนี้จะถูกกำหนดให้กับกลุ่มบทบาทผู้จัดการ eDiscovery เท่านั้น ดู[กำหนดการอนุญาต eDiscovery](https://support.office.com/article/assign-ediscovery-permissions-in-the-office-365-security-compliance-center-5b9a067b-9d2e-4aa5-bb33-99d8c0d0b5d7#moreinfo)</span><span class="sxs-lookup"><span data-stu-id="e78a0-p101">You're assigned the Export role in the Office 365 Security &amp; Compliance Center. By default, this role is only assigned to the eDiscovery Manager role group. See [Assign eDiscovery permissions](https://support.office.com/article/assign-ediscovery-permissions-in-the-office-365-security-compliance-center-5b9a067b-9d2e-4aa5-bb33-99d8c0d0b5d7#moreinfo).</span></span>
    
<span data-ttu-id="e78a0-116">สำหรับข้อมูลเพิ่มเติม ให้ดู[ผลลัพธ์การค้นหาเนื้อหาที่มีการส่งออก](https://support.office.com/article/Export-Content-Search-results-from-the-Office-365-Security-Compliance-Center-ed48d448-3714-4c42-85f5-10f75f6a4278)</span><span class="sxs-lookup"><span data-stu-id="e78a0-116">For more information, see [Export Content Search results](https://support.office.com/article/Export-Content-Search-results-from-the-Office-365-Security-Compliance-Center-ed48d448-3714-4c42-85f5-10f75f6a4278).</span></span>
  

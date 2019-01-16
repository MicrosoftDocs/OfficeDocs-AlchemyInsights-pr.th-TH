---
title: AADConnect การปรับรุ่น 932
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 9add88a0e4a2590639cbfc546afdcdf5e6aa4886
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/15/2019
ms.locfileid: "28316857"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="fd1e7-102">การเชื่อมต่อ Azure AD การปรับรุ่น</span><span class="sxs-lookup"><span data-stu-id="fd1e7-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="fd1e7-p101">โดยค่าเริ่มต้น การอัพเกรดอัตโนมัติถูกเปิดใช้งานสำหรับการเชื่อมต่อ AD Azure ซึ่งช่วยให้แน่ใจว่าคุณกำลังเรียกใช้รุ่นล่าสุด เมื่อต้องการตรวจสอบการตั้งค่าการปรับรุ่นอัตโนมัติ ใช้ cmdlet การ**ADSyncAutoUpgrade รับ**ใน PowerShell โฆษณา Azure Cmdlet นี้จะส่งกลับค่าหนึ่งค่าต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="fd1e7-p101">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version. To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell. The cmdlet will return one of following values:</span></span> 
  
- <span data-ttu-id="fd1e7-106">**เปิดการใช้งาน**: เปิดใช้งานการปรับรุ่นโดยอัตโนมัติ</span><span class="sxs-lookup"><span data-stu-id="fd1e7-106">**Enabled**: Automatic upgrade is enabled.</span></span> 
    
- <span data-ttu-id="fd1e7-107">**ปิดการใช้งาน**: การอัพเกรดอัตโนมัติถูกปิดใช้งาน</span><span class="sxs-lookup"><span data-stu-id="fd1e7-107">**Disabled**: Automatic upgrade is disabled.</span></span> 
    
- <span data-ttu-id="fd1e7-p102">**ระงับ**: ระบบไม่มีสิทธิ์ได้รับการปรับรุ่นโดยอัตโนมัติ คุณไม่สามารถกำหนดค่านี้ จะถูกกำหนด โดยระบบ</span><span class="sxs-lookup"><span data-stu-id="fd1e7-p102">**Suspended**: The system is no longer eligible to receive automatic upgrades. You can't configure this value; it's set by the system.</span></span> 
    
<span data-ttu-id="fd1e7-110">สำหรับข้อมูลเพิ่มเติม ดู[การอัพเกรดโดยอัตโนมัติ](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)</span><span class="sxs-lookup"><span data-stu-id="fd1e7-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>
  
<span data-ttu-id="fd1e7-111">เมื่อต้องการดาวน์โหลดรุ่นล่าสุดของการเชื่อมต่อ AD Azure ไป[https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594)</span><span class="sxs-lookup"><span data-stu-id="fd1e7-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
  

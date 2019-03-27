---
title: 1491-search-not-returning-expected-results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 1491
ms.assetid: ''
ms.openlocfilehash: 517d9b75fc3aef09c0c2d5870aa695cc0ab10f06
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/22/2019
ms.locfileid: "30776100"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="fe430-102">ค้นหาเนื้อหาที่ไม่ส่งกลับผลลัพธ์ที่คาดไว้</span><span class="sxs-lookup"><span data-stu-id="fe430-102">Content Search not returning expected results</span></span>

<span data-ttu-id="fe430-103">เมื่อรันการค้นหาเนื้อหาจาก & Office 365 Security Center การปฏิบัติตามกฎระเบียบ คุณอาจได้รับผลลัพธ์การค้นหาที่ไม่คาดคิด</span><span class="sxs-lookup"><span data-stu-id="fe430-103">When running Content Searches from the Office 365 Security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="fe430-104">พิจารณาสิ่งต่อไปนี้ที่สามารถส่งผลกระทบต่อผลลัพธ์การค้นหาของคุณ:</span><span class="sxs-lookup"><span data-stu-id="fe430-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="fe430-105">**ตำแหน่งที่ตั้งเนื้อหาและเงื่อนไขการค้นหา**: ตรวจสอบว่า คุณได้เลือกตำแหน่งที่ตั้งเนื้อหาที่เหมาะสม และเงื่อนไขการค้นหา</span><span class="sxs-lookup"><span data-stu-id="fe430-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="fe430-106">ถ้าคุณเรียกใช้การค้นหาที่มีขนาดใหญ่ (มีหลายตำแหน่งที่ตั้ง), พิจารณาเป็นการแบ่งเป็นหลายการค้นหา</span><span class="sxs-lookup"><span data-stu-id="fe430-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="fe430-107">**ดัชนีรายการบางส่วน**:[ดัชนีสินค้าบางส่วน](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search)จากกล่องจดหมายที่รวมอยู่ในผลลัพธ์การค้นหาที่ประเมิน</span><span class="sxs-lookup"><span data-stu-id="fe430-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="fe430-108">อย่างไรก็ตาม สินค้าบางส่วนมีการทำดัชนีจากไซต์ SharePoint และ OneDrive จะไม่ถูกรวมในการประเมินการค้นหา</span><span class="sxs-lookup"><span data-stu-id="fe430-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="fe430-109">**ความล้มเหลวในการค้นหา**: เมื่อค้นหาจำนวนมากกล่องจดหมาย (กล่องจดหมายมากกว่า 100000), คุณอาจได้รับข้อผิดพลาดค้นหา ด้วยรหัสข้อผิดพลาดเช่น CS008 009 และ CS012-002 โดย) ได้</span><span class="sxs-lookup"><span data-stu-id="fe430-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="fe430-110">ในกรณีนี้ ลองการค้นหาตำแหน่งที่ตั้งเนื้อหาที่ล้มเหลวเท่านั้นอีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="fe430-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="fe430-111">ดู[บทความนี้](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search)สำหรับข้อมูลเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="fe430-111">See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
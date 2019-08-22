---
title: การกำหนดรุ่นใน SharePoint และ OneDrive
ms.author: efrene
author: efrene
ms.date: 8/07/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: a84868ba-7657-4f34-8a57-df9c6f9732dc
ms.custom:
- "5300025"
- "1702"
ms.openlocfilehash: 9c1ffe8c384a76d3df425623285fa4f9ebf757f2
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36503978"
---
# <a name="versioning-in-sharepoint-and-onedrive"></a><span data-ttu-id="a303c-102">การกำหนดรุ่นใน SharePoint และ OneDrive</span><span class="sxs-lookup"><span data-stu-id="a303c-102">Versioning in SharePoint and OneDrive</span></span> 


<span data-ttu-id="a303c-103">เมื่อเปิดใช้งานการกำหนดรุ่นในรายการ SharePoint หรือไลบรารีของคุณ คุณสามารถจัดเก็บ ติดตาม และคืนค่าในรายการและแฟ้มในไลบรารีเมื่อใดก็ ตามที่จะเปลี่ยนแปลง</span><span class="sxs-lookup"><span data-stu-id="a303c-103">When versioning is enabled in your SharePoint list or library, you can store, track, and restore items in a list and files in a library whenever they change.</span></span> <span data-ttu-id="a303c-104">กำหนดรุ่น รวมกับการตั้งค่าอื่น ๆ เช่นเช็คเอาท์ ช่วยให้คุณควบคุมเนื้อหาที่มีการลงรายการบัญชีบนไซต์ของคุณ และสามารถกำหนดค่าจริงถ้าคุณเคยมีความต้องการดู หรือคืนค่ารายการหรือแฟ้มรุ่นเก่า มากมาย</span><span class="sxs-lookup"><span data-stu-id="a303c-104">Versioning, combined with other settings, such as checkout, gives you a lot of control of the content that is posted on your site and can provide real value if you ever have a need to look at or restore an old version of an item or file.</span></span>

<span data-ttu-id="a303c-105">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการกำหนดรุ่นโปรดเยี่ยมชมด้านล่างของบทความ</span><span class="sxs-lookup"><span data-stu-id="a303c-105">For more information on versioning please visit the below articles.</span></span>

- [<span data-ttu-id="a303c-106">วิธีการกำหนดรุ่นไม่ทำในรายการ SharePoint หรือไลบรารี</span><span class="sxs-lookup"><span data-stu-id="a303c-106">How does versioning work in a SharePoint list or library</span></span>](https://support.office.com/article/how-does-versioning-work-in-a-sharepoint-list-or-library-0f6cd105-974f-44a4-aadb-43ac5bdfd247)

- [<span data-ttu-id="a303c-107">เปิดใช้งาน และกำหนดค่าการกำหนดรุ่นสำหรับรายการหรือไลบรารี</span><span class="sxs-lookup"><span data-stu-id="a303c-107">Enable and configure versioning for a list or library</span></span>](https://support.office.com/article/enable-and-configure-versioning-for-a-list-or-library-1555d642-23ee-446a-990a-bcab618c7a37?ocmsassetID=HA102772148&amp;CTT=3&amp;CorrelationId=52441bb1-a619-4375-89d5-19d28769890f&amp;ui=en-US&amp;rs=en-US&amp;ad=US)

- [<span data-ttu-id="a303c-108">วิธีการดูประวัติรุ่น</span><span class="sxs-lookup"><span data-stu-id="a303c-108">How to view version history</span></span>](https://support.office.com/article/View-the-version-history-of-an-item-or-file-in-a-list-or-library-53262060-5092-424D-A50B-C798B0EC32B1)

- [<span data-ttu-id="a303c-109">คืนค่ารุ่นก่อนหน้าของแฟ้มใน OneDrive</span><span class="sxs-lookup"><span data-stu-id="a303c-109">Restore a previous version of a file in OneDrive</span></span>](https://support.office.com/article/restore-a-previous-version-of-a-file-in-onedrive-159cad6d-d76e-4981-88ef-de6e96c93893?ui=en-US&amp;rs=en-US&amp;ad=US)

- [<span data-ttu-id="a303c-110">ดูไฟล์ Office เวอร์ชันก่อนหน้า</span><span class="sxs-lookup"><span data-stu-id="a303c-110">View previous versions of Office files</span></span>](https://support.office.com/article/view-previous-versions-of-office-files-5c1e076f-a9c9-41b8-8ace-f77b9642e2c2)

- [<span data-ttu-id="a303c-111">ขีดจำกัดการกำหนดรุ่น</span><span class="sxs-lookup"><span data-stu-id="a303c-111">Versioning limits</span></span>](https://docs.microsoft.com/office365/servicedescriptions/sharepoint-online-service-description/sharepoint-online-limits)

>[!Note] 
><span data-ttu-id="a303c-112">ถ้าคุณเป็นลูกค้า Office 365 การกำหนดรุ่นในขณะนี้เปิดอยู่ตามค่าเริ่มต้นเมื่อคุณสร้าง OneDrive ใหม่สำหรับไลบรารีของธุรกิจ และดังกล่าวโดยอัตโนมัติจะบันทึกเอกสารรุ่นล่าสุด 500</span><span class="sxs-lookup"><span data-stu-id="a303c-112">If you are an Office 365 customer, versioning is now turned on by default when you create new OneDrive for Business libraries, and it will automatically save the last 500 versions of a document.</span></span> <span data-ttu-id="a303c-113">ซึ่งจะช่วยให้คุณสามารถป้องกันการสูญเสียข้อมูลหรือเอกสารสำคัญ</span><span class="sxs-lookup"><span data-stu-id="a303c-113">This will help you prevent losing important documents or data.</span></span> <span data-ttu-id="a303c-114">ถ้าคุณมีไลบรารีที่มีอยู่ บน OneDrive ของคุณสำหรับไซต์ธุรกิจ หรือไซต์สำหรับทีมที่ไม่มีการเปิดใช้งานการกำหนดรุ่น คุณสามารถเปิดการกำหนดรุ่นสำหรับอุปกรณ์เหล่านี้เมื่อใดก็</span><span class="sxs-lookup"><span data-stu-id="a303c-114">If you have existing libraries on your OneDrive for Business site or on your team site that do not have versioning enabled, you can turn versioning on for them at any time.</span></span>



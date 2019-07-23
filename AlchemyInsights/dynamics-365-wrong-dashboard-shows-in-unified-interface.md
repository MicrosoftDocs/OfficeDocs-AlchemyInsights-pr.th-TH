---
title: Dynamics 365 - แดชบอร์ดไม่ถูกต้องแสดงในอินเทอร์เฟซประกอบการ Dynamics 365
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 6edf6fbae0174f3fa4d635c7a99e7daae1243b60
ms.sourcegitcommit: a413a0e27ef4ab8c484fa9fccff8bbef381c8b96
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/16/2019
ms.locfileid: "35748969"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="ae610-102">แดชบอร์ดไม่ถูกต้องที่แสดงในอินเทอร์เฟซประกอบการ Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="ae610-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="ae610-103">มีหลายเหตุผลที่ทำไมคุณอาจเห็นแดชบอร์ดแตกต่างจากคุณคาดว่า:</span><span class="sxs-lookup"><span data-stu-id="ae610-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="ae610-104">ผู้ใช้ที่กำหนดแดชบอร์ดเริ่มต้นของผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="ae610-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="ae610-105">โดยทั่วไปคุณสามารถระบุผู้ใช้ตั้งค่าแดชบอร์ดเริ่มต้นถ้าปุ่ม**ตั้งค่าเป็นค่าเริ่มต้น**ไม่แสดงในแถบคำสั่งแดชบอร์ดได้</span><span class="sxs-lookup"><span data-stu-id="ae610-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="ae610-106">แดชบอร์ดเริ่มต้นของผู้ใช้จะแทนทั้งหมดอื่น ๆ เริ่มต้นแดชบอร์ด แม้ว่าแดชบอร์ดเริ่มต้นของผู้ใช้ที่ไม่ได้อยู่ในโปรแกรมประยุกต์ปัจจุบัน</span><span class="sxs-lookup"><span data-stu-id="ae610-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="ae610-107">ใช้การแก้ปัญหาต่อไปนี้เมื่อต้องการยกเลิกการตั้งแดชบอร์ดเริ่มต้นของพวกเขา</span><span class="sxs-lookup"><span data-stu-id="ae610-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="ae610-108">สร้างแดชบอร์ดส่วนบุคคลใหม่</span><span class="sxs-lookup"><span data-stu-id="ae610-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="ae610-109">ตั้งค่าแดชบอร์ดใหม่ที่เป็นค่าเริ่มต้นผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="ae610-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="ae610-110">ลบแดชบอร์ดนั้น</span><span class="sxs-lookup"><span data-stu-id="ae610-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="ae610-111">แดชบอร์ดที่ถูกตั้งค่าในแบบแผนผังเว็บไซต์</span><span class="sxs-lookup"><span data-stu-id="ae610-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="ae610-112">คุณอาจกำหนดแดชบอร์ดเริ่มต้นขององค์กร โดยเลือกแดชบอร์ด และเลือก 'ตั้งเป็นค่าเริ่มต้น' ภายใต้ 'ระบบการแบบกำหนดเอง'</span><span class="sxs-lookup"><span data-stu-id="ae610-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="ae610-113">แต่แดชบอร์ดที่กำหนดเองในตัวออกแบบแผนผังเว็บไซต์จะเกิดขึ้นก่อนหน้านี้แดชบอร์ด ถ้าผู้ใช้เข้าถึง</span><span class="sxs-lookup"><span data-stu-id="ae610-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="ae610-114">เมื่อต้องการให้ผู้ใช้เห็นแดชบอร์ดที่คุณได้ตั้งค่าเป็นค่าเริ่มต้นขององค์กร คุณสามารถทำอย่างใดอย่างหนึ่ง:</span><span class="sxs-lookup"><span data-stu-id="ae610-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="ae610-115">ตั้งค่าแดชบอร์ดนั้นในแบบแผนผังเว็บไซต์</span><span class="sxs-lookup"><span data-stu-id="ae610-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="ae610-116">เอาการเข้าถึงไปยังแดชบอร์ดแผนผังเว็บไซต์ที่กำหนดไว้สำหรับผู้ใช้เหล่านั้น</span><span class="sxs-lookup"><span data-stu-id="ae610-116">Remove access to the sitemap defined dashboard for those users</span></span>
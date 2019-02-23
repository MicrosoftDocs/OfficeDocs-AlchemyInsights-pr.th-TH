---
title: 1385-สำนักงาน-365-เตือนนโยบาย
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: ''
ms.openlocfilehash: a0a1c749a120714c33cffd9fbdad08ea2cd6d62f
ms.sourcegitcommit: 983d08cd9ffe9542db75102b5b5c036d38eff67b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/14/2019
ms.locfileid: "30056843"
---
# <a name="office-365-alert-policies"></a><span data-ttu-id="92c3e-102">นโยบายการแจ้งเตือน office 365</span><span class="sxs-lookup"><span data-stu-id="92c3e-102">Office 365 Alert policies</span></span>

<span data-ttu-id="92c3e-p101">Office 365 ปลอดภัย & ศูนย์ปฏิบัติตามกฎระเบียบข้อเสนอ[เริ่มต้นนโยบายการแจ้งเตือน](https://docs.microsoft.com/office365/securitycompliance/alert-policies#default-alert-policies)ที่ทริกเกอร์ข้อความแจ้งเตือนสำหรับองค์กรที่มีการสมัครใช้งาน Office 365 องค์กร หรือ Office 365 เรารัฐบาล E1/G1, E3/G3 หรือ E5/G5 ดังนั้น ผู้ดูแลระบบอาจได้รับการแจ้งเตือนอีเมลการแจ้งเตือนที่ส่ง โดย Office365Alerts@microsoft.com กับบรรทัดชื่อเรื่องเช่น "การแจ้งเตือนต่ำความรุนแรง:*ชื่อของนโยบายการแจ้งเตือน*" ได้ การแจ้งเตือนจะส่งการแจ้งเตือนเมื่อข้อความแจ้งเตือนจะถูกทริกเกอร์สำหรับกิจกรรมทั่วไป เช่นเมื่อผู้ใช้:</span><span class="sxs-lookup"><span data-stu-id="92c3e-p101">The Office 365 Security & Compliance Center offers [default alert policies](https://docs.microsoft.com/office365/securitycompliance/alert-policies#default-alert-policies) that trigger alerts for organizations with an Office 365 Enterprise or Office 365 US Government E1/G1, E3/G3, or E5/G5 subscription. Therefore, admins may receive an alert email notification sent by Office365Alerts@microsoft.com with a subject line such as "A low-severity alert:*name of alert policy*". Alert notifications are sent when alerts are triggered for common activities, such as when users:</span></span>

- <span data-ttu-id="92c3e-106">สร้างกฎของกล่องขาเข้าที่ส่งต่ออีเมล</span><span class="sxs-lookup"><span data-stu-id="92c3e-106">Create inbox rules that forward email.</span></span>
- <span data-ttu-id="92c3e-107">กำหนดสิทธิ์ในกล่องจดหมายของพวกเขา</span><span class="sxs-lookup"><span data-stu-id="92c3e-107">Assign permissions their mailbox.</span></span>
- <span data-ttu-id="92c3e-108">ใช้ร่วมกัน หรือการลบแฟ้มใน SharePoint ใช้แฟ้มร่วมกันเป็นจำนวนมาก</span><span class="sxs-lookup"><span data-stu-id="92c3e-108">Sharing or deleting a large number of files in SharePoint file sharing.</span></span>
- <span data-ttu-id="92c3e-109">สร้างการค้นหา eDiscovery และส่งออกผลลัพธ์การค้นหา</span><span class="sxs-lookup"><span data-stu-id="92c3e-109">Create eDiscovery searches and export search results.</span></span>
 
<span data-ttu-id="92c3e-110">เมื่อต้องการตรวจทาน และดำเนินการกับข้อความแจ้งเตือน:</span><span class="sxs-lookup"><span data-stu-id="92c3e-110">To review and act on an alert:</span></span>

1. <span data-ttu-id="92c3e-111">ไปที่[ความปลอดภัย & ศูนย์ปฏิบัติตามกฎระเบียบ](https://protection.office.com)และเข้าสู่ระบบ</span><span class="sxs-lookup"><span data-stu-id="92c3e-111">Go to the [Security & Compliance Center](https://protection.office.com) and sign in.</span></span>
2. <span data-ttu-id="92c3e-112">คลิกที่**ข้อความแจ้งเตือน > ดูการแจ้งเตือน**</span><span class="sxs-lookup"><span data-stu-id="92c3e-112">Click **Alerts > View alerts**.</span></span>
3. <span data-ttu-id="92c3e-113">คลิกที่ข้อความแจ้งเตือนเพื่อแสดงหน้าเมนูลอยขึ้น ด้วยรายละเอียดเกี่ยวกับการแจ้งเตือน</span><span class="sxs-lookup"><span data-stu-id="92c3e-113">Click an alert to display a flyout page with information about the alert.</span></span>

<span data-ttu-id="92c3e-p102">คุณสามารถดำเนินการแจ้งเตือน เช่นการ[เอากฎกล่องขาเข้าที่น่าสงสัย](https://docs.microsoft.com/office365/securitycompliance/responding-to-a-compromised-email-account) หรือเพียงแต่คุณสามารถปิดการแจ้งเตือน โดยการคลิก**แก้ไข**บนหน้าเมนูลอยขึ้นแจ้งเตือน</span><span class="sxs-lookup"><span data-stu-id="92c3e-p102">You can take action on an alert, such as [removing a suspicious inbox rule](https://docs.microsoft.com/office365/securitycompliance/responding-to-a-compromised-email-account). Or you can simply close the alert by clicking **Resolve** on the alert flyout page.</span></span>

<span data-ttu-id="92c3e-116">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการตั้งค่าคอนฟิก และจัดการนโยบายการแจ้งเตือน ดู[บทความนี้](https://docs.microsoft.com/office365/securitycompliance/alert-policies)</span><span class="sxs-lookup"><span data-stu-id="92c3e-116">For more information about configuring and managing alert policies, see  [this article](https://docs.microsoft.com/office365/securitycompliance/alert-policies).</span></span>

<span data-ttu-id="92c3e-117">**สิ่งสำคัญ**: การแจ้งเตือนทางอีเมลการแจ้งเตือนจาก Microsoft จะไม่เคยขอให้คุณทำสิ่งต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="92c3e-117">**Important**: Alert email notifications from Microsoft will never ask you to do the following:</span></span>

- <span data-ttu-id="92c3e-118">ใส่รหัสผ่าน</span><span class="sxs-lookup"><span data-stu-id="92c3e-118">Provide a password.</span></span>
- <span data-ttu-id="92c3e-119">ตรวจสอบรายละเอียดความปลอดภัยของบัญชีของคุณ</span><span class="sxs-lookup"><span data-stu-id="92c3e-119">Verify the security details of your account.</span></span>
- <span data-ttu-id="92c3e-120">การรับรองความถูกต้องด้วยตัวคุณเอง</span><span class="sxs-lookup"><span data-stu-id="92c3e-120">Re-authenticate yourself.</span></span>

<span data-ttu-id="92c3e-p103">หากคุณได้รับข้อความอีเมลดังนี้ จะไม่ถูกส่ง โดย Microsoft และควรคำนึงถึงกลโกงของฟิชชิ่งจะเป็น ถ้าเกิดเหตุการณ์เช่น โปรด[รายงานปัญหาไปยัง Microsoft](https://docs.microsoft.com/office365/SecurityCompliance/report-junk-email-and-phishing-scams-in-outlook-on-the-web-eop)</span><span class="sxs-lookup"><span data-stu-id="92c3e-p103">If you receive an email message like this, it was not sent by Microsoft and should be considered a phishing scam. If that happens, please [report it to Microsoft](https://docs.microsoft.com/office365/SecurityCompliance/report-junk-email-and-phishing-scams-in-outlook-on-the-web-eop).</span></span>
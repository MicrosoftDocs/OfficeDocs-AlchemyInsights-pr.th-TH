---
title: การแก้ไขปัญหาการซิงโครไนส์ของรหัสผ่าน
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: c71fce8621057093d23891c26f7b0285fdc8b9ed
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/15/2019
ms.locfileid: "28316819"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="b584d-102">การแก้ไขปัญหาการซิงโครไนส์ของรหัสผ่าน</span><span class="sxs-lookup"><span data-stu-id="b584d-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="b584d-103">เมื่อต้องการแก้ไขปัญหาที่ไม่มีรหัสผ่านที่จะทำข้อมูลให้ตรงกับการเชื่อมต่อ AD Azure รุ่น 1.1.614.0 หรือรุ่นที่ใหม่กว่า:</span><span class="sxs-lookup"><span data-stu-id="b584d-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="b584d-104">เปิดเซสชัน Windows PowerShell ใหม่บนเซิร์ฟเวอร์ของคุณเชื่อมต่อ AD Azure ด้วยตัวเลือกที่**เรียกใช้ในฐานะผู้ดูแล**</span><span class="sxs-lookup"><span data-stu-id="b584d-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span> 
    
2. <span data-ttu-id="b584d-105">เรียกใช้**ชุด ExecutionPolicy RemoteSigned**หรือ**ExecutionPolicy ชุดที่ไม่จำกัด**</span><span class="sxs-lookup"><span data-stu-id="b584d-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span> 
    
3. <span data-ttu-id="b584d-106">เริ่มตัวช่วยสร้างการเชื่อมต่อ AD Azure</span><span class="sxs-lookup"><span data-stu-id="b584d-106">Start the Azure AD Connect wizard.</span></span>
    
4. <span data-ttu-id="b584d-107">นำทางไปยัง \*\* งานเพิ่มเติม \*\* หน้า เลือก \*\* แก้ไข **, และคลิก**ถัดไป\*\*</span><span class="sxs-lookup"><span data-stu-id="b584d-107">Navigate to the \*\* Additional Tasks \*\* page, select \*\* Troubleshoot \*\*, and click **Next**.</span></span> 
    
5. <span data-ttu-id="b584d-108">บนหน้าการแก้ไขปัญหาเบื้องต้น คลิก**เปิดใช้เพื่อเริ่มต้นการแก้ไขปัญหา**เมนูใน PowerShell</span><span class="sxs-lookup"><span data-stu-id="b584d-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span> 
    
6. <span data-ttu-id="b584d-109">ในเมนูหลัก เลือก**การแก้ปัญหาการซิงโครไนส์ของรหัสผ่าน**</span><span class="sxs-lookup"><span data-stu-id="b584d-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span> 
    
7. <span data-ttu-id="b584d-110">ในเมนูย่อย เลือก**ซิงโครไนส์รหัสผ่านไม่ทำงานเลย**</span><span class="sxs-lookup"><span data-stu-id="b584d-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span> 
    
 <span data-ttu-id="b584d-111">**การทำความเข้าใจเกี่ยวกับผลลัพธ์ของการแก้ไขปัญหางาน**</span><span class="sxs-lookup"><span data-stu-id="b584d-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="b584d-112">งานการแก้ไขปัญหาเบื้องต้นทำการตรวจสอบต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="b584d-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="b584d-113">ตรวจสอบว่า เปิดใช้งานคุณลักษณะการซิงโครไนส์รหัสผ่านสำหรับผู้เช่าโฆษณา Azure ของคุณ</span><span class="sxs-lookup"><span data-stu-id="b584d-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>
    
- <span data-ttu-id="b584d-114">ตรวจสอบว่า เซิร์ฟเวอร์การเชื่อมต่อ AD Azure ไม่ได้อยู่ในโหมดการจัดเตรียม</span><span class="sxs-lookup"><span data-stu-id="b584d-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>
    
- <span data-ttu-id="b584d-115">สำหรับแต่ละที่มีอยู่ในสถานที่ Active Directory ตัวเชื่อมต่อ (ซึ่งสอดคล้องกับการฟอเรสต์ Active Directory ที่มีอยู่แล้ว):</span><span class="sxs-lookup"><span data-stu-id="b584d-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>
    
- 
  - <span data-ttu-id="b584d-116">ตรวจสอบว่า คุณลักษณะการซิงโครไนส์รหัสผ่านถูกเปิดใช้งาน</span><span class="sxs-lookup"><span data-stu-id="b584d-116">Validates that the password synchronization feature is enabled.</span></span>
    
  - <span data-ttu-id="b584d-117">การค้นหาสำหรับเหตุการณ์แบบฮาร์ทบีซิงโครไนส์ของรหัสผ่านในล็อกเหตุการณ์ของแอพลิเคชัน Windows</span><span class="sxs-lookup"><span data-stu-id="b584d-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>
    
  - <span data-ttu-id="b584d-118">สำหรับแต่ละโดเมน Active Directory ภายใต้ตัวเชื่อมต่อไดเรกทอรีที่ใช้งานอยู่ในสถานที่:</span><span class="sxs-lookup"><span data-stu-id="b584d-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>
    
  - <span data-ttu-id="b584d-119">ตรวจสอบว่าโดเมนสามารถเข้าถึงได้จากเซิร์ฟเวอร์เชื่อมต่อ AD Azure</span><span class="sxs-lookup"><span data-stu-id="b584d-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>
    
  - <span data-ttu-id="b584d-120">ตรวจสอบว่า บัญชีบริการระบบโดเมนไดเรกทอรีที่ใช้งานอยู่ (AD DS) ที่ใช้ โดยตัวเชื่อมต่อไดเรกทอรีที่ใช้งานอยู่ในสถานที่ที่มีชื่อผู้ใช้ที่ถูกต้อง รหัสผ่าน และสิทธิ์ที่จำเป็นสำหรับการซิงโครไนส์รหัสผ่าน</span><span class="sxs-lookup"><span data-stu-id="b584d-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>
    
<span data-ttu-id="b584d-121">สำหรับวิธีใช้เพิ่มเติมการแก้ไขปัญหาการซิงค์รหัสผ่าน ดู[การซิงโครไนส์รหัสผ่านแก้ไขปัญหากับการเชื่อมต่อ AD Azure ซิงค์](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization)</span><span class="sxs-lookup"><span data-stu-id="b584d-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  

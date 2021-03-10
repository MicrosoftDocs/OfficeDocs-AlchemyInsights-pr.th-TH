---
title: การเตรียมใช้งานผู้ใช้
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
- "9004348"
- "8428"
ms.openlocfilehash: bd415b2d44bccf0c2b3eccb4e38452498b748b3a
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482913"
---
# <a name="user-provisioning"></a><span data-ttu-id="040b7-102">การเตรียมใช้งานผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="040b7-102">User provisioning</span></span>

- <span data-ttu-id="040b7-103">ใช้ [ความสามารถในการเตรียมใช้งานตามความต้องการ](https://docs.microsoft.com/azure/active-directory/app-provisioning/provision-on-demand) ในการเตรียมใช้งานผู้ใช้และรับการวินิจฉัยโดยละเอียดเกี่ยวกับขั้นตอนที่ใช้</span><span class="sxs-lookup"><span data-stu-id="040b7-103">Use the [on-demand provisioning](https://docs.microsoft.com/azure/active-directory/app-provisioning/provision-on-demand) capability to provision a user and get detailed diagnostics about the steps taken.</span></span>
- <span data-ttu-id="040b7-104">เมื่อต้องการแก้ไขปัญหาที่คุณพบเมื่อเตรียมใช้งานผู้ใช้และกลุ่ม ให้ดูคู่มือการแก้ไขปัญหา [ไม่มีการเตรียมใช้งาน](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned)ผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="040b7-104">To troubleshoot issues you encounter when provisioning users and groups, see the troubleshooting guide [No users are being provisioned](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned).</span></span>
- <span data-ttu-id="040b7-105">ถ้าคุณสังเกตเห็นว่าผู้ใช้จะไม่ถูกเตรียมใช้งาน ดูแฟ้มบันทึก [การเตรียมใช้งาน (ตัวอย่าง)](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs) ใน Azure Active Directory (AD)</span><span class="sxs-lookup"><span data-stu-id="040b7-105">If you observe that users are not being provisioned, see [Provisioning logs (preview)](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs) in Azure Active Directory (AD).</span></span> <span data-ttu-id="040b7-106">ค้นหารายการบันทึกที่เกี่ยวข้องกับผู้ใช้ที่ระบุ</span><span class="sxs-lookup"><span data-stu-id="040b7-106">Search for log entries pertaining to a specific user.</span></span>
- <span data-ttu-id="040b7-107">รีสตาร์ตการเตรียมใช้งานเป็นระยะๆ เพื่อติดตามผู้ใช้ที่ไม่ได้รับในรอบการเตรียมใช้งานก่อนหน้านี้</span><span class="sxs-lookup"><span data-stu-id="040b7-107">Periodically restart provisioning to catch any users that were missed in a previous provisioning cycle.</span></span>
- <span data-ttu-id="040b7-108">ผู้ใช้/กลุ่มอาจยังไม่ได้เตรียมใช้งานเนื่องจากบริการของเรายังไม่มีโอกาสที่จะประเมินผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="040b7-108">The user/group may not have been provisioned because our service hasn't had a chance to evaluate the user yet.</span></span> <span data-ttu-id="040b7-109">ตรวจทานแนวทางสําหรับระยะเวลาการเตรียมใช้งานรวมถึงแถบความคืบหน้าบนหน้าการกําหนดค่าการเตรียมใช้งาน</span><span class="sxs-lookup"><span data-stu-id="040b7-109">Review the guidance for how long provisioning takes as well as the progress bar on the provisioning configuration page.</span></span> <span data-ttu-id="040b7-110">ถ้าสถานะคงที่ที่ระบุไว้ในส่วนรายละเอียดเพิ่มเติมอยู่ก่อนวันที่ผู้ใช้ถูกสร้าง/อัปเดต/ลบ หมายความว่าเรายังไม่ได้ประเมินผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="040b7-110">If the steady state specified in the additional details section is before the date the user was created/updated/deleted, it means we have not evaluated the user yet.</span></span> <span data-ttu-id="040b7-111">ในสถานการณ์นี้ วิธีที่ดีที่สุดคือการรอให้บริการการเตรียมใช้งานเสร็จสิ้น</span><span class="sxs-lookup"><span data-stu-id="040b7-111">In this scenario, the best thing to do is wait for the provisioning service to finish.</span></span> <span data-ttu-id="040b7-112">ถ้าสถานะคงที่สมาสได้เราขอแนะนนะให้เริ่มการรีสตาร์ตจาก UI ในพอร์ทัล Azure</span><span class="sxs-lookup"><span data-stu-id="040b7-112">If the steady state has been achieved, we recommend performing a restart from the UI in the Azure Portal.</span></span>
  - <span data-ttu-id="040b7-113">โปรดทราบว่าบริการของเรารับทราบเฉพาะการเปลี่ยนแปลงของผู้ใช้/กลุ่มในระบบต้นทาง (Azure Active Directory) เท่านั้น</span><span class="sxs-lookup"><span data-stu-id="040b7-113">Note that our service is only aware of changes to a user/group in the source system (Azure Active Directory).</span></span> <span data-ttu-id="040b7-114">ถ้าผู้ใช้/กลุ่มถูกเอาออกโดยตรงในแอปพลิเคชัน (ตัวอย่างเช่น ServiceNow) เราไม่ทราบถึงการเปลี่ยนแปลงเหล่านั้นและจะไม่ย้อนกลับโดยยึดตามสถานะของผู้ใช้ในระบบต้นทาง</span><span class="sxs-lookup"><span data-stu-id="040b7-114">If a user/group is removed directly in the application (for example, ServiceNow), we are not aware of those changes and do not roll it back based on the state of the user in the source system.</span></span> <span data-ttu-id="040b7-115">ในสถานการณ์นี้ การย้อนกลับการเปลี่ยนแปลงโดยตรงในแอปพลิเคชันเป้าหมายจะดีที่สุด</span><span class="sxs-lookup"><span data-stu-id="040b7-115">In this scenario, it is best to roll back the change directly in the target application.</span></span>
- <span data-ttu-id="040b7-116">บริการของเราประเมินผู้ใช้/กลุ่ม และกําหนดว่าไม่ควรเตรียมใช้งาน:</span><span class="sxs-lookup"><span data-stu-id="040b7-116">Our service evaluated the user/group and determined it should not be provisioned:</span></span>
  - <span data-ttu-id="040b7-117">ถ้าคุณตั้งค่าขอบเขตให้กับผู้ใช้และกลุ่มที่มอบหมาย ให้ตรวจสอบว่าผู้ใช้/กลุ่มถูกมอบหมายให้กับแอปพลิเคชันหรือไม่</span><span class="sxs-lookup"><span data-stu-id="040b7-117">If you have set the scope to assigned users and groups, check if the user/group is assigned to the application.</span></span>
  - <span data-ttu-id="040b7-118">ถ้าผู้ใช้/กลุ่มถูกมอบหมายให้กับแอปพลิเคชัน ตรวจสอบให้แน่ใจว่าไม่ได้มอบหมายให้กับบทบาทการเข้าถึงเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="040b7-118">If the user/group is assigned to the application, ensure that they are not assigned to the default access role.</span></span> <span data-ttu-id="040b7-119">บทบาทนี้ไม่สามารถใช้เพื่อเตรียมใช้งานได้</span><span class="sxs-lookup"><span data-stu-id="040b7-119">This role cannot be used for provisioning.</span></span>
  - <span data-ttu-id="040b7-120">ถ้าคุณได้ตั้งค่าตัวกรองการซ้อนทับแอตทริบิวต์ โปรดตรวจสอบให้แน่ใจว่าผู้ใช้ตรงตามเกณฑ์ที่คุณระบุ</span><span class="sxs-lookup"><span data-stu-id="040b7-120">If you have set an attribute based scoping filter, ensure that the user meets the criteria that you have specified.</span></span>
  - <span data-ttu-id="040b7-121">If users already exist in the target system and the state of the user in the source and target match, we won't take any further action.</span><span class="sxs-lookup"><span data-stu-id="040b7-121">If users already exist in the target system and the state of the user in the source and target match, we won't take any further action.</span></span>
- <span data-ttu-id="040b7-122">บริการของเราพยายามเตรียมใช้งานผู้ใช้แต่ล้มเหลว</span><span class="sxs-lookup"><span data-stu-id="040b7-122">Our service attempted to provision the user and it failed.</span></span> <span data-ttu-id="040b7-123">ดูสถานการณ์สมมติเหล่านี้ ที่แท็บการแก้ไขปัญหาและข้อเสนอแนะของบันทึกการเตรียมใช้งาน:</span><span class="sxs-lookup"><span data-stu-id="040b7-123">For these scenarios, review the troubleshooting and recommendations tab of the provisioning logs:</span></span>
  - <span data-ttu-id="040b7-124">แอตทริบิวต์ที่ต้องมีกับผู้ใช้อาจหายไปใน Azure Active Directory หรือไม่ตรงกับรูปแบบที่แอปพลิเคชันของบริษัทอื่นต้องการ</span><span class="sxs-lookup"><span data-stu-id="040b7-124">A required attribute on the user might be missing in Azure Active Directory or does not match the format required by the third party application.</span></span> <span data-ttu-id="040b7-125">For example, the Country attribute on a user might be set to United States when it should be US.</span><span class="sxs-lookup"><span data-stu-id="040b7-125">For example, the Country attribute on a user might be set to United States when it should be US.</span></span>
  - <span data-ttu-id="040b7-126">แอตทริบิวต์เป็นแอตทริบิวต์ที่อ้างอิงที่ยังไม่มีอยู่ในแอปพลิเคชันเป้าหมาย</span><span class="sxs-lookup"><span data-stu-id="040b7-126">The attribute is a referential attribute that does not yet exist in the target application.</span></span> <span data-ttu-id="040b7-127">แอตทริบิวต์การอ้างอิงเป็นแอตทริบิวต์ที่ชี้ไปยังวัตถุอื่น ตัวอย่างเช่น ผู้ใช้ที่เป็นสมาชิกของกลุ่ม</span><span class="sxs-lookup"><span data-stu-id="040b7-127">A referential attribute is an attribute that points to another object, for example, a user that is a member of a group.</span></span> <span data-ttu-id="040b7-128">ID ของผู้ใช้จะอยู่ในแอตทริบิวต์สมาชิกของกลุ่ม แต่จะสามารถประมวลผลได้ถ้าวัตถุของผู้ใช้ชี้ไปที่มีอยู่แล้วเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="040b7-128">The user's ID would be in the member attribute of the group, but can only be processed if the user object it points to already exists.</span></span>
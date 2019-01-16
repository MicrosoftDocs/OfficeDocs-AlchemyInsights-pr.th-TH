---
title: ใช้เครื่องมือการปรับใช้ Office
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: b4ade0f21794a8986aa7a37d783da5fa289488fc
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/15/2019
ms.locfileid: "28316841"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="9347b-102">ใช้เครื่องมือการปรับใช้ Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="9347b-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="9347b-p101">คุณสามารถใช้เครื่องมือการปรับใช้ Office (ODT) เพื่อปรับใช้ Office รุ่น Office 365 เครื่องมือการปรับใช้ Office (setup.exe) ถูกเรียกใช้จากบรรทัดคำสั่ง และใช้แฟ้ม XML การกำหนดค่าการตั้งค่าใดที่จะนำไปใช้เมื่อปรับใช้ Office</span><span class="sxs-lookup"><span data-stu-id="9347b-p101">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office. The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="9347b-105">ดาวน์โหลดเครื่องมือการปรับใช้ Office รุ่นล่าสุดจาก[ศูนย์ดาวน์โหลดของไมโครซอฟท์](http://go.microsoft.com/fwlink/p/?LinkID=626065)</span><span class="sxs-lookup"><span data-stu-id="9347b-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
    
2. <span data-ttu-id="9347b-p102">ใช้เครื่อง[มือกำหนดเอง Office (OCT)](https://config.office.com)เพื่อเลือกการกำหนดลักษณะของคุณปรับใช้ และสร้างแฟ้ม XML การกำหนดค่า แฟ้มการกำหนดค่าการส่งออก และวางไว้ในโฟลเดอร์เดียวกับที่ setup.exe ที่ตั้งอยู่ภายในเครื่อง</span><span class="sxs-lookup"><span data-stu-id="9347b-p102">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file. Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span> 
    
    <span data-ttu-id="9347b-p103">**หมายเหตุ:** การติดตั้ง office ออกใช้โดยทั่วไปเกิดขึ้นครบกำหนดเพื่อ misconfigured หรือ malformatted แฟ้มการตั้งค่าคอนฟิก เมื่อต้องการหลีกเลี่ยงปัญหาดังกล่าว เราขอแนะนำให้ คุณใช้เครื่องมือกำหนดเองของ Office เมื่อต้องการสร้างแฟ้มการกำหนดค่า คุณยังสามารถนำเข้าแฟ้มการกำหนดค่าที่มีอยู่ลงในเครื่องมือกำหนดเองของ Office</span><span class="sxs-lookup"><span data-stu-id="9347b-p103">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files. To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file. You can also import existing configuration files into the Office Customization Tool.</span></span> 
    
3. <span data-ttu-id="9347b-p104">จากพร้อมท์คำสั่ง สลับไปยังตำแหน่งที่ตั้งที่ setup.exe และเรียกใช้เครื่องมือการปรับใช้ Office ในโหมดดาวน์โหลด และระบุแฟ้มการกำหนดค่าที่คุณเพิ่งบันทึก ในตัวอย่างนี้ แฟ้มการกำหนดค่าถูกตั้งชื่อว่า Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="9347b-p104">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved. In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="9347b-113">เรียกใช้เครื่องมือการปรับใช้ Office ในโหมดที่ตั้งค่าคอนฟิก และระบุแฟ้มการกำหนดค่า</span><span class="sxs-lookup"><span data-stu-id="9347b-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="9347b-114">**หมายเหตุ:** คุณต้องเรียกใช้ขั้นตอนนี้จากคอมพิวเตอร์ไคลเอนต์ที่คุณต้องการติดตั้ง Office และคุณต้องมีสิทธิ์เป็นผู้ดูแลท้องถิ่นบนคอมพิวเตอร์เครื่องนั้น</span><span class="sxs-lookup"><span data-stu-id="9347b-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span> 
    
<span data-ttu-id="9347b-p105">เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับการใช้เครื่องมือการปรับใช้ Office สำหรับสถานการณ์การปรับใช้ Office 365 ProPlus ของคุณ ดู[ภาพรวมของเครื่องมือการปรับใช้ Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool) สำหรับรายละเอียดเพิ่มเติมเกี่ยวกับวิธีการใช้เครื่องมือกำหนดเอง Office ดู[ภาพรวมของเครื่องมือการกำหนดเองของ Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)</span><span class="sxs-lookup"><span data-stu-id="9347b-p105">To learn more about using Office Deployment Tool for your Office 365 ProPlus deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
  

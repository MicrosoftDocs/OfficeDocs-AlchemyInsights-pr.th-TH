---
title: การคืนค่าโฟลเดอร์สาธารณะที่ถูกลบ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: cd85dd3c0eb14f6e02ac4f912e733468403387aa
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158546"
---
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="a1c83-102">การคืนค่าโฟลเดอร์สาธารณะที่ถูกลบ</span><span class="sxs-lookup"><span data-stu-id="a1c83-102">Restore a deleted public folder</span></span>

<span data-ttu-id="a1c83-103">**เมื่อต้องการคืนค่ารายการที่ถูกลบจากโฟลเดอร์สาธารณะ**:</span><span class="sxs-lookup"><span data-stu-id="a1c83-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="a1c83-104">ดู[คุณไม่สามารถกู้คืนรายการที่ถูกลบจากโฟลเดอร์สาธารณะที่ไม่ใช่จดหมายใน Outlook ๒๐๑๖](https://aka.ms/pfrec)</span><span class="sxs-lookup"><span data-stu-id="a1c83-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="a1c83-105">**เมื่อต้องการคืนค่าโฟลเดอร์สาธารณะที่ถูกลบ (ชนิดใดก็ได้)**:</span><span class="sxs-lookup"><span data-stu-id="a1c83-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="a1c83-106">โปรดใช้คำสั่ง EXO PowerShell ต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="a1c83-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="a1c83-107">ไวยากรณ์:</span><span class="sxs-lookup"><span data-stu-id="a1c83-107">Syntax:</span></span>

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    <span data-ttu-id="a1c83-108">ตัวอย่าง: คำสั่งต่อไปนี้จะคืนค่า Subfolder1 และวางภายใต้ \Parent1:</span><span class="sxs-lookup"><span data-stu-id="a1c83-108">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

<span data-ttu-id="a1c83-109">ดู[ที่การคืนค่าโฟลเดอร์สาธารณะที่ถูกลบ](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder)สำหรับรายละเอียดเพิ่มเติม</span><span class="sxs-lookup"><span data-stu-id="a1c83-109">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>

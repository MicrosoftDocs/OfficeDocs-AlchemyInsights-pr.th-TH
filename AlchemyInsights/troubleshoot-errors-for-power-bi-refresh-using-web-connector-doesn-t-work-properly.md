---
Title: ฟื้นฟูผ่านตัวเชื่อมต่อไม่ทำงานอย่างถูกต้อง
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1316"
- "2500002"
ms.openlocfilehash: e6c0f44f8f62b01e7f4dd23776ba8c13a2999c6b
ms.sourcegitcommit: e17e7d17fdb638349bb320b318085138d18f284c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/16/2019
ms.locfileid: "35753329"
---
# <a name="refresh-using-web-connector-doesnt-work-properly"></a><span data-ttu-id="1609f-102">ฟื้นฟูผ่านตัวเชื่อมต่อไม่ทำงานอย่างถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="1609f-102">Refresh using Web connector doesn't work properly</span></span>

<span data-ttu-id="1609f-103">ถ้าคุณมีตัวเชื่อมต่อเว็บสคริปต์ที่ใช้ฟังก์ชัน[Web.Page](https://msdn.microsoft.com/library/mt260924.aspx)และคุณได้ปรับปรุงชุดข้อมูลหรือรายงานของคุณหลังจาก 18th พฤศจิกายน 2016 คุณจำเป็นต้องใช้เกตเวย์ในใบสั่งสำหรับการฟื้นฟูให้ทำงานได้อย่างถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="1609f-103">If you have a web connector script that's using the [Web.Page](https://msdn.microsoft.com/library/mt260924.aspx) function, and you have updated your dataset or report after November 18th, 2016, you need to use a gateway in order for refresh to work properly.</span></span>

<span data-ttu-id="1609f-104">สำหรับข้อมูลเพิ่มเติม:[https://docs.microsoft.com/power-bi/refresh-troubleshooting-refresh-scenarios](https://docs.microsoft.com/power-bi/refresh-troubleshooting-refresh-scenarios)</span><span class="sxs-lookup"><span data-stu-id="1609f-104">For more information: [https://docs.microsoft.com/power-bi/refresh-troubleshooting-refresh-scenarios](https://docs.microsoft.com/power-bi/refresh-troubleshooting-refresh-scenarios)</span></span>
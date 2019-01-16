---
title: กฎ DLP สำหรับเราหมายเลขบัญชีธนาคารไม่ทำงาน
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 6eae9146d33f5fc307085dbf931d57bdbb28b82e
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/15/2019
ms.locfileid: "28317241"
---
<span data-ttu-id="45bd6-p101">คุณกำลังมีปัญหากับ**การป้องกันการสูญเสียข้อมูล (DLP)** ไม่ทำงานสำหรับเนื้อหาที่ประกอบด้วยหมาย**เลขบัญชีธนาคารของสหรัฐอเมริกา**เมื่อใช้ชนิดข้อมูลที่เป็นความลับ DLP ใน O365 หรือไม่ ถ้าเป็นเช่นนั้น ทำให้แน่ใจว่าเนื้อหาของคุณประกอบด้วยข้อมูลที่จำเป็นสำหรับสิ่งนโยบาย DLP จะค้นหาเมื่อถูกประเมิน</span><span class="sxs-lookup"><span data-stu-id="45bd6-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span> 
  
<span data-ttu-id="45bd6-104">ตัวอย่างเช่น**หมายเลขบัญชีธนาคารของสหรัฐอเมริกา**โยบายการกำหนดค่า ด้วยระดับความเชื่อมั่นของ 85% ต่อไปนี้จะถูกประเมิน และต้องถูกตรวจพบกฎเพื่อทริกเกอร์:</span><span class="sxs-lookup"><span data-stu-id="45bd6-104">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span> 
  
- <span data-ttu-id="45bd6-105">**[รูปแบบ:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** ตัวเลข 8-17</span><span class="sxs-lookup"><span data-stu-id="45bd6-105">**[Format:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span> 
    
- <span data-ttu-id="45bd6-106">**[รูปแบบ:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8 17 ตัวเลขที่ต่อเนื่องกัน</span><span class="sxs-lookup"><span data-stu-id="45bd6-106">**[Pattern:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span> 
    
- <span data-ttu-id="45bd6-107">**[Checksum:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** ไม่มี ไม่มี Checksum ไม่มี</span><span class="sxs-lookup"><span data-stu-id="45bd6-107">**[Checksum:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="45bd6-108">**[คำนิยาม:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)** นโยบาย DLP คือ 75% มั่นใจจะได้ตรวจพบชนิดข้อมูลที่เป็นความลับนี้ if ภายในมีความใกล้เคียง 300 อักขระ:</span><span class="sxs-lookup"><span data-stu-id="45bd6-108">**[Definition:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="45bd6-109">นิพจน์ทั่วไป Regex_usa_bank_account_number ค้นหาเนื้อหาที่ตรงกับรูปแบบ</span><span class="sxs-lookup"><span data-stu-id="45bd6-109">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>
    
  - <span data-ttu-id="45bd6-110">พบคำสำคัญจาก Keyword_usa_Bank_Account</span><span class="sxs-lookup"><span data-stu-id="45bd6-110">A keyword from Keyword_usa_Bank_Account is found.</span></span>
    
    <span data-ttu-id="45bd6-111">ตัวอย่างเช่น ตัวอย่างต่อไปนี้จะทริกเกอร์สำหรับ**หมายเลขบัญชีธนาคารของสหรัฐอเมริกา**นโยบาย: 78344011 บัญชีกระแสรายวัน</span><span class="sxs-lookup"><span data-stu-id="45bd6-111">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span> 
    
<span data-ttu-id="45bd6-112">สำหรับข้อมูลเพิ่มเติมบนสิ่งจำเป็นสำหรับ**หมายเลขบัญชีธนาคารของสหรัฐอเมริกา**เพื่อพบกับเนื้อหาของคุณ ให้ดูส่วนต่อไปนี้ในบทความนี้:[สิ่งสำคัญชนิดข้อมูลค้นหาหมายเลขบัญชีธนาคารของสหรัฐอเมริกา](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="45bd6-112">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="45bd6-113">โดยใช้ชนิดข้อมูลที่สำคัญในตัวแตกต่างกัน ดูบทความต่อไปนี้สำหรับข้อมูลเกี่ยวกับสิ่งจำเป็นสำหรับชนิดอื่น ๆ:[สิ่งสำคัญชนิดข้อมูลค้นหา](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="45bd6-113">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

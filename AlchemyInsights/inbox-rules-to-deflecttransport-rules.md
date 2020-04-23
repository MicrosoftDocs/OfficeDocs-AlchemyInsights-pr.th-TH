---
title: กฎกล่องขาเข้า 929 เพื่อ deflect กฎการขนส่ง
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "929"
- "1800021"
ms.assetid: 9733ef4e-db8d-4345-a072-c251480875a1
ms.openlocfilehash: 6b6e64c0332a579e8f6132b08f2f89b15eb4de27
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43724611"
---
# <a name="mail-flow-rules-also-known-as-transport-rules"></a><span data-ttu-id="d9f5d-102">กฎขั้นตอนจดหมาย (หรือที่เรียกว่ากฎการส่งผ่าน)</span><span class="sxs-lookup"><span data-stu-id="d9f5d-102">Mail flow rules (also known as transport rules)</span></span>

- <span data-ttu-id="d9f5d-103">ภาพรวมทั่วไปของกฎขั้นตอนจดหมาย:[กฎการไหลของจดหมาย (กฎการขนส่ง) ในการแลกเปลี่ยนแบบออนไลน์](https://technet.microsoft.com/library/jj919238.aspx)</span><span class="sxs-lookup"><span data-stu-id="d9f5d-103">General overview of mail flow rules: [Mail flow rules (transport rules) in Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)</span></span>

- <span data-ttu-id="d9f5d-104">ตั้งค่ากฎขั้นตอนของขั้นตอนจดหมาย:[ขั้นตอนกฎขั้นตอนของกระแสจดหมายในการแลกเปลี่ยนแบบออนไลน์](https://technet.microsoft.com/library/dn600436.aspx)</span><span class="sxs-lookup"><span data-stu-id="d9f5d-104">Setup mail flow rules: [Mail flow rule procedures in Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)</span></span>

- <span data-ttu-id="d9f5d-105">สร้าง แก้ไข และลบกฎขั้นตอนจดหมาย:[จัดการกฎขั้นตอนจดหมาย](https://technet.microsoft.com/library/jj657505.aspx)</span><span class="sxs-lookup"><span data-stu-id="d9f5d-105">Create, modify, and delete mail flow rules: [Manage mail flow rules](https://technet.microsoft.com/library/jj657505.aspx)</span></span>

<span data-ttu-id="d9f5d-106">คุณยังสามารถจัดการกฎกระแสจดหมายใน PowerShell แบบออนไลน์ของอัตราแลกเปลี่ยน</span><span class="sxs-lookup"><span data-stu-id="d9f5d-106">You can also manage mail flow rules in Exchange Online PowerShell.</span></span> <span data-ttu-id="d9f5d-107">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[กฎการรับส่ง](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule)(มุมมอง),[กฎการขนส่งใหม่](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule)(สร้าง[),](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) [Set-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) [Disable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) [Enable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule)</span><span class="sxs-lookup"><span data-stu-id="d9f5d-107">For more information, see [Get-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (view), [New-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (create), [Remove-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (delete), [Set-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (modify existing), [Disable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (disable existing), and [Enable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (enable existing).</span></span>

<span data-ttu-id="d9f5d-108">cmdlet กฎกระแสจดหมายเพิ่มเติม:[รับ-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (รายการการดําเนินการพร้อมใช้งาน),[รับ-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (เงื่อนไขที่มีอยู่รายการและข้อยกเว้น),[ส่งออก-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (กฎการส่งออก), และ[การนําเข้า-กฎการขนส่ง](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection)(กฎการนําเข้า)</span><span class="sxs-lookup"><span data-stu-id="d9f5d-108">Additional mail flow rule cmdlets: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (list available actions), [Get-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (list available conditions and exceptions), [Export-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (export rules), and [Import-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (import rules).</span></span>

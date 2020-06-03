---
title: Opération UpdateItem (tâche)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateItem
api_type:
- schema
ms.assetid: b0a7f114-d040-40eb-a8f3-05ea6489e472
description: L’opération UpdateItem est utilisée pour mettre à jour les propriétés d’élément de tâche dans la Banque d’Exchange.
ms.openlocfilehash: 0041af114d11fd9577037dd154e40b84e8483c35
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459804"
---
# <a name="updateitem-operation-task"></a><span data-ttu-id="7d083-103">Opération UpdateItem (tâche)</span><span class="sxs-lookup"><span data-stu-id="7d083-103">UpdateItem operation (task)</span></span>

<span data-ttu-id="7d083-104">L’opération UpdateItem est utilisée pour mettre à jour les propriétés d’élément de tâche dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="7d083-104">The UpdateItem operation is used to update task item properties in the Exchange store.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7d083-105">Remarques</span><span class="sxs-lookup"><span data-stu-id="7d083-105">Remarks</span></span>

<span data-ttu-id="7d083-106">Vous ne pouvez pas utiliser les services Web Exchange pour envoyer des demandes de tâches.</span><span class="sxs-lookup"><span data-stu-id="7d083-106">You cannot use Exchange Web Services to send task requests.</span></span> <span data-ttu-id="7d083-107">Les services Web Exchange peuvent renvoyer des demandes de tâche créées par MicrosoftOfficeOutlook.</span><span class="sxs-lookup"><span data-stu-id="7d083-107">Exchange Web Services can return task requests that are created by MicrosoftOfficeOutlook.</span></span> <span data-ttu-id="7d083-108">Si une demande de tâche a déjà été envoyée, une demande de mise à jour de la tâche renverra une erreur.</span><span class="sxs-lookup"><span data-stu-id="7d083-108">If a task request has already been sent, a request to update the task will return an error.</span></span>
  
## <a name="updating-the-current-occurrence-of-a-recurring-task"></a><span data-ttu-id="7d083-109">Mise à jour de l’occurrence actuelle d’une tâche périodique</span><span class="sxs-lookup"><span data-stu-id="7d083-109">Updating the Current Occurrence of a Recurring Task</span></span>

<span data-ttu-id="7d083-110">Le résultat d’une opération UpdateItem sur les tâches récurrentes diffère du résultat de l’opération UpdateItem sur une tâche unique, non périodique.</span><span class="sxs-lookup"><span data-stu-id="7d083-110">The result of an UpdateItem operation on recurring tasks differs from the result of the UpdateItem operation on a single, nonrecurring task.</span></span> <span data-ttu-id="7d083-111">Les modifications apportées à une occurrence d’une tâche périodique entraînent la génération de tâches ponctuelles lorsque les mises à jour suivantes sont effectuées :</span><span class="sxs-lookup"><span data-stu-id="7d083-111">Changes to an occurrence of a recurring task cause one-off tasks to be generated when the following updates are made:</span></span>
  
1. <span data-ttu-id="7d083-112">La propriété Status d’une tâche récurrente de régénération ou nonregenerating est définie sur **terminé**.</span><span class="sxs-lookup"><span data-stu-id="7d083-112">The status property of a regenerating or nonregenerating recurrent task is set to **Completed**.</span></span>
    
2. <span data-ttu-id="7d083-113">La date de début ou la date de fin d’une tâche récurrente nonregenerating est modifiée.</span><span class="sxs-lookup"><span data-stu-id="7d083-113">The start date or end date of a nonregenerating recurrent task is changed.</span></span>
    
<span data-ttu-id="7d083-114">Par exemple, si une requête **UpdateItem** définit la valeur achevée d’une tâche périodique sur **true**, le **UpdateItemResponse** inclut un nouvel ID et ChangeKey qui représentent une nouvelle tâche ponctuelle.</span><span class="sxs-lookup"><span data-stu-id="7d083-114">For example, if an **UpdateItem** request sets the Completed value of a recurring task to **true**, the **UpdateItemResponse** will include a new Id and ChangeKey that represent a newly created one-off task.</span></span> <span data-ttu-id="7d083-115">L’ID qui a été inclus dans la demande est toujours valide et la tâche périodique représentée par cet ID a été mise à jour pour représenter l’occurrence suivante.</span><span class="sxs-lookup"><span data-stu-id="7d083-115">The Id that was included in the request is still valid and the recurring task that is represented by that Id has been updated to represent the next occurrence.</span></span> <span data-ttu-id="7d083-116">Le ChangeKey qui a été inclus dans la demande n’est plus valide car la tâche périodique a été mise à jour.</span><span class="sxs-lookup"><span data-stu-id="7d083-116">The ChangeKey that was included in the request is no longer valid because the recurring task has been updated.</span></span> 
  
<span data-ttu-id="7d083-117">Vous pouvez utiliser l' [opération GetItem](getitem-operation.md) pour obtenir la dernière **ChangeKey** de la tâche périodique.</span><span class="sxs-lookup"><span data-stu-id="7d083-117">You can use the [GetItem operation](getitem-operation.md) to get the latest **ChangeKey** for the recurring task.</span></span> 
  
<span data-ttu-id="7d083-118">Pour les tâches non périodiques ou pour la dernière occurrence d’une tâche périodique, la réponse UpdateItem renvoie le même **ID** qui lui a été passé et renvoie la **ChangeKey**mise à jour associée.</span><span class="sxs-lookup"><span data-stu-id="7d083-118">For nonrecurring tasks or for the last occurrence of a recurring task, the UpdateItem response returns the same **Id** that was passed to it and returns the associated updated **ChangeKey**.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="7d083-119">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7d083-119">See also</span></span>



[<span data-ttu-id="7d083-120">UpdateItem Operation</span><span class="sxs-lookup"><span data-stu-id="7d083-120">UpdateItem operation</span></span>](updateitem-operation.md)


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
description: L’opération UpdateItem est utilisée pour mettre à jour les propriétés d’élément de tâche dans la banque d’informations Exchange.
ms.openlocfilehash: d6f966fa663300b476383a136d30cf611d6bfb9b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838888"
---
# <a name="updateitem-operation-task"></a><span data-ttu-id="56c96-103">Opération UpdateItem (tâche)</span><span class="sxs-lookup"><span data-stu-id="56c96-103">UpdateItem operation (task)</span></span>

<span data-ttu-id="56c96-104">L’opération UpdateItem est utilisée pour mettre à jour les propriétés d’élément de tâche dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="56c96-104">The UpdateItem operation is used to update task item properties in the Exchange store.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="56c96-105">Remarques</span><span class="sxs-lookup"><span data-stu-id="56c96-105">Remarks</span></span>

<span data-ttu-id="56c96-106">Vous ne pouvez pas utiliser les Services Web Exchange pour envoyer les demandes de tâche.</span><span class="sxs-lookup"><span data-stu-id="56c96-106">You cannot use Exchange Web Services to send task requests.</span></span> <span data-ttu-id="56c96-107">Services Web Exchange peut renvoyer des demandes de tâches qui sont créés par MicrosoftOfficeOutlook.</span><span class="sxs-lookup"><span data-stu-id="56c96-107">Exchange Web Services can return task requests that are created by MicrosoftOfficeOutlook.</span></span> <span data-ttu-id="56c96-108">Si une demande de tâche a déjà été envoyée, une demande de mise à jour de la tâche renverra une erreur.</span><span class="sxs-lookup"><span data-stu-id="56c96-108">If a task request has already been sent, a request to update the task will return an error.</span></span>
  
## <a name="updating-the-current-occurrence-of-a-recurring-task"></a><span data-ttu-id="56c96-109">Mise à jour de l’Occurrence en cours d’une tâche périodique</span><span class="sxs-lookup"><span data-stu-id="56c96-109">Updating the Current Occurrence of a Recurring Task</span></span>

<span data-ttu-id="56c96-110">Le résultat d’une opération UpdateItem sur les tâches récurrentes diffère le résultat de l’opération UpdateItem sur une seule tâche non périodique.</span><span class="sxs-lookup"><span data-stu-id="56c96-110">The result of an UpdateItem operation on recurring tasks differs from the result of the UpdateItem operation on a single, nonrecurring task.</span></span> <span data-ttu-id="56c96-111">Modifications apportées à une occurrence d’une tâche périodique entraînent des tâches uniques à être généré lorsque les mises à jour suivantes sont apportées :</span><span class="sxs-lookup"><span data-stu-id="56c96-111">Changes to an occurrence of a recurring task cause one-off tasks to be generated when the following updates are made:</span></span>
  
1. <span data-ttu-id="56c96-112">La propriété status d’une tâche périodique régénération ou nonregenerating est définie sur **terminée**.</span><span class="sxs-lookup"><span data-stu-id="56c96-112">The status property of a regenerating or nonregenerating recurrent task is set to **Completed**.</span></span>
    
2. <span data-ttu-id="56c96-113">La date de début ou date de fin d’une tâche périodique nonregenerating est modifiée.</span><span class="sxs-lookup"><span data-stu-id="56c96-113">The start date or end date of a nonregenerating recurrent task is changed.</span></span>
    
<span data-ttu-id="56c96-114">Par exemple, si **une demande **UpdateItem** affecte la valeur d’une tâche périodique,** **UpdateItemResponse** inclut un nouvel Id et ChangeKey qui représentent une tâche unique nouvellement créée.</span><span class="sxs-lookup"><span data-stu-id="56c96-114">For example, if an **UpdateItem** request sets the Completed value of a recurring task to **true**, the **UpdateItemResponse** will include a new Id and ChangeKey that represent a newly created one-off task.</span></span> <span data-ttu-id="56c96-115">L’Id qui a été inclus dans la demande est toujours valide et la tâche périodique qui est représentée par cet Id a été mis à jour pour représenter l’occurrence suivante.</span><span class="sxs-lookup"><span data-stu-id="56c96-115">The Id that was included in the request is still valid and the recurring task that is represented by that Id has been updated to represent the next occurrence.</span></span> <span data-ttu-id="56c96-116">Le ChangeKey qui a été inclus dans la demande n’est plus valide car la tâche périodique a été mis à jour.</span><span class="sxs-lookup"><span data-stu-id="56c96-116">The ChangeKey that was included in the request is no longer valid because the recurring task has been updated.</span></span> 
  
<span data-ttu-id="56c96-117">Vous pouvez utiliser l' [opération GetItem](getitem-operation.md) pour obtenir les dernières **ChangeKey** pour la tâche périodique.</span><span class="sxs-lookup"><span data-stu-id="56c96-117">You can use the [GetItem operation](getitem-operation.md) to get the latest **ChangeKey** for the recurring task.</span></span> 
  
<span data-ttu-id="56c96-118">Pour les tâches non récurrentes ou la dernière occurrence d’une tâche périodique, la réponse UpdateItem renvoie le même **Id** qui a été passé et qu’elle renvoie qu'associé **ChangeKey**mis à jour.</span><span class="sxs-lookup"><span data-stu-id="56c96-118">For nonrecurring tasks or for the last occurrence of a recurring task, the UpdateItem response returns the same **Id** that was passed to it and returns the associated updated **ChangeKey**.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="56c96-119">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="56c96-119">See also</span></span>



[<span data-ttu-id="56c96-120">UpdateItem Operation</span><span class="sxs-lookup"><span data-stu-id="56c96-120">UpdateItem operation</span></span>](updateitem-operation.md)


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
# <a name="updateitem-operation-task"></a>Opération UpdateItem (tâche)

L’opération UpdateItem est utilisée pour mettre à jour les propriétés d’élément de tâche dans la Banque d’Exchange.
  
## <a name="remarks"></a>Remarques

Vous ne pouvez pas utiliser les services Web Exchange pour envoyer des demandes de tâches. Les services Web Exchange peuvent renvoyer des demandes de tâche créées par MicrosoftOfficeOutlook. Si une demande de tâche a déjà été envoyée, une demande de mise à jour de la tâche renverra une erreur.
  
## <a name="updating-the-current-occurrence-of-a-recurring-task"></a>Mise à jour de l’occurrence actuelle d’une tâche périodique

Le résultat d’une opération UpdateItem sur les tâches récurrentes diffère du résultat de l’opération UpdateItem sur une tâche unique, non périodique. Les modifications apportées à une occurrence d’une tâche périodique entraînent la génération de tâches ponctuelles lorsque les mises à jour suivantes sont effectuées :
  
1. La propriété Status d’une tâche récurrente de régénération ou nonregenerating est définie sur **terminé**.
    
2. La date de début ou la date de fin d’une tâche récurrente nonregenerating est modifiée.
    
Par exemple, si une requête **UpdateItem** définit la valeur achevée d’une tâche périodique sur **true**, le **UpdateItemResponse** inclut un nouvel ID et ChangeKey qui représentent une nouvelle tâche ponctuelle. L’ID qui a été inclus dans la demande est toujours valide et la tâche périodique représentée par cet ID a été mise à jour pour représenter l’occurrence suivante. Le ChangeKey qui a été inclus dans la demande n’est plus valide car la tâche périodique a été mise à jour. 
  
Vous pouvez utiliser l' [opération GetItem](getitem-operation.md) pour obtenir la dernière **ChangeKey** de la tâche périodique. 
  
Pour les tâches non périodiques ou pour la dernière occurrence d’une tâche périodique, la réponse UpdateItem renvoie le même **ID** qui lui a été passé et renvoie la **ChangeKey**mise à jour associée.
  
## <a name="see-also"></a>Voir aussi



[UpdateItem Operation](updateitem-operation.md)


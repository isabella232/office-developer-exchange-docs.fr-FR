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
# <a name="updateitem-operation-task"></a>Opération UpdateItem (tâche)

L’opération UpdateItem est utilisée pour mettre à jour les propriétés d’élément de tâche dans la banque d’informations Exchange.
  
## <a name="remarks"></a>Remarques

Vous ne pouvez pas utiliser les Services Web Exchange pour envoyer les demandes de tâche. Services Web Exchange peut renvoyer des demandes de tâches qui sont créés par MicrosoftOfficeOutlook. Si une demande de tâche a déjà été envoyée, une demande de mise à jour de la tâche renverra une erreur.
  
## <a name="updating-the-current-occurrence-of-a-recurring-task"></a>Mise à jour de l’Occurrence en cours d’une tâche périodique

Le résultat d’une opération UpdateItem sur les tâches récurrentes diffère le résultat de l’opération UpdateItem sur une seule tâche non périodique. Modifications apportées à une occurrence d’une tâche périodique entraînent des tâches uniques à être généré lorsque les mises à jour suivantes sont apportées :
  
1. La propriété status d’une tâche périodique régénération ou nonregenerating est définie sur **terminée**.
    
2. La date de début ou date de fin d’une tâche périodique nonregenerating est modifiée.
    
Par exemple, si **une demande **UpdateItem** affecte la valeur d’une tâche périodique,** **UpdateItemResponse** inclut un nouvel Id et ChangeKey qui représentent une tâche unique nouvellement créée. L’Id qui a été inclus dans la demande est toujours valide et la tâche périodique qui est représentée par cet Id a été mis à jour pour représenter l’occurrence suivante. Le ChangeKey qui a été inclus dans la demande n’est plus valide car la tâche périodique a été mis à jour. 
  
Vous pouvez utiliser l' [opération GetItem](getitem-operation.md) pour obtenir les dernières **ChangeKey** pour la tâche périodique. 
  
Pour les tâches non récurrentes ou la dernière occurrence d’une tâche périodique, la réponse UpdateItem renvoie le même **Id** qui a été passé et qu’elle renvoie qu'associé **ChangeKey**mis à jour.
  
## <a name="see-also"></a>Voir aussi



[UpdateItem Operation](updateitem-operation.md)


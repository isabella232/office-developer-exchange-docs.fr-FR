---
title: Opération UpdateItem (tâche)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- UpdateItem
api_type:
- schema
ms.assetid: b0a7f114-d040-40eb-a8f3-05ea6489e472
description: L’opération UpdateItem est utilisée pour mettre à jour les propriétés d’élément de tâche dans Exchange store.
ms.openlocfilehash: a268b4b281f149f14bc6c48a774fc9071093ebb5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510749"
---
# <a name="updateitem-operation-task"></a>Opération UpdateItem (tâche)

L’opération UpdateItem est utilisée pour mettre à jour les propriétés d’élément de tâche dans Exchange store.
  
## <a name="remarks"></a>Remarques

Vous ne pouvez pas utiliser Exchange Web Services web pour envoyer des demandes de tâches. Exchange Les services web peuvent renvoyer des demandes de tâches créées par MicrosoftOfficeOutlook. Si une demande de tâche a déjà été envoyée, une demande de mise à jour de la tâche retourne une erreur.
  
## <a name="updating-the-current-occurrence-of-a-recurring-task"></a>Mise à jour de l’occurrence actuelle d’une tâche périodique

Le résultat d’une opération UpdateItem sur des tâches périodiques diffère du résultat de l’opération UpdateItem sur une tâche unique non périodique. Les modifications apportées à une occurrence d’une tâche périodique entraînent la générer lors des mises à jour suivantes :
  
1. La propriété d’état d’une tâche périodique régénérant ou non régénérant est définie sur **Terminé**.
    
2. La date de début ou de fin d’une tâche périodique non régénérante est modifiée.
    
Par exemple, si une demande **UpdateItem** définit la valeur Terminée d’une tâche périodique sur **true,** **UpdateItemResponse** inclut un nouvel ID et ChangeKey qui représentent une tâche qui vient d’être créée. L’ID qui a été inclus dans la demande est toujours valide et la tâche périodique représentée par cet ID a été mise à jour pour représenter l’occurrence suivante. La clé ChangeKey incluse dans la demande n’est plus valide car la tâche périodique a été mise à jour. 
  
Vous pouvez utiliser [l’opération GetItem](getitem-operation.md) pour obtenir la dernière **changeKey** pour la tâche périodique. 
  
Pour les tâches non récurrentes ou pour la dernière occurrence d’une tâche périodique, la réponse UpdateItem renvoie le même **ID** qui lui a été transmis et renvoie la clé ChangeKey mise à **jour associée.**
  
## <a name="see-also"></a>Voir aussi



[UpdateItem Operation](updateitem-operation.md)


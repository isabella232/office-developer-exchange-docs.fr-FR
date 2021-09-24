---
title: découverte électronique dans EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 3128419f-dd5f-46d2-bb0d-0940738d0bb6
description: Découvrez eDiscovery dans EWS dans Exchange.
ms.openlocfilehash: 0b4f211e7f8a6ec085fd03ada1cc5a35187106e9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512309"
---
# <a name="ediscovery-in-ews-in-exchange"></a>découverte électronique dans EWS dans Exchange

Découvrez eDiscovery dans EWS dans Exchange.
  
eDiscovery est un service web de requête fédérée qui permet aux applications externes d’effectuer des requêtes de Exchange données.
  
La découverte se compose de plusieurs phases, y compris l’identification et la conservation des données clés, l’élimination et l’examen des données, ainsi que la production de données devant un tribunal. Les requêtes eDiscovery facilitent le processus de découverte en fournissant un flux de travail de découverte unique Exchange et SharePoint.
  
## <a name="ediscovery-operations"></a>Opérations eDiscovery

La fonctionnalité eDiscovery exposée par EWS est disponible via les opérations introduites dans Exchange Online, Exchange Online dans le cadre de Office 365 et les versions de Exchange à partir de Exchange 2013. 
  
**Tableau 1. Nouvelles opérations pour eDiscovery**

|**Nom de l’opération**|**Description**|
|:-----|:-----|
|[GetDiscoverySearchConfiguration](https://msdn.microsoft.com/library/8a54a6dc-110c-4972-a8bc-5ddb43c4b857%28Office.15%29.aspx) <br/> |Obtient des informations de configuration pour les conserves sur place, les recherches de découverte enregistrées et les boîtes aux lettres activées pour la recherche de découverte.  <br/> |
|[GetHoldOnMailboxes](https://msdn.microsoft.com/library/9157f329-80b4-4cd0-a158-378064966ae6%28Office.15%29.aspx) <br/> |Obtient l’état d’une mise en attente basée sur une requête, qui est définie à l’aide de l’opération [SetHoldOnMailboxes](https://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx).  <br/> |
|[GetNonIndexableItemDetails](https://msdn.microsoft.com/library/9279c3ad-f7c8-4bbc-b0a7-2c78416cb39a%28Office.15%29.aspx) <br/> |Récupère des détails sur les éléments qui ne peuvent pas être indexés. Cela inclut, sans s’y limiter, l’identificateur de l’élément, un code d’erreur, une description d’erreur, lorsqu’une tentative d’indexation de l’élément a été tentée et des informations supplémentaires sur le fichier.  <br/> |
|[GetNonIndexableItemStatistics](https://msdn.microsoft.com/library/ed077877-9d98-4434-b8b6-a4a905e7f7a6%28Office.15%29.aspx) <br/> |Récupère le nombre d’éléments qui ne peuvent pas être indexés dans une boîte aux lettres.  <br/> |
|[GetSearchableMailboxes](https://msdn.microsoft.com/library/47f8ff57-4835-4d2d-9136-44afb31a4cbe%28Office.15%29.aspx) <br/> |Obtient la liste des boîtes aux lettres sur qui le client est autorisé à effectuer des recherches ou à effectuer une découverte électronique.  <br/> |
|[SearchMailboxes](https://msdn.microsoft.com/library/8a67c1d8-d021-4e68-aa62-35f7d9c2edc7%28Office.15%29.aspx) <br/> |Recherche des éléments dans des boîtes aux lettres spécifiques qui correspondent à des mots clés de requête.  <br/> |
|[SetHoldOnMailboxes](https://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx) <br/> |Définit une attente basée sur une requête sur les éléments.  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)
    
- [Commencer à utiliser les services web dans Exchange](start-using-web-services-in-exchange.md)
    
- [Vue d'ensemble de la conception client EWS pour Exchange](ews-client-design-overview-for-exchange.md)
    


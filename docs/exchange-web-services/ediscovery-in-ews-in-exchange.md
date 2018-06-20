---
title: découverte électronique dans EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 3128419f-dd5f-46d2-bb0d-0940738d0bb6
description: En savoir plus sur la découverte électronique dans EWS dans Exchange.
ms.openlocfilehash: 6491fdd9f2246870a89bfa89bf7d97b972d67c92
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754765"
---
# <a name="ediscovery-in-ews-in-exchange"></a>découverte électronique dans EWS dans Exchange

En savoir plus sur la découverte électronique dans EWS dans Exchange.
  
découverte électronique est un service web requête fédérée qui permet aux applications externes d’effectuer des requêtes de données Exchange.
  
Découverte comprend plusieurs étapes, y compris identification préserver les données critiques, élimination vers le bas et examen des données et créer des données dans un tribunal. requêtes eDiscovery facilitent le processus de découverte en fournissant un flux de travail unique découverte entre Exchange et SharePoint.
  
## <a name="ediscovery-operations"></a>opérations de découverte électronique

La fonctionnalité de découverte électronique qui est exposée par EWS est disponible par le biais d’opérations introduites dans Exchange Online, Exchange Online dans le cadre d’Office 365 et les versions d’Exchange commençant par Exchange 2013. 
  
**Le tableau 1. Nouvelles opérations eDiscovery**

|**Nom de l’opération**|**Description**|
|:-----|:-----|
|[GetDiscoverySearchConfiguration](http://msdn.microsoft.com/library/8a54a6dc-110c-4972-a8bc-5ddb43c4b857%28Office.15%29.aspx) <br/> |Obtient les informations de configuration pour les archives permanentes, enregistrement des recherches de découverte et les boîtes aux lettres qui sont activées pour la recherche de découverte.  <br/> |
|[GetHoldOnMailboxes](http://msdn.microsoft.com/library/9157f329-80b4-4cd0-a158-378064966ae6%28Office.15%29.aspx) <br/> |Obtient l’état d’une suspension basée sur une requête, qui est définie à l’aide de l' [opération SetHoldOnMailboxes](http://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx).  <br/> |
|[GetNonIndexableItemDetails](http://msdn.microsoft.com/library/9279c3ad-f7c8-4bbc-b0a7-2c78416cb39a%28Office.15%29.aspx) <br/> |Récupère le plus d’informations sur les éléments qui ne peuvent pas être indexés. Cela inclut, mais n’est pas limité à l’identificateur d’élément, un code d’erreur, une description de l’erreur lors de la tentative d’index de l’élément et des informations supplémentaires sur le fichier.  <br/> |
|[GetNonIndexableItemStatistics](http://msdn.microsoft.com/library/ed077877-9d98-4434-b8b6-a4a905e7f7a6%28Office.15%29.aspx) <br/> |Récupère le nombre d’éléments qui ne peuvent pas être indexés dans une boîte aux lettres.  <br/> |
|[GetSearchableMailboxes](http://msdn.microsoft.com/library/47f8ff57-4835-4d2d-9136-44afb31a4cbe%28Office.15%29.aspx) <br/> |Obtient une liste des boîtes aux lettres que le client a l’autorisation de rechercher ou d’effectuer une découverte électronique sur.  <br/> |
|[SearchMailboxes](http://msdn.microsoft.com/library/8a67c1d8-d021-4e68-aa62-35f7d9c2edc7%28Office.15%29.aspx) <br/> |Recherche des éléments dans des boîtes aux lettres spécifiques qui correspondent à des mots clés de requête.  <br/> |
|[SetHoldOnMailboxes](http://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx) <br/> |Ensembles de basée sur une requête en attente sur les éléments.  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)
    
- [Commencer à utiliser les services web dans Exchange](start-using-web-services-in-exchange.md)
    
- [Vue d'ensemble de la conception client EWS pour Exchange](ews-client-design-overview-for-exchange.md)
    


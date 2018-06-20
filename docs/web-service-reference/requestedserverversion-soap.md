---
title: RequestedServerVersion (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: cf3f9d7a-2add-4457-b009-2929220f90b5
description: L’élément RequestedServerVersion spécifie la version du serveur une méthode de découverte automatique cibles d’appels.
ms.openlocfilehash: 6b9d31f3b7bca087652f04e4943becc5ac4e68e7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829132"
---
# <a name="requestedserverversion-soap"></a>RequestedServerVersion (SOAP)

L’élément **RequestedServerVersion** spécifie la version du serveur une méthode de **découverte automatique** cibles d’appels. 
  
```XML
<RequestedServerVersion/>
```

 **ExchangeVersion**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="text-value"></a>Valeur de texte

La valeur de texte de l’élément **RequestedServerVersion** spécifie la version du serveur une méthode de **découverte automatique** cibles d’appels. Le tableau suivant répertorie les versions de serveur valide. 
  
|**Valeur texte**|**Description**|
|:-----|:-----|
|Exchange2007_SP1  <br/> |Exchange Server 2007 Service Pack 1 (SP1).  <br/> |
|Exchange2010  <br/> |Exchange Server 2010.  <br/> |
|Exchange2010_SP1  <br/> |Exchange Server 2010 Service Pack 1 (SP1).  <br/> |
|Exchange2010_SP2  <br/> |Exchange Server 2010 Service Pack 2 (SP2).  <br/> |
|Exchange2013  <br/> |Exchange Server 2013. Le champ Exchange2013 est applicable pour les clients qui ciblent Exchange Online et versions d’Exchange commençant par Exchange Server 2013.  <br/> |
|Exchange2013_SP1  <br/> |Exchange Server 2013 Service Pack 1 (SP1). Le champ Exchange2013_SP1 est applicable pour les clients qui ciblent Exchange Online et versions d’Exchange commençant par Exchange Server 2013 SP1.  <br/> |
   
## <a name="remarks"></a>Remarques

L’élément **RequestedServerVersion** est définie dans l’en-tête SOAP. 
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |messages.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   


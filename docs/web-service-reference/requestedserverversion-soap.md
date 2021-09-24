---
title: RequestedServerVersion (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: cf3f9d7a-2add-4457-b009-2929220f90b5
description: L’élément RequestedServerVersion spécifie la version du serveur ciblée par un appel de méthode de découverte automatique.
ms.openlocfilehash: 0690481523ab48497c40338a8808dfa2ed9b0e99
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540558"
---
# <a name="requestedserverversion-soap"></a>RequestedServerVersion (SOAP)

**L’élément RequestedServerVersion** spécifie la  version du serveur ciblée par un appel de méthode de découverte automatique. 
  
```XML
<RequestedServerVersion/>
```

 **ExchangeVersion**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="text-value"></a>Valeur texte

La valeur texte de **l’élément RequestedServerVersion**  spécifie la version du serveur ciblée par un appel de méthode de découverte automatique. Le tableau suivant répertorie les versions de serveur valides. 
  
|**Valeur de texte**|**Description**|
|:-----|:-----|
|Exchange2007_SP1  <br/> |Exchange Server 2007 Service Pack 1 (SP1).  <br/> |
|Exchange2010  <br/> |Exchange Server 2010.  <br/> |
|Exchange2010_SP1  <br/> |Exchange Server 2010 Service Pack 1 (SP1).  <br/> |
|Exchange2010_SP2  <br/> |Exchange Server 2010 Service Pack 2 (SP2).  <br/> |
|Exchange2013  <br/> |Exchange Server 2013. Le champ Exchange2013 s’applique aux clients qui ciblent Exchange Online et les versions de Exchange à partir de Exchange Server 2013.  <br/> |
|Exchange2013_SP1  <br/> |Exchange Server 2013 Service Pack 1 (SP1). Le Exchange2013_SP1 est applicable pour les clients qui ciblent Exchange Online et les versions de Exchange à partir de Exchange Server 2013 SP1.  <br/> |
   
## <a name="remarks"></a>Remarques

**L’élément RequestedServerVersion** est définie dans l’en-tête SOAP. 
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |messages.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   


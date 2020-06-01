---
title: GetDiscoverySearchConfigurationResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9d963e6c-e94d-462b-8c44-95d55c848fb2
description: L’élément GetDiscoverySearchConfigurationResponse spécifie la réponse à une demande GetDiscoverySearchConfiguration.
ms.openlocfilehash: 98393943434b5e3460485b7d75c2b5285983f597
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460980"
---
# <a name="getdiscoverysearchconfigurationresponse"></a>GetDiscoverySearchConfigurationResponse

L’élément **GetDiscoverySearchConfigurationResponse** spécifie la réponse à une demande **GetDiscoverySearchConfiguration** . 
  
```XML
<GetDiscoverySearchConfigurationResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <DiscoverySearchConfigurations/>
</GetDiscoverySearchConfigurationResponse>
```

 **GetDiscoverySearchConfigurationResponseMessageType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

[MessageText](messagetext.md)  |  [ResponseCode](responsecode.md)  |  [DescriptiveLinkKey](descriptivelinkkey.md)  |  [Messagexml](messagexml.md)  |  [DiscoverySearchConfigurations](discoverysearchconfigurations.md)
  
### <a name="parent-elements"></a>Éléments parents

[ResponseMessages](responsemessages.md)
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |false  <br/> |
   


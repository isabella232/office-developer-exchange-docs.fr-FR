---
title: GetClientExtension
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c96c2b4c-45cb-482a-a3bb-7a11a0fff43b
description: L’élément GetClientExtension représente une demande pour obtenir une extension de client.
ms.openlocfilehash: 9d3abb4572a5f74f24925d24a2fbbe8ded593731
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756546"
---
# <a name="getclientextension"></a>GetClientExtension

L’élément **GetClientExtension** représente une demande pour obtenir une extension de client. 
  
```XML
<GetClientExtension>
   <RequestedExtensionIds/>
   <UserParameters/>
   <IsDebug/>
</GetClientExtension>
```

 ****
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

[RequestedExtensionIds](requestedextensionids.md) | [UserParameters](userparameters.md) | [IsDebug](isdebug.md)
  
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> ||
   


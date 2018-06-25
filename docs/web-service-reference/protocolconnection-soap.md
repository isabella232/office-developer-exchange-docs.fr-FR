---
title: ProtocolConnection (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 6eef2188-6194-48f1-ad7e-46104aecdf56
description: L’élément ProtocolConnection représente le protocole de connexion du client Web server.
ms.openlocfilehash: 8b5396821cd959e41d24fcf7a94c519f9c634a1f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828915"
---
# <a name="protocolconnection-soap"></a>ProtocolConnection (SOAP)

L’élément **ProtocolConnection** représente le protocole de connexion du client Web server. 
  
```XML
<ProtocolConnection>
   <Hostname/>
   <Port/>
   <EncryptionMethod/>
</ProtocolConnection>
```

 **ProtocolConnection**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Nom d’hôte (SOAP)](hostname-soap.md) <br/> |Représente la partie de nom d’hôte du nom complet de l’ordinateur de l’ordinateur.  <br/> |
|[Port (SOAP)](port-soap.md) <br/> |Représente le numéro de port à utiliser pour le protocole.  <br/> |
|[EncryptionMethod (SOAP)](encryptionmethod-soap.md) <br/> |Représente la méthode de chiffrement qui est utilisée pour les protocoles POP, IMAP et SMTP.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ProtocolConnections (SOAP)](protocolconnections-soap.md) <br/> |Contient zéro ou plusieurs connexions de protocole.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



[ProtocolConnectionCollectionSetting (SOAP)](protocolconnectioncollectionsetting-soap.md)


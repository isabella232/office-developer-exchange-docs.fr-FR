---
title: PhoneCallInformation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- PhoneCallInformation
api_type:
- schema
ms.assetid: a0363c42-6d35-4074-bc17-946eb12736ff
description: L’élément PhoneCallInformation spécifie les informations d’état d’un appel téléphonique.
ms.openlocfilehash: 815e0ffac761b12969483752f5022f8580f6cc62
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59528325"
---
# <a name="phonecallinformation"></a>PhoneCallInformation

**L’élément PhoneCallInformation** spécifie les informations d’état d’un appel téléphonique. 
  
```XML
<PhoneCallInformation>
   <PhoneCallState/>
   <ConnectionFailureCause/>
   <SIPResponseText/>
   <SIPResponseCode/>
</PhoneCallInformation>
```

 **PhoneCallInformationType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[PhoneCallState](phonecallstate.md) <br/> |Spécifie l’état d’un appel téléphonique. Cet élément est obligatoire.  <br/> |
|[ConnectionFailureCause](connectionfailurecause.md) <br/> |Spécifie la cause d’une défaillance de connexion. Cet élément est obligatoire.  <br/> |
|[SIPResponseText](sipresponsetext.md) <br/> |Spécifie le texte de réponse SIP. Cet élément est facultatif.  <br/> |
|[SIPResponseCode](sipresponsecode.md) <br/> |Spécifie le code de réponse SIP. Cet élément est facultatif.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetPhoneCallInformationResponse](getphonecallinformationresponse.md) <br/> |Définit une réponse à une [demande d’opération GetPhoneCallInformation.](getphonecallinformation-operation.md)  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)


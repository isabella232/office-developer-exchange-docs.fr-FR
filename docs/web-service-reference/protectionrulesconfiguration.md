---
title: ProtectionRulesConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ProtectionRulesConfiguration
api_type:
- schema
ms.assetid: e5b4699a-476e-4053-bb52-873eb921c046
description: L’élément ProtectionRulesConfiguration contient des informations de configuration de service pour le service de règles de protection.
ms.openlocfilehash: 0d88f5c8ef414c96ae5f65cf3f82362fe2137472
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516403"
---
# <a name="protectionrulesconfiguration"></a>ProtectionRulesConfiguration

**L’élément ProtectionRulesConfiguration** contient des informations de configuration de service pour le service de règles de protection. 
  
```XML
<ProtectionRulesConfiguration RefreshInterval="">
   <Rules/>
   <InternalDomains/>
</ProtectionRulesConfiguration>
```

 **ProtectionRulesServiceConfiguration**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**RefreshInterval** <br/> |Spécifie la fréquence, en heures entières, pendant combien de temps le client doit demander des règles de protection au serveur. Cet attribut est obligatoire et sa valeur doit être un nombre inférieur ou supérieur à 1.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Règles ](rules-ex15websvcsotherref.md) <br/> |Tableau de règles de protection. Cet élément est obligatoire.  <br/> |
|[InternalDomains (SmtpDomainList)](internaldomains-smtpdomainlist.md) <br/> |Identifie la liste des domaines SMTP internes de l’organisation. Cet élément est obligatoire.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ServiceConfigurationResponseMessageType](serviceconfigurationresponsemessagetype.md) <br/> |Contient les paramètres de configuration du service.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

La configuration du service des règles de protection se compose d’une liste de règles, de domaines internes et d’un intervalle d’actualisation.
  
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


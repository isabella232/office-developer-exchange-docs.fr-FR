---
title: DomainResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 6aa319be-3a01-4044-8dfc-8fa1318524c3
description: L’élément DomainResponse contient les paramètres demandés pour le domaine spécifié.
ms.openlocfilehash: dea6e36c51ceea53201b668cfba616c03a44df86
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456961"
---
# <a name="domainresponse-soap"></a>DomainResponse (SOAP)

L’élément **DomainResponse** contient les paramètres demandés pour le domaine spécifié. 
  
```XML
<DomainResponse>
   <DomainSettingErrors/>
   <DomainSettings/>
   <RedirectTarget/>
   <ErrorCode/>
   <ErrorMessage/>
</DomainResponse>
```

 **DomainResponse**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[DomainSettingErrors (SOAP)](domainsettingerrors-soap.md) <br/> |Contient des informations d’erreur pour les paramètres qui n’ont pas pu être renvoyés.  <br/> |
|[DomainSettings (SOAP)](domainsettings-soap.md) <br/> |Représente les paramètres de domaine qui ont été envoyés dans une demande de découverte automatique ou renvoyés par une réponse de découverte automatique.  <br/> |
|[RedirectTarget (SOAP)](redirecttarget-soap.md) <br/> |Identifie la cible de la redirection. La cible peut être une URL ou une adresse de messagerie.  <br/> |
|[ErrorCode (SOAP)](errorcode-soap.md) <br/> |Spécifie le code d’erreur associé à la demande spécifique.  <br/> |
|[ErrorMessage (SOAP)](errormessage-soap.md) <br/> |Spécifie le message d’erreur qui est associé à la demande spécifique.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ArrayOfDomainResponse (SOAP)](arrayofdomainresponse-soap.md) <br/> |Contient un tableau d’éléments **DomainResponse** . Chaque élément **DomainResponse** contient les paramètres demandés pour l’utilisateur spécifié.  <br/> |
|[DomainResponses (SOAP)](domainresponses-soap.md) <br/> |Contient les réponses pour chaque domaine.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucune.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)


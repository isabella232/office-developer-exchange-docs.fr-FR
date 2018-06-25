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
description: L’élément DomainResponse contient les paramètres requis pour le domaine spécifié.
ms.openlocfilehash: c40f33a278b5032913329a7cd64346b572f5df2f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756033"
---
# <a name="domainresponse-soap"></a>DomainResponse (SOAP)

L’élément **DomainResponse** contient les paramètres requis pour le domaine spécifié. 
  
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

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[DomainSettingErrors (SOAP)](domainsettingerrors-soap.md) <br/> |Contient des informations d’erreur pour les paramètres qui ne peut pas être retourné.  <br/> |
|[DomainSettings (SOAP)](domainsettings-soap.md) <br/> |Représente les paramètres de domaine qui ont été envoyés dans une requête de découverte automatique ou renvoyés par une réponse de découverte automatique.  <br/> |
|[RedirectTarget (SOAP)](redirecttarget-soap.md) <br/> |Identifie la cible de la redirection. La cible peut être une URL ou une adresse de messagerie.  <br/> |
|[ErrorCode (SOAP)](errorcode-soap.md) <br/> |Spécifie le code d’erreur qui est associé à la demande spécifique.  <br/> |
|[ErrorMessage (SOAP)](errormessage-soap.md) <br/> |Spécifie le message d’erreur qui est associé à la demande spécifique.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ArrayOfDomainResponse (SOAP)](arrayofdomainresponse-soap.md) <br/> |Contient un tableau d’éléments **DomainResponse** . Chaque élément **DomainResponse** contient les paramètres requis pour l’utilisateur spécifié.  <br/> |
|[DomainResponses (SOAP)](domainresponses-soap.md) <br/> |Contient les réponses pour chaque domaine.  <br/> |
   
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

- [Opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)


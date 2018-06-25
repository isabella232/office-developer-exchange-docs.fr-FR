---
title: SerializedSecurityContext
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SerializedSecurityContext
api_type:
- schema
ms.assetid: a02c4fc1-ed1a-40d9-a18e-6cfdae21a690
description: L’élément SerializedSecurityContext est utilisé dans l’en-tête SOAP Simple Object Access Protocol () pour la sérialisation de jeton de l’authentification de serveur à serveur. Sérialisation de jeton n’est pas pris en charge.
ms.openlocfilehash: c5590551dc0780d918b05902e4f48fb9d1390b59
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829363"
---
# <a name="serializedsecuritycontext"></a>SerializedSecurityContext

L’élément **SerializedSecurityContext** est utilisé dans l’en-tête SOAP Simple Object Access Protocol () pour la sérialisation de jeton de l’authentification de serveur à serveur. Sérialisation de jeton n’est pas pris en charge. 
  
```xml
<SerializedSecurityContext>
   <UserSid/>
   <GroupSids/>
   <RestrictedGroupSids/>
   <PrimarySmtpAddress/>
</SerializedSecurityContext>
```

 **SerializedSecurityContextType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[UserSid](usersid.md) <br/> |Représente le formulaire sécurité descripteur definition language (SDDL) de l’identificateur de sécurité utilisateur dans un en-tête SOAP de contexte sérialisés de sécurité.  <br/> |
|[GroupSids](groupsids.md) <br/> |Représente une collection d’identificateurs de sécurité Active Directory directory service groupe objet.  <br/> |
|[RestrictedGroupSids](restrictedgroupsids.md) <br/> |Représente l’identificateur du groupe de sécurité et les attributs d’un groupe restreint.  <br/> |
|[PrimarySmtpAddress](primarysmtpaddress.md) <br/> |Représente l’adresse SMTP Simple Mail Transfer Protocol () principal d’un compte à utiliser pour l’autorisation de serveur à serveur.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2007 ayant le rôle de serveur (CAS) d’accès au Client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)


[Autorisation de serveur à serveur dans EWS](http://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)


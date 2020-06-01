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
description: L’élément SerializedSecurityContext est utilisé dans l’en-tête SOAP (Simple Object Access Protocol) pour la sérialisation de jetons dans l’authentification de serveur à serveur. La sérialisation de jetons n’est pas prise en charge.
ms.openlocfilehash: 58fea1c7f613315d59e81935561f92f318afc769
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462051"
---
# <a name="serializedsecuritycontext"></a>SerializedSecurityContext

L’élément **SerializedSecurityContext** est utilisé dans l’en-tête SOAP (Simple Object Access Protocol) pour la sérialisation de jetons dans l’authentification de serveur à serveur. La sérialisation de jetons n’est pas prise en charge. 
  
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

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[UserSid](usersid.md) <br/> |Représente la forme SDDL (Security Descriptor Definition Language) de l’identificateur de sécurité de l’utilisateur dans un en-tête SOAP de contexte de sécurité sérialisé.  <br/> |
|[GroupSids](groupsids.md) <br/> |Représente une collection d’identificateurs de sécurité d’objet de groupe de service d’annuaire Active Directory.  <br/> |
|[RestrictedGroupSids](restrictedgroupsids.md) <br/> |Représente l’identificateur de sécurité de groupe et les attributs d’un groupe restreint.  <br/> |
|[PrimarySmtpAddress](primarysmtpaddress.md) <br/> |Représente l’adresse SMTP (Simple Mail Transfer Protocol) principale d’un compte à utiliser pour l’autorisation de serveur à serveur.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d’accès au client (CAS) est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML EWS dans Exchange](ews-xml-elements-in-exchange.md)


[Autorisation de serveur à serveur dans EWS](https://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)


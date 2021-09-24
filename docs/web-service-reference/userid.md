---
title: UserId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- UserId
api_type:
- schema
ms.assetid: 244af9e0-bf3c-46b4-8bfa-9719a1ed3107
description: L’élément UserId identifie un utilisateur délégué ou un utilisateur qui dispose d’autorisations d’accès aux dossiers.
ms.openlocfilehash: f03914745f8f7f47c64685b3e7c52eefece5ff6d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510756"
---
# <a name="userid"></a>UserId

**L’élément UserId** identifie un utilisateur délégué ou un utilisateur qui dispose d’autorisations d’accès aux dossiers. 
  
```xml
<UserId>
   <SID/>
   <PrimarySmtpAddress/>
   <DisplayName/>
   <DistinguishedUser/>
   <ExternalUserIdentity/>
</UserId>
```

 **UserIdType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[SID](sid.md) <br/> |Représente le formulaire SDDL (Security Descriptor Definition Language) de l’identificateur de sécurité (SID).  <br/> |
|[PrimarySmtpAddress](primarysmtpaddress.md) <br/> |Représente l’adresse SMTP (Simple Mail Transfer Protocol) principale d’un compte à utiliser pour l’accès délégué.  <br/> |
|[DisplayName (chaîne)](displayname-string.md) <br/> |Définit le nom complet d’un dossier, d’un contact, d’une liste de distribution ou d’un utilisateur délégué.  <br/> |
|[DistinguishedUser](distinguisheduser.md) <br/> |Identifie les comptes d’utilisateur anonymes et par défaut pour l’accès délégué.  <br/> |
|[ExternalUserIdentity](externaluseridentity.md) <br/> |Identifie un utilisateur délégué externe ou un utilisateur externe qui dispose d’autorisations d’accès aux dossiers.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[DelegateUser](delegateuser.md) <br/> |Identifie un délégué unique à ajouter ou à mettre à jour dans une boîte aux lettres.  <br/> |
|[Autorisation](permission.md) <br/> |Définit l'accès dont dispose un utilisateur dans un dossier.  <br/> |
|[CalendarPermission](calendarpermission.md) <br/> |Définit l'accès dont dispose un utilisateur dans un dossier de calendrier.  <br/> |
|[UserIds](userids.md) <br/> |Contient un tableau d’utilisateurs délégués à obtenir ou à supprimer de la boîte aux lettres d’un principal.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération AddDelegate](adddelegate-operation.md)
  
[Opération UpdateDelegate](updatedelegate-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)


[Ajout de délégués](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)


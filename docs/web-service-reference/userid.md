---
title: UserId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UserId
api_type:
- schema
ms.assetid: 244af9e0-bf3c-46b4-8bfa-9719a1ed3107
description: L’élément UserId identifie un utilisateur délégué ou un utilisateur qui dispose des autorisations d’accès au dossier.
ms.openlocfilehash: 8e9867f5a8cdd62dd2dae55fbf527595ac14f46d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838957"
---
# <a name="userid"></a>UserId

L’élément **UserId** identifie un utilisateur délégué ou un utilisateur qui dispose des autorisations d’accès au dossier. 
  
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

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[SID](sid.md) <br/> |Représente le formulaire sécurité descripteur definition language (SDDL) de l’identificateur de sécurité (SID).  <br/> |
|[PrimarySmtpAddress](primarysmtpaddress.md) <br/> |Représente l’adresse SMTP Simple Mail Transfer Protocol () principal d’un compte à utiliser pour l’accès délégué.  <br/> |
|[DisplayName (chaîne)](displayname-string.md) <br/> |Définit le nom complet d’un dossier, un contact, une liste de distribution ou un utilisateur délégué.  <br/> |
|[DistinguishedUser](distinguisheduser.md) <br/> |Identifie les comptes d’utilisateurs par défaut et anonymes pour l’accès délégué.  <br/> |
|[ExternalUserIdentity](externaluseridentity.md) <br/> |Identifie un utilisateur délégué externe ou un utilisateur externe qui dispose des autorisations d’accès au dossier.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Utilisateur_délégué](delegateuser.md) <br/> |Identifie un délégué pour ajouter ou mettre à jour dans une boîte aux lettres unique.  <br/> |
|[Autorisation](permission.md) <br/> |Définit l'accès dont dispose un utilisateur dans un dossier.  <br/> |
|[CalendarPermission](calendarpermission.md) <br/> |Définit l'accès dont dispose un utilisateur dans un dossier de calendrier.  <br/> |
|[ID utilisateur](userids.md) <br/> |Contient un tableau d’utilisateurs délégué d’obtenir ou de supprimer la boîte aux lettres d’un utilisateur principal.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération AddDelegate](adddelegate-operation.md)
  
[Opération UpdateDelegate](updatedelegate-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)


[Ajout de délégués](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)


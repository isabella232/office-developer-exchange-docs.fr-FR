---
title: PrimarySmtpAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- PrimarySmtpAddress
api_type:
- schema
ms.assetid: eee79904-9412-4e61-b9b8-aff0ce25fade
description: L’élément PrimarySmtpAddress représente l’adresse SMTP (Simple Mail Transfer Protocol) principale d’un compte à utiliser pour l’autorisation de serveur à serveur ou l’accès délégué.
ms.openlocfilehash: 7963fbc92de88b38da93e577ebd2c39dbedac009
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523873"
---
# <a name="primarysmtpaddress"></a>PrimarySmtpAddress

**L’élément PrimarySmtpAddress** représente l’adresse SMTP (Simple Mail Transfer Protocol) principale d’un compte à utiliser pour l’autorisation de serveur à serveur ou l’accès délégué. 
  
```xml
<PrimarySmtpAddress/>
```

 **PrimarySmtpAddressType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ConnectingSID](connectingsid.md) <br/> |Représente un compte à usurper lorsque vous utilisez l’en-tête SOAP ExchangeImpersonation.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/ExchangeImpersonation/ConnectingSID` <br/> |
|[SerializedSecurityContext](serializedsecuritycontext.md) <br/> |Utilisé dans l’en-tête SOAP pour la sérialisation des jetons dans l’authentification de serveur à serveur.  <br/> |
|[UserId](userid.md) <br/> |Identifie un utilisateur délégué ou un utilisateur qui dispose d’autorisations d’accès aux dossiers.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte qui représente une adresse SMTP est requise.
  
## <a name="remarks"></a>Remarques

Exchange Les services web exigent que les boîtes aux lettres soient identifiées par l’adresse SMTP principale de la boîte aux lettres. Les adresses proxy ou alternatives ne sont pas acceptées.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur exécutant Microsoft Exchange Server 2010 sur qui le rôle serveur d’accès au client est installé.
  
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
  
[Travailler avec l’accès délégué](https://msdn.microsoft.com/library/dfd6b4a3-8fd3-47ba-83c0-52465cb5f3f3%28Office.15%29.aspx)


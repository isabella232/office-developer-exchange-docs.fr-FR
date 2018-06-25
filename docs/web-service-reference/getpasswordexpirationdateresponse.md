---
title: GetPasswordExpirationDateResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3d3fff1f-ef13-46d5-bd7f-ef535eb80c72
description: L’élément GetPasswordExpirationDateResponse définit la réponse à une demande d’opération GetPasswordExpirationDate opération.
ms.openlocfilehash: 3754a53da53c12479f11c2e32cd15a08cba665fb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756714"
---
# <a name="getpasswordexpirationdateresponse"></a>GetPasswordExpirationDateResponse

L’élément **GetPasswordExpirationDateResponse** définit la réponse à une demande d’opération [GetPasswordExpirationDate opération](getpasswordexpirationdate-operation.md) . 
  
- [ResponseMessages](responsemessages.md)
- [GetPasswordExpirationDateResponse](getpasswordexpirationdateresponse.md)
  
```XML
<GetPasswordExpirationDateResponse>
    <PasswordExpirationDate />
</GetPasswordExpirationDateResponse>
```

 **GetPasswordExpirationDateResponseMessageType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**ResponseClass** <br/> | Décrit l’état de la réponse. <br/><br/>Les valeurs suivantes sont valides pour cet attribut :  <br/><br/>-Réussite  <br/>-Avertissement  <br/>-Erreur  <br/> |
   
#### <a name="responseclass-attribute-values"></a>Valeurs des attributs ResponseClass

|**Valeur**|**Description**|
|:-----|:-----|
|**Opération réussie** <br/> |Décrit une demande est remplie.  <br/> |
|**Avertissement** <br/> | Décrit une demande qui n’a pas aboutie. Un message d’avertissement peut être renvoyée si une erreur s’est produite pendant le traite d’un élément dans la demande et les éléments suivants n’ont pas peuvent être traités.<br/><br/> Voici des exemples de sources d’avertissements :  <br/><br/>-La banque d’informations Exchange est en mode hors connexion pendant le traitement par lots.  <br/>-Services de domaine actives Directory (AD DS) est en mode hors connexion.  <br/>-Boîtes aux lettres ont été déplacés.  <br/>-La base de données de message (MDB) est en mode hors connexion.  <br/>-Un mot de passe a expiré.  <br/>-Un quota a été dépassé.  <br/> |
|**Erreur** <br/> | Décrit une demande ne peut pas être traitée. <br/><br/>Voici des exemples de sources d’erreurs :  <br/><br/>-Non valide attributs ou éléments.  <br/>-Les attributs ou les éléments qui sont hors de portée.  <br/>-Une balise inconnue.  <br/>-Un attribut ou un élément qui n’est pas valide dans le contexte.  <br/>-Une tentative d’accès non autorisé par n’importe quel client.  <br/>-Une panne côté serveur en réponse à un appel côté client valid.  <br/><br/>  Vous trouverez plus d’informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Nom de l'élément**|**Description**|
|:-----|:-----|
|[PasswordExpirationDate](passwordexpirationdate.md) <br/> |Fournit la date d’expiration de mot de passe du compte de messagerie spécifiée dans la demande.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Nom de l'élément**|**Description**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Contient les messages de réponse pour une demande d’Exchange Web Services (EWS).  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 2 (SP2).
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération GetPasswordExpirationDate](getpasswordexpirationdate-operation.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)


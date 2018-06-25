---
title: ResolveNamesResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResolveNamesResponseMessage
api_type:
- schema
ms.assetid: edcdaf58-ef63-412e-8c58-409213e6ab0d
description: L’élément ResolveNamesResponseMessage contient l’état et les résultats d’une demande d’opération ResolveNames.
ms.openlocfilehash: 953a1f0b19c078d969ffe175c22df02b58c5e939
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829170"
---
# <a name="resolvenamesresponsemessage"></a>ResolveNamesResponseMessage

L’élément **ResolveNamesResponseMessage** contient l’état et les résultats d’une demande [d’opération ResolveNames](resolvenames-operation.md) . 
  
- [ResolveNamesResponse](resolvenamesresponse.md) 
- [ResponseMessages](responsemessages.md)
- [ResolveNamesResponseMessage](resolvenamesresponsemessage.md)
  
```xml
<ResolveNamesResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <ResolutionSet/>
</ResolveNamesResponseMessage>
```

 **ResolveNamesResponseMessageType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**ResponseClass** <br/> | Décrit l’état d’une réponse de [l’opération ResolveNames](resolvenames-operation.md) . <br/><br/>Les valeurs suivantes sont valides pour cet attribut :  <br/><br/>-Réussite  <br/>-Avertissement  <br/>-Erreur  <br/> |
   
#### <a name="responseclass-attribute"></a>Attribut ResponseClass

|**Valeur**|**Description**|
|:-----|:-----|
|**Opération réussie** <br/> |Décrit une demande est remplie. Cela se produit lorsque le nom demandé est non ambigu et la réponse contient un destinataire unique.  <br/> |
|**Avertissement** <br/> | Décrit une demande qui n’a pas aboutie. Un message d’avertissement peut être renvoyée si une erreur s’est produite pendant le traite d’un élément dans la demande et les éléments suivants n’ont pas peuvent être traités. <br/><br/>Exemple de sources des avertissements sont les suivantes :  <br/><br/>-La banque d’informations Exchange est déconnecté pendant le traitement par lots.  <br/>-Services de domaine actives Directory (AD DS) passe en mode hors connexion.  <br/>-Boîtes aux lettres sont déplacées.  <br/>-La base de données de boîtes aux lettres (MDB) passe en mode hors connexion.  <br/>-Un mot de passe a expiré.  <br/>-Un quota est dépassé.  <br/>-Le nom demandé est ambigu et la réponse contient plusieurs destinataires.  <br/> |
|**Erreur** <br/> | Décrit une demande ne peut pas être traitée. <br/><br/>Voici des exemples de sources d’erreurs :  <br/><br/>-Le nom demandé n’a pas pu être résolu.  <br/>-Attributs ou éléments ne sont pas valides.  <br/>-Attributs ou éléments sont hors de portée.  <br/>-Une balise est inconnue.  <br/>-Un attribut ou un élément n’est pas valide dans le contexte.  <br/>-Une tentative d’accès non autorisés par n’importe quel client s’est produite.  <br/>-Une défaillance du côté serveur s’est produite en réponse à un appel côté client valid.  <br/>  <br/>Vous trouverez plus d’informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |Fournit une description textuelle de l’état de la réponse.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Fournit des informations sur la demande.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |Actuellement inutilisés et est réservé à un usage ultérieur. Il contient une valeur de 0.  <br/> |
|[MessageXml](messagexml.md) <br/> |Fournit des informations de réponse d’erreur.  <br/> |
|[ResolutionSet](resolutionset.md) <br/> |Contient un tableau des résolutions pour un nom ambigu.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Contient les messages de réponse pour une demande de Services Web Exchange.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 ayant le rôle de serveur d’accès au Client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [ResolveNames](resolvenames.md)
- [ResolveNamesResponse](resolvenamesresponse.md)
- [Opération ResolveNames](resolvenames-operation.md)


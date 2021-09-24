---
title: ResolveNamesResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ResolveNamesResponseMessage
api_type:
- schema
ms.assetid: edcdaf58-ef63-412e-8c58-409213e6ab0d
description: L’élément ResolveNamesResponseMessage contient l’état et le résultat d’une demande d’opération ResolveNames.
ms.openlocfilehash: a7debc5f5056ad7a33ebfaf2b0d5d914acdb2397
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523474"
---
# <a name="resolvenamesresponsemessage"></a>ResolveNamesResponseMessage

**L’élément ResolveNamesResponseMessage** contient l’état et le résultat d’une demande d’opération [ResolveNames.](resolvenames-operation.md) 
  
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

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**ResponseClass** <br/> | Décrit l’état d’une [réponse d’opération ResolveNames.](resolvenames-operation.md) <br/><br/>Les valeurs suivantes sont valides pour cet attribut :  <br/><br/>- Réussite  <br/>- Avertissement  <br/>- Erreur  <br/> |
   
#### <a name="responseclass-attribute"></a>Attribut ResponseClass

|**Valeur**|**Description**|
|:-----|:-----|
|**Success** <br/> |Décrit une demande qui est remplie. Cela se produit lorsque le nom demandé n’est pas ambigu et que la réponse contient un seul destinataire.  <br/> |
|**Warning** <br/> | Décrit une demande qui n’a pas été traitée. Un avertissement peut être renvoyé si une erreur s’est produite alors qu’un élément de la demande était en cours de traitement et que les éléments suivants n’ont pas pu être traitées. <br/><br/>Voici un exemple de sources d’avertissements :  <br/><br/>- Le magasin Exchange est hors connexion pendant le lot.  <br/>- Les services de domaine Active Directory (AD DS) sont déconnectés.  <br/>- Les boîtes aux lettres sont déplacées.  <br/>- La base de données de boîtes aux lettres (MDB) est déconnectée.  <br/>- Un mot de passe a expiré.  <br/>- Un quota est dépassé.  <br/>- Le nom demandé est ambigu et la réponse contient plusieurs destinataires.  <br/> |
|**Erreur** <br/> | Décrit une demande qui ne peut pas être remplie. <br/><br/>Voici quelques exemples de sources d’erreurs :  <br/><br/>- Le nom demandé n’a pas pu être résolu.  <br/>- Les attributs ou les éléments ne sont pas valides.  <br/>- Les attributs ou les éléments sont hors de portée.  <br/>- Une balise est inconnue.  <br/>- Attribut ou élément non valide dans le contexte.  <br/>- Une tentative d’accès non autorisé par un client s’est produite.  <br/>- Une défaillance côté serveur s’est produite en réponse à un appel côté client valide.  <br/>  <br/>Des informations sur l’erreur se trouvent dans les éléments [ResponseCode](responsecode.md) et [MessageText.](messagetext.md)  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |Fournit une description textuelle de l’état de la réponse.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Fournit des informations d’erreur sur la demande.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |Actuellement inutilisé et réservé à une utilisation ultérieure. Il contient la valeur 0.  <br/> |
|[MessageXml](messagexml.md) <br/> |Fournit des informations supplémentaires sur la réponse aux erreurs.  <br/> |
|[ResolutionSet](resolutionset.md) <br/> |Contient un tableau de résolutions pour un nom ambigu.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Contient les messages de réponse pour une demande Exchange services Web.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur exécutant Microsoft Exchange Server 2010 sur qui le rôle serveur d’accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [ResolveNames](resolvenames.md)
- [ResolveNamesResponse](resolvenamesresponse.md)
- [Opération ResolveNames](resolvenames-operation.md)


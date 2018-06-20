---
title: ExpandDLResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExpandDLResponseMessage
api_type:
- schema
ms.assetid: 1140601b-98cf-4cb4-a019-321c7f63d5be
description: L’élément ExpandDLResponseMessage contient l’état et les résultats d’une demande d’opération ExpandDL unique.
ms.openlocfilehash: 62a81574f9c513b905a92876b3d757c635b4f07b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756264"
---
# <a name="expanddlresponsemessage"></a>ExpandDLResponseMessage

L’élément **ExpandDLResponseMessage** contient l’état et les résultats d’une seule demande [d’opération ExpandDL](expanddl-operation.md) . 
  
- [ExpandDLResponse](expanddlresponse.md)  
- [ResponseMessages](responsemessages.md) 
- [ExpandDLResponseMessage](expanddlresponsemessage.md)
  
```xml
<ExpandDLResponseMessage ResponseClass="" IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <DLExpansion/>
</ExpandDLResponseMessage>
```

**ExpandDLResponseMessageType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**ResponseClass** <br/> | Décrit l’état d’une réponse de [l’opération ExpandDL](expanddl-operation.md) .<br/><br/>Les valeurs suivantes sont valides pour cet attribut : <br/> <br/>-Réussite  <br/>-Avertissement  <br/>-Erreur  <br/> |
|**IndexedPagingOffset** <br/> |Représente l’index suivant doit être utilisé pour la requête suivante lorsqu’une vue indexée de pagination est utilisée.  <br/> |
|**NumeratorOffset** <br/> |Représente la nouvelle valeur numérateur à utiliser pour la requête suivante lors de la fraction les vues de page sont utilisées.  <br/> |
|**AbsoluteDenominator** <br/> |Représente le dénominateur suivant à utiliser pour la requête suivante lors de la pagination en fraction.  <br/> |
|**IncludesLastItemInRange** <br/> |Indique que le fichier d’échange supplémentaire n’est pas nécessaire. Cet attribut aura la valeur true si le résultat actuel contient le dernier élément dans la requête.  <br/> |
|**TotalItemsInView** <br/> |Représente le nombre total d’éléments qui transmet la restriction.  <br/> |
   
#### <a name="responseclass-attribute-values"></a>Valeurs des attributs ResponseClass

|**Valeur**|**Description**|
|:-----|:-----|
|**Opération réussie** <br/> |Décrit une demande est remplie.  <br/> |
|**Avertissement** <br/> | Décrit une demande qui n’a pas aboutie. Un message d’avertissement peut être renvoyée si une erreur s’est produite pendant le traite d’un élément dans la demande et les éléments suivants n’ont pas peuvent être traités.<br/><br/> Voici des exemples de sources d’avertissements :<br/>  <br/>-La banque d’informations Exchange est en mode hors connexion pendant le traitement par lots.  <br/>-Services de domaine actives Directory (AD DS) est en mode hors connexion.  <br/>-Boîtes aux lettres sont déplacées.  <br/>-La base de données de boîtes aux lettres (MDB) est en mode hors connexion.  <br/>-Un mot de passe a expiré.  <br/>-Un quota a été dépassé.  <br/> |
|**Erreur** <br/> | Décrit une demande ne peut pas être traitée.<br/><br/> Voici des exemples de sources d’erreurs :  <br/><br/>-Non valide attributs ou éléments  <br/>-Attributs ou éléments qui se trouvent en dehors des limites  <br/>-Une balise inconnue  <br/>-Un attribut ou un élément qui n’est pas valide dans le contexte  <br/>-Une tentative d’accès non autorisés par n’importe quel client  <br/>-Une panne côté serveur en réponse à un appel côté client valid <br/> <br/>  Vous trouverez plus d’informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |Fournit une description textuelle de l’état de la réponse.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Fournit un code d’erreur qui identifie l’erreur spécifique qui a rencontré la demande.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |Actuellement inutilisés et est réservé à un usage ultérieur. Il contient une valeur de 0.  <br/> |
|[MessageXml](messagexml.md) <br/> |Fournit des informations de réponse d’erreur.  <br/> |
|[DLExpansion](dlexpansion.md) <br/> |Contient un tableau de boîtes aux lettres qui sont contenus dans une liste de distribution.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Contient les messages de réponse pour une demande de Services Web Exchange.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Exchange Server avec le rôle de serveur d’accès au Client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération ExpandDL](expanddl-operation.md)
- [Référence EWS pour Exchange](ews-reference-for-exchange.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)


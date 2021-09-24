---
title: ExpandDLResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ExpandDLResponseMessage
api_type:
- schema
ms.assetid: 1140601b-98cf-4cb4-a019-321c7f63d5be
description: L’élément ExpandDLResponseMessage contient l’état et le résultat d’une demande d’opération ExpandDL unique.
ms.openlocfilehash: 4683195af3daa462758acbfac4903994818a120e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517069"
---
# <a name="expanddlresponsemessage"></a>ExpandDLResponseMessage

**L’élément ExpandDLResponseMessage** contient l’état et le résultat d’une demande [d’opération ExpandDL](expanddl-operation.md) unique. 
  
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

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**ResponseClass** <br/> | Décrit l’état [d’une réponse d’opération ExpandDL.](expanddl-operation.md)<br/><br/>Les valeurs suivantes sont valides pour cet attribut : <br/> <br/>- Réussite  <br/>- Avertissement  <br/>- Erreur  <br/> |
|**IndexedPagingOffset** <br/> |Représente l’index suivant qui doit être utilisé pour la demande suivante lorsqu’un affichage de pagination indexée est utilisé.  <br/> |
|**NumeratorOffset** <br/> |Représente la nouvelle valeur de numérateur à utiliser pour la demande suivante lorsque des affichages de page de fraction sont utilisés.  <br/> |
|**AbsoluteDenominator** <br/> |Représente le dénominateur suivant à utiliser pour la demande suivante lors de la pagination fractionnaire.  <br/> |
|**IncludesLastItemInRange** <br/> |Indique que la pagination supplémentaire n’est pas nécessaire. Cet attribut aura la valeur true si les résultats actuels contiennent le dernier élément de la requête.  <br/> |
|**TotalItemsInView** <br/> |Représente le nombre total d’éléments qui passent la restriction.  <br/> |
   
#### <a name="responseclass-attribute-values"></a>Valeurs d’attribut ResponseClass

|**Valeur**|**Description**|
|:-----|:-----|
|**Success** <br/> |Décrit une demande qui est remplie.  <br/> |
|**Warning** <br/> | Décrit une demande qui n’a pas été traitée. Un avertissement peut être renvoyé si une erreur s’est produite alors qu’un élément de la demande était en cours de traitement et que les éléments suivants n’ont pas pu être traitées.<br/><br/> Voici quelques exemples de sources d’avertissements :<br/>  <br/>- Le magasin Exchange est hors connexion pendant le lot.  <br/>- Les services de domaine Active Directory (AD DS) sont hors connexion.  <br/>- Les boîtes aux lettres sont déplacées.  <br/>- La base de données de boîtes aux lettres (MDB) est hors connexion.  <br/>- Un mot de passe a expiré.  <br/>- Un quota a été dépassé.  <br/> |
|**Erreur** <br/> | Décrit une demande qui ne peut pas être remplie.<br/><br/> Voici quelques exemples de sources d’erreurs :  <br/><br/>- Attributs ou éléments non valides  <br/>- Attributs ou éléments en dehors de la plage  <br/>- Balise inconnue  <br/>- Attribut ou élément non valide dans le contexte  <br/>- Une tentative d’accès non autorisé par un client  <br/>- Une défaillance côté serveur en réponse à un appel côté client valide <br/> <br/>  Des informations sur l’erreur se trouvent dans les éléments [ResponseCode](responsecode.md) et [MessageText.](messagetext.md)  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |Fournit une description textuelle de l’état de la réponse.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Fournit un code d’erreur qui identifie l’erreur spécifique rencontrée par la demande.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |Actuellement inutilisé et réservé à une utilisation ultérieure. Il contient la valeur 0.  <br/> |
|[MessageXml](messagexml.md) <br/> |Fournit des informations supplémentaires sur la réponse aux erreurs.  <br/> |
|[DLExpansion](dlexpansion.md) <br/> |Contient un tableau de boîtes aux lettres contenues dans une liste de distribution.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Contient les messages de réponse pour une demande Exchange services Web.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Exchange Server avec le rôle serveur d’accès au client installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération ExpandDL](expanddl-operation.md)
- [Référence EWS pour Exchange](ews-reference-for-exchange.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)


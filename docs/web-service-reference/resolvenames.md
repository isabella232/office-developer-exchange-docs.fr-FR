---
title: ResolveNames
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResolveNames
api_type:
- schema
ms.assetid: c85207e1-1315-443b-94ec-2b58f405076b
description: L’élément ResolveNames définit une demande de résolution de noms ambigus.
ms.openlocfilehash: e97b6e78d99cf8ffa3d680907916882d40963f59
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829172"
---
# <a name="resolvenames"></a>ResolveNames

L’élément **ResolveNames** définit une demande de résolution de noms ambigus. 
  
```XML
<ResolveNames ReturnFullContactData="" SearchScope="" ContactDataShape="">
   <ParentFolderIds/>
   <UnresolvedEntry/>
</ResolveNames>
```

 **ResolveNamesType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**ReturnFullContactData** <br/> |Indique si les détails de contact pour les contacts publics pour un nom résolu sont retournés dans la réponse. Cet attribut est requis pour les contacts publics. Cette valeur n’affecte pas les contacts privés et les listes de distribution privée, pour laquelle [ItemId](itemid.md) est toujours renvoyée.  <br/> |
|**SearchScope** <br/> |Identifie le sens et l’étendue de la recherche ResolveNames.  <br/> |
|ContactDataShape  <br/> |Identifie la propriété la valeur renvoyée pour les contacts. Cet attribut est une nouveauté dans Exchange Server 2010 Service Pack 2 (SP2).  <br/> |
   
#### <a name="returnfullcontactdata-attribute-values"></a>Valeurs des attributs ReturnFullContactData

|**Valeur**|**Description**|
|:-----|:-----|
|True  <br/> |Plus d’informations de contacts pour les contacts publics sont renvoyés.  <br/> |
|Faux  <br/> |Plus d’informations de contacts pour les contacts publics ne sont pas renvoyés.  <br/> |
   
#### <a name="searchscope-attribute-values"></a>Valeurs d’attribut SearchScope

|**Valeur**|**Description**|
|:-----|:-----|
|ActiveDirectory  <br/> |Recherche uniquement le service d’annuaire Active Directory est effectuée.  <br/> |
|ActiveDirectoryContacts  <br/> |Active Directory est recherché en premier, puis les dossiers de contacts qui sont spécifiés dans la propriété [ParentFolderIds](parentfolderids.md) sont recherchés.  <br/> |
|Contacts  <br/> |Seuls les dossiers de contacts qui sont identifiés par la propriété [ParentFolderIds](parentfolderids.md) sont recherchés.  <br/> |
|ContactsActiveDirectory  <br/> |Dossiers de contacts qui sont identifiés par la propriété [ParentFolderIds](parentfolderids.md) sont recherchés en premier, et puis Active Directory est recherché.  <br/> |
   
#### <a name="contactdatashape-attribute-values"></a>Valeurs des attributs ContactDataShape

|**Valeur**|**Description**|
|:-----|:-----|
|IdOnly  <br/> |La propriété d’élément de contact identificateur est renvoyée.  <br/> |
|Default (Défaut)  <br/> |L’ensemble par défaut des propriétés de l’élément de contact est renvoyée. Pour plus d’informations, voir [formes réponse dans EWS](http://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx).  <br/> |
|AllProperties  <br/> |L’ensemble de AllProperties des propriétés de l’élément de contact sont renvoyés. Pour plus d’informations, voir [formes réponse dans EWS](http://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx).  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ParentFolderIds](parentfolderids.md) <br/> |Contient un tableau d’identificateurs de dossier de contacts qui doit être recherché si l’attribut **SearchScope** est défini sur ActiveDirectoryContacts, Contacts ou ContactsActiveDirectory. Le tableau ParentFolderIds ne peut contenir qu’un identificateur unique de dossier de contacts. Si l’élément **ParentFolderIds** n’est pas présent, le dossier Contacts par défaut est recherché.  <br/> L’identificateur de dossier peut être utilisé pour l’accès délégué.  <br/> Recherches Active Directory sont effectuées à l’aide de listes de contrôle d’accès (ACL). Certains utilisateurs n’est peut-être pas les droits à voir certains objets Active Directory.  <br/> Cet élément est facultatif.  <br/> |
|[UnresolvedEntry](unresolvedentry.md) <br/> |Contient le nom d’une liste de contacts ou de distribution à résoudre.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération ResolveNames](resolvenames-operation.md)
  
[ResolveNamesType](https://msdn.microsoft.com/library/ExchangeWebServices.ResolveNamesType.aspx)
  
[ResolveNamesSearchScopeType](https://msdn.microsoft.com/library/ExchangeWebServices.ResolveNamesSearchScopeType.aspx)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)


[À l’aide de la résolution de noms](http://msdn.microsoft.com/library/9257fb07-89d2-46eb-b885-e2173fe6fbc1%28Office.15%29.aspx)


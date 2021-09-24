---
title: ResolveNames
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ResolveNames
api_type:
- schema
ms.assetid: c85207e1-1315-443b-94ec-2b58f405076b
description: L’élément ResolveNames définit une demande de résolution de noms ambigus.
ms.openlocfilehash: 8fbf933593b43de656bf8731aa86cc8c8eb76bb4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514143"
---
# <a name="resolvenames"></a>ResolveNames

**L’élément ResolveNames** définit une demande de résolution de noms ambigus. 
  
```XML
<ResolveNames ReturnFullContactData="" SearchScope="" ContactDataShape="">
   <ParentFolderIds/>
   <UnresolvedEntry/>
</ResolveNames>
```

 **ResolveNamesType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**ReturnFullContactData** <br/> |Indique si les coordonnées complètes des contacts publics pour un nom résolu sont renvoyées dans la réponse. Cet attribut est requis pour les contacts publics. Cette valeur n’affecte pas les contacts privés et les listes de distribution privées, pour lesquelles [ItemId](itemid.md) est toujours renvoyé.  <br/> |
|**SearchScope** <br/> |Identifie l’ordre et l’étendue d’une recherche ResolveNames.  <br/> |
|ContactDataShape  <br/> |Identifie le jeu de propriétés renvoyé pour les contacts. Cet attribut a été introduit dans Exchange Server 2010 Service Pack 2 (SP2).  <br/> |
   
#### <a name="returnfullcontactdata-attribute-values"></a>Valeurs d’attribut ReturnFullContactData

|**Valeur**|**Description**|
|:-----|:-----|
|True  <br/> |Les coordonnées complètes des contacts publics sont renvoyées.  <br/> |
|Faux  <br/> |Les coordonnées complètes des contacts publics ne sont pas renvoyées.  <br/> |
   
#### <a name="searchscope-attribute-values"></a>Valeurs d’attribut SearchScope

|**Valeur**|**Description**|
|:-----|:-----|
|ActiveDirectory  <br/> |Seul le service d’annuaire Active Directory est recherché.  <br/> |
|ActiveDirectoryContacts  <br/> |Active Directory est recherché en premier, puis les dossiers de contacts spécifiés dans la [propriété ParentFolderIds](parentfolderids.md) sont recherchés.  <br/> |
|Contacts  <br/> |Seuls les dossiers de contacts identifiés par la [propriété ParentFolderIds](parentfolderids.md) sont recherchés.  <br/> |
|ContactsActiveDirectory  <br/> |Les dossiers de contacts identifiés par la [propriété ParentFolderIds](parentfolderids.md) sont d’abord recherchés, puis Active Directory est recherché.  <br/> |
   
#### <a name="contactdatashape-attribute-values"></a>Valeurs d’attribut ContactDataShape

|**Valeur**|**Description**|
|:-----|:-----|
|IdOnly  <br/> |La propriété d’identificateur de l’élément de contact est renvoyée.  <br/> |
|Par défaut  <br/> |L’ensemble par défaut des propriétés d’élément de contact est renvoyé. Pour plus d’informations, voir [Les formes de réponse dans EWS.](https://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx)  <br/> |
|AllProperties  <br/> |L’ensemble AllProperties des propriétés d’élément de contact est renvoyé. Pour plus d’informations, voir [Les formes de réponse dans EWS.](https://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx)  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ParentFolderIds](parentfolderids.md) <br/> |Contient un tableau d’identificateurs de dossier de contacts qui seraient recherchés si l’attribut **SearchScope** est définie sur ActiveDirectoryContacts, Contacts ou ContactsActiveDirectory. Le tableau ParentFolderIds ne peut contenir qu’un seul identificateur de dossier de contacts. Si **l’élément ParentFolderIds n’est** pas présent, le dossier Contacts par défaut est recherché.  <br/> L’identificateur de dossier peut être utilisé pour l’accès délégué.  <br/> Les recherches Active Directory sont effectuées à l’aide de listes de contrôle d’accès. Certains utilisateurs peuvent ne pas avoir le droit de voir certains objets Active Directory.  <br/> Cet élément est facultatif.  <br/> |
|[UnresolvedEntry](unresolvedentry.md) <br/> |Contient le nom d’un contact ou d’une liste de distribution à résoudre.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération ResolveNames](resolvenames-operation.md)
  
[ResolveNamesType](https://msdn.microsoft.com/library/ExchangeWebServices.ResolveNamesType.aspx)
  
[ResolveNamesSearchScopeType](https://msdn.microsoft.com/library/ExchangeWebServices.ResolveNamesSearchScopeType.aspx)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)


[Utilisation de la résolution de noms](https://msdn.microsoft.com/library/9257fb07-89d2-46eb-b885-e2173fe6fbc1%28Office.15%29.aspx)


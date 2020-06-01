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
ms.openlocfilehash: 9c36a5f84451f91e90a8e7148cf384b5cacd7f29
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467948"
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

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**ReturnFullContactData** <br/> |Indique si les détails du contact complet pour les contacts publics pour un nom résolu sont renvoyés dans la réponse. Cet attribut est requis pour les contacts publics. Cette valeur n’affecte pas les contacts privés et les listes de distribution privées, pour lesquelles [ItemId](itemid.md) est toujours renvoyé.  <br/> |
|**SearchScope** <br/> |Identifie l’ordre et l’étendue d’une recherche ResolveNames.  <br/> |
|ContactDataShape  <br/> |Identifie le jeu de propriétés renvoyé pour les contacts. Cet attribut a été introduit dans Exchange Server 2010 Service Pack 2 (SP2).  <br/> |
   
#### <a name="returnfullcontactdata-attribute-values"></a>Valeurs d’attribut ReturnFullContactData

|**Valeur**|**Description**|
|:-----|:-----|
|True  <br/> |Les détails du contact complet pour les contacts publics sont renvoyés.  <br/> |
|Faux  <br/> |Les détails du contact complet pour les contacts publics ne sont pas renvoyés.  <br/> |
   
#### <a name="searchscope-attribute-values"></a>Valeurs de l’attribut SearchScope

|**Valeur**|**Description**|
|:-----|:-----|
|ActiveDirectory  <br/> |Seul le service d’annuaire Active Directory fait l’objet d’une recherche.  <br/> |
|ActiveDirectoryContacts  <br/> |Active Directory est recherché en premier, puis les dossiers de contacts qui sont spécifiés dans la propriété [ParentFolderIds](parentfolderids.md) sont recherchés.  <br/> |
|Contacts  <br/> |Seuls les dossiers de contacts identifiés par la propriété [ParentFolderIds](parentfolderids.md) sont recherchés.  <br/> |
|ContactsActiveDirectory  <br/> |Les dossiers de contacts identifiés par la propriété [ParentFolderIds](parentfolderids.md) sont recherchés en premier, puis Active Directory est recherché.  <br/> |
   
#### <a name="contactdatashape-attribute-values"></a>Valeurs d’attribut ContactDataShape

|**Valeur**|**Description**|
|:-----|:-----|
|IdOnly  <br/> |La propriété de l’identificateur d’élément de contact est renvoyée.  <br/> |
|Par défaut  <br/> |L’ensemble par défaut des propriétés d’élément de contact est renvoyé. Pour plus d’informations, consultez la rubrique [Shapes Response in EWS](https://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx).  <br/> |
|AllProperties  <br/> |Le jeu AllProperties de propriétés d’élément de contact est renvoyé. Pour plus d’informations, consultez la rubrique [Shapes Response in EWS](https://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx).  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ParentFolderIds](parentfolderids.md) <br/> |Contient un tableau d’identificateurs de dossiers de contacts qui seraient recherchés si l’attribut **SearchScope** est défini sur ActiveDirectoryContacts, contacts ou ContactsActiveDirectory. Le tableau ParentFolderIds ne peut contenir qu’un seul identificateur de dossier de contact. Si l’élément **ParentFolderIds** n’est pas présent, le dossier de contacts par défaut est recherché.  <br/> L’identificateur de dossier peut être utilisé pour l’accès délégué.  <br/> Les recherches Active Directory sont effectuées à l’aide de listes de contrôle d’accès (ACL). Certains utilisateurs ne disposent pas des droits pour afficher certains objets Active Directory.  <br/> Cet élément est facultatif.  <br/> |
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
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération ResolveNames](resolvenames-operation.md)
  
[ResolveNamesType](https://msdn.microsoft.com/library/ExchangeWebServices.ResolveNamesType.aspx)
  
[ResolveNamesSearchScopeType](https://msdn.microsoft.com/library/ExchangeWebServices.ResolveNamesSearchScopeType.aspx)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)


[Utilisation de la résolution de noms](https://msdn.microsoft.com/library/9257fb07-89d2-46eb-b885-e2173fe6fbc1%28Office.15%29.aspx)


---
title: ContactsView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ContactsView
api_type:
- schema
ms.assetid: 8534f44b-a5af-4a9f-9621-23a3eff5f9d8
description: L’élément ContactsView définit une recherche d’éléments de contact en fonction des noms complets alphabétiques.
ms.openlocfilehash: a96da6270d2396e5e82851dcc200f818cec5a7ed
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59531098"
---
# <a name="contactsview"></a>ContactsView

**L’élément ContactsView** définit une recherche d’éléments de contact en fonction des noms complets alphabétiques. 
  
[FindItem](finditem.md)
  
[ContactsView](contactsview.md)
  
```xml
<ContactsView MaxEntriesReturned="" InitialName="" FinalName="" />
```

**ContactsViewType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**MaxEntriesReturned** <br/> |Décrit le nombre maximal de résultats à renvoyer dans la [réponse FindItem.](finditem.md)  <br/> |
|**InitialName** <br/> |Définit le prénom de la liste de contacts à renvoyer dans la réponse. Si le nom initial spécifié ne figure pas dans la liste des contacts, le nom alphabétique suivant, tel que défini par le contexte culturel, est renvoyé, sauf si le nom suivant vient après **FinalName**. Si **l’attribut InitialName** est omis, la réponse contient une liste de contacts qui commence par le prénom dans la liste des contacts. Cet attribut est facultatif.  <br/> |
|**FinalName** <br/> |Définit le nom de famille dans la liste de contacts à renvoyer dans la réponse. Si **l’attribut FinalName** est omis, la réponse contiendra tous les contacts suivants dans l’ordre de tri spécifié. Si le nom final spécifié ne figure pas dans la liste des contacts, le nom alphabétique suivant, tel que défini par le contexte culturel, sera exclu.  <br/><br/>Par exemple, si FinalName="Name », mais que Name ne figure pas dans la liste des contacts, les contacts dont le nom complet est Name1 ou NAME ne seront pas inclus.  <br/><br/>Cet attribut est facultatif.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |Définit une demande de recherche d’éléments dans une boîte aux lettres.<br/><br/> Voici l’expression XPath de cet élément :  <br/>  `/FindItem` <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="example"></a>Exemple

L’exemple de requête suivant montre comment trouver les trois premiers contacts en commençant par le contact dont le nom complet est Kelly Rollin.
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem Traversal="Shallow" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="contacts:DisplayName"/>
        </t:AdditionalProperties>
      </ItemShape>
      <ContactsView MaxEntriesReturned="3" InitialName="Kelly Rollin" />
      <SortOrder>
        <t:FieldOrder Order="Descending">
          <t:FieldURI FieldURI="contacts:DisplayName"/>
        </t:FieldOrder>
        </SortOrder>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="contacts"/>
      </ParentFolderIds>
    </FindItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération FindItem](finditem-operation.md)
- [Recherche d’éléments](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)


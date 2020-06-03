---
title: QueryString (QueryStringType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
api_name:
- QueryString
api_type:
- schema
ms.assetid: cadbf9a5-b87e-4d7f-b488-b76fb0ee7150
description: L’élément QueryString contient une chaîne de requête de boîte aux lettres basée sur la syntaxe de requête avancée (AQS).
localization_priority: Priority
ms.openlocfilehash: eafbbab6de8d191197fb4b80e2b8e3cea80ab800
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459187"
---
# <a name="querystring-querystringtype"></a>QueryString (QueryStringType)

L’élément **QueryString** contient une chaîne de requête de boîte aux lettres basée sur la syntaxe de requête avancée (AQS). 
  
```XML
<QueryString/>
```

 **QueryStringType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|ResetCache  <br/> |Indique que le cache doit être réinitialisé.  <br/> |
|ReturnDeletedItems  <br/> |Indique que les éléments supprimés doivent être renvoyés.  <br/> |
|ReturnHighlightTerms  <br/> |Indique que les termes mis en surbrillance doivent être retournés.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |Définit une requête pour rechercher des éléments dans une boîte aux lettres.  <br/> Voici l’expression XPath de cet élément:/FindItem.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte de l’élément **QueryString** représente une requête de boîte aux lettres effectuée à l’aide d’un sous-ensemble de la [syntaxe de requête avancée (AQS)](https://msdn.microsoft.com/library/aa965711%28VS.85%29.aspx). Pour plus d’informations sur les options de syntaxe prises en charge pour les chaînes de requête, voir la section Notes.
  
## <a name="remarks"></a>Remarques

Dans Exchange Server 2010, cet élément est un type de chaîne de schéma XML. Dans les versions d’Exchange commençant par Exchange Server 2013, y compris Exchange Online, le type de cet élément est **QueryStringType**. Cette modification n’interrompt pas les clients existants, car elle ajoute trois nouveaux attributs facultatifs. 
  
L’élément **QueryString** exclut l’utilisation des restrictions EWS. AQS dans EWS prend en charge trois types de restrictions : la restriction de phase de Word, la restriction de plage de dates et la restriction de type de message. Les tableaux suivants répertorient les propriétés de recherche prises en charge pour chaque type de restriction. 
  
**Restriction de phase de Word**

|**Property**|**Exemple**|**Fonction**|
|:-----|:-----|:-----|
|from  <br/> |De : Dean  <br/> De : « Dean Halstead »  <br/> |Éléments de recherche envoyés par Dean.  <br/> Éléments de recherche envoyés à partir de Dean Halstead. L’expéditeur doit être « Dean Halstead » exactement.  <br/> |
|au  <br/> |À : Dean  <br/> |Éléments de recherche envoyés à Dean.  <br/> |
|cc  <br/> |CC : Dean  <br/> |Recherchez des éléments à l’aide de Dean sur la ligne CC.  <br/> |
|bcc  <br/> |CCI : Dean  <br/> |Recherchez des éléments à l’aide de Dean sur la ligne CCI.  <br/> |
|Participants  <br/> |Participants : Dean  <br/> |Recherchez des éléments à l’aide de Dean dans les champs à, CC ou CCI.  <br/> |
|Subject  <br/> |Subject : Product  <br/> Objet : (développement de produit)  <br/> Objet : « développement de produit »  <br/> |Recherchez des éléments dont le produit est dans l’objet.  <br/> Recherchez des éléments avec Product et Development dans l’objet.  <br/> |
|Corps  <br/> Contenu  <br/> |Corps : progression  <br/> Contenu : progression  <br/> |Recherchez les éléments dont la progression est dans le corps.  <br/> |
|Pièce jointe  <br/> |Pièce jointe : rapport  <br/> |Recherchez des éléments dont le nom de fichier ou le corps du fichier de pièce jointe comporte un rapport.  <br/> |
|(la propriété n’est pas spécifiée)  <br/> |Développement de produits  <br/> |Recherchez des éléments qui contiennent à la fois Product et Development dans toutes les propriétés de phase Word.  <br/> |
   
La correspondance de restriction de phase de mot est toujours insensible à la casse. La restriction de phase de Word prend en charge deux types de correspondance : correspondance de préfixe ou correspondance exacte. La correspondance de préfixe est le comportement de correspondance par défaut. Si vous souhaitez une correspondance exacte, utilisez des guillemets doubles. Par exemple, objet : « produit » correspond à « produit » mais pas à « production » dans l’objet. Plusieurs mots entre guillemets restreignent les phases de mot et leur ordre. Par exemple, « produit Win » correspond uniquement à « produit Win », et non « produit Win95 » ou « produit de Win ». Vous pouvez utiliser un astérisque ( \* ) pour définir une correspondance de préfixe avec une commande restreinte. Par exemple, « Win Product » \* correspond à « Win95 Product », « Windows production line » mais pas « Windows New Product » ou « Product of Win ». Vous pouvez rechercher tous les messages envoyés depuis ou vers un domaine. Par exemple, from : "@hotmail. com" renvoie tous les messages envoyés à partir de hotmail.com.
  
Le tableau suivant décrit les restrictions de plage de dates.
  
**Restriction de plage de dates**

|**Property**|**Exemple**|**Fonction**|
|:-----|:-----|:-----|
|Sent  <br/> |Envoyé : semaine dernière  <br/> Envoyé : 01/01/2001  <br/> Envoyé : 01/01/2001.. 01/15/2001  <br/> |Éléments de recherche envoyés la semaine précédente.  <br/> Éléments de recherche envoyés le 1er janvier 2001.  <br/> Éléments de recherche envoyés entre le 1er janvier 2001 et le 15 janvier 2001.  <br/> |
|Received  <br/> |Date de réception : aujourd’hui  <br/> Reçus : 01/01/2001  <br/> |Éléments de recherche reçus aujourd’hui.  <br/> Éléments de recherche reçus le 1er janvier 2001.  <br/> |
   
Les deux points (..) sont un opérateur de plage. Elle peut être utilisée pour définir une plage avec une date de début et une date de fin. Pour spécifier une date, vous pouvez utiliser des dates relatives. Les dates relatives suivantes sont prises en charge :
  
- Dates relatives : aujourd’hui, demain, hier
    
- Dates relatives à Word : cette semaine, le mois prochain, la semaine dernière, le mois dernier ou l’année à venir
    
- Jours : dimanche, lundi, mardi, mercredi, jeudi, vendredi, samedi
    
- Janvier, février, mars, avril, mai, juin, juillet, août, septembre, octobre, novembre, décembre
    
Le tableau suivant décrit les restrictions de type de message. 
  
**Restriction de type de message**

|**Property**|**Exemple**|**Fonction**|
|:-----|:-----|:-----|
|Kind  <br/> |Type : tâches  <br/> |Rechercher tous les éléments de tâche.  <br/> |
   
AQS dans EWS utilise la propriété **Kind** pour spécifier le type de message. La propriété Kind peut être utilisée avec les types d’éléments suivants : 
  
- email
    
- meetings
    
- tasks
    
- notes
    
- docs
    
- journals
    
- contacts
    
- im
    
Le tableau suivant décrit le regroupement des connecteurs logiques.
  
**Regroupement de connecteurs logiques**

|**Connector**|**Exemple**|**Fonction**|
|:-----|:-----|:-----|
|AND  <br/> |Subject : Product et Subject : Development  <br/> Objet : (produit et développement)  <br/> Objet : (développement de produit)  <br/> |Recherchez des éléments avec produit et développement dans l’objet.  <br/> |
|OR  <br/> |Body : Project ou Body : proposition  <br/> Corps : (projet ou proposition)  <br/> |Rechercher des éléments avec un produit ou un développement dans le corps.  <br/> |
|NOT  <br/> |NOT Body : proposition  <br/> Corps : (pas proposition)  <br/> |Rechercher des messages sans proposition dans le corps.  <br/> |
   
Il s’agit toujours du connecteur par défaut. Par exemple, Subject : Project AND Body : la proposition est identique à Subject : Project Body : proposition. Les connecteurs logiques sont sensibles à la casse. Par exemple, Body : (Project ou proposition) recherche les messages avec « Project », « or » et « proposition » dans le corps au lieu de « Project » ou « proposition ». Le symbole plus (+) équivaut à et. Le symbole de trait d’Union (-) équivaut à NOT. Par exemple, Body : (Project-proposition) recherche les messages avec « Project », mais sans « proposition » dans le corps. 
  
La chaîne de requête peut également contenir des propriétés non indexées pour la recherche. Si la chaîne de requête contient des propriétés non indexées, la recherche peut effectuer une recherche Exchange sur les propriétés indexées et une recherche dans la Banque sur les propriétés non indexées. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="example"></a>Exemple

L’exemple suivant montre une demande de recherche de messages dans la boîte de réception avec Autodiscover dans l’objet.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="1" Offset="0" BasePoint="Beginning" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox" />
      </m:ParentFolderIds>
      <m:QueryString>subject:Autodiscover</m:QueryString>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

L’exemple suivant montre une réponse réussie à la demande.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="20" 
                         Version="Exchange2010" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="1" 
                        TotalItemsInView="5" 
                        IncludesLastItemInRange="false">
            <t:Items>
              <t:Message>
                <t:ItemId Id="AAMkADEzOTExYjJkLTYx" ChangeKey="CQAAABY" />
                <t:Subject>How to use Autodiscover</t:Subject>
              </t:Message>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>

```

## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération FindItem](finditem-operation.md)
  
[Opération FindConversation](findconversation-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)


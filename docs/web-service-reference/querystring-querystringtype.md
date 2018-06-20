---
title: QueryString (QueryStringType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- QueryString
api_type:
- schema
ms.assetid: cadbf9a5-b87e-4d7f-b488-b76fb0ee7150
description: L’élément de la chaîne de requête contient une chaîne de requête de boîte aux lettres basée sur la syntaxe de requête avancée (AQS).
ms.openlocfilehash: 410405638b3f8628dc589049873cfea1f153310c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828943"
---
# <a name="querystring-querystringtype"></a>QueryString (QueryStringType)

L’élément de la **chaîne de requête** contient une chaîne de requête de boîte aux lettres basée sur la syntaxe de requête avancée (AQS). 
  
```XML
<QueryString/>
```

 **QueryStringType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|ResetCache  <br/> |Indique que le cache doit être réinitialisé.  <br/> |
|ReturnDeletedItems  <br/> |Indique que les éléments supprimés doivent être retournées.  <br/> |
|ReturnHighlightTerms  <br/> |Indique que la mise en surbrillance des termes doivent être retournés.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |Définit une requête pour rechercher des éléments dans une boîte aux lettres.  <br/> Voici l’expression XPath pour cet élément : /FindItem.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de texte d’élément **QueryString** représente une requête de boîte aux lettres qui est effectuée à l’aide d’un sous-ensemble de [La syntaxe de requête avancée (AQS)](http://msdn.microsoft.com/en-us/library/aa965711%28VS.85%29.aspx). Voir la section Notes pour plus d’informations sur les options de syntaxe prise en charge pour les chaînes de requête.
  
## <a name="remarks"></a>Remarques

Dans Exchange Server 2010, cet élément est un type de chaîne de schéma XML. Dans les versions d’Exchange commençant par Exchange Server 2013, notamment Exchange Online, le type de cet élément est **QueryStringType**. Cette modification n’arrête pas tous les clients existants, car elle ajoute trois nouveaux attributs facultatifs. 
  
L’élément **QueryString** exclut l’utilisation des restrictions EWS. AQS dans EWS prend en charge trois types de restrictions : word phase restriction, restriction de plage de date et restriction de type de message. Les tableaux suivants répertorient les propriétés de recherche prises en charge pour chaque type de restriction. 
  
**Restriction de phase de Word**

|**Propriété**|**Exemple**|**Fonction**|
|:-----|:-----|:-----|
|from  <br/> |À partir de : Olivier  <br/> À partir de : « Olivier Halstead »  <br/> |Rechercher des éléments envoyés à partir d’Olivier.  <br/> Rechercher des éléments envoyés à partir de Dean Halstead. L’expéditeur doit être exactement « Olivier Halstead ».  <br/> |
|et utilisez à la place  <br/> |À : Olivier  <br/> |Rechercher des éléments envoyés à Olivier.  <br/> |
|cc  <br/> |Cc:Dean  <br/> |Rechercher des éléments avec Olivier sur la ligne Cc.  <br/> |
|bcc  <br/> |Bcc:Dean  <br/> |Rechercher des éléments avec Olivier sur la ligne Cci.  <br/> |
|Participants  <br/> |Participants : Olivier  <br/> |Recherche d’éléments dont l’olivier dans l’à, Cc ou Cci champs.  <br/> |
|Objet  <br/> |Objet : produit  <br/> Objet :(product development)  <br/> Objet : « développement de produit »  <br/> |Rechercher des éléments avec le produit dans l’objet.  <br/> Rechercher des éléments avec des produits et de développement dans l’objet.  <br/> |
|Corps  <br/> Content  <br/> |Corps : progression  <br/> Contenu : progression  <br/> |Rechercher des éléments avec l’avancement dans le corps.  <br/> |
|Pièce jointe  <br/> |Pièce jointe : état  <br/> |Recherche d’éléments dont l’état dans le corps de fichier ou nom de fichier des pièces jointes.  <br/> |
|(la propriété n’est pas spécifiée)  <br/> |Développement de produits  <br/> |Rechercher des éléments qui contiennent des produits et développement dans toutes les propriétés de phase de word.  <br/> |
   
Correspondance de restriction de phase Word est toujours la casse. Restriction de phase Word prend en charge deux types de correspondance : correspondance de préfixe ou correspondance exacte. Correspondance de préfixe est le comportement de correspondance par défaut. Si vous souhaitez une correspondance exacte, utilisez des guillemets doubles. Par exemple, l’objet : « produit » correspond à « produit » mais pas « production » dans l’objet. Plusieurs mots dans des guillemets doubles restreindre les phases de word et leur ordre. Par exemple, « produit win » correspond à la seule « win produit », pas « produit Windows 95 » ou « produit de win ». Vous pouvez utiliser un astérisque (\*) pour définir une correspondance de préfixe avec commande restreints. Par exemple, « win produit »\* correspond à « produit Windows 95 », « ligne de production windows » mais pas « windows nouveau produit » ou « produit de win ». Vous pouvez rechercher tous les messages envoyés à partir d’ou à un domaine. Par exemple, from:"@hotmail.com » renvoie tous les messages envoyés à partir de hotmail.com.
  
Le tableau suivant décrit les restrictions de plage de date.
  
**Restriction de plage de date**

|**Propriété**|**Exemple**|**Fonction**|
|:-----|:-----|:-----|
|Envoyé  <br/> |Envoyés : semaine dernière  <br/> Envoyés : 01/01/2001  <br/> Sent:01/01/2001..01/15/2001  <br/> |Recherche éléments envoyés la semaine dernière.  <br/> Rechercher des éléments envoyés sur le 1er janvier 2001.  <br/> Rechercher des éléments envoyés entre le 1er janvier 2001 et le 15 janvier 2001.  <br/> |
|Received  <br/> |Reçus : aujourd'hui  <br/> Reçus : 01/01/2001  <br/> |Rechercher des éléments reçus dans la journée.  <br/> Rechercher des éléments reçus sur le 1er janvier 2001.  <br/> |
   
Les deux points (.) est un opérateur de plage. Il peut être utilisé pour définir une plage avec un point de départ et une date de fin. Pour spécifier une date, vous pouvez utiliser des dates relatives. Les dates relatives suivantes sont prises en charge :
  
- Dates relatives : aujourd'hui, demain, hier
    
- Expressions de plusieurs dates relatives : cette semaine, le mois prochain, semaine dernière, au-delà de mois ou année
    
- Jours : Dimanche, lundi, mardi, mercredi, jeudi, vendredi, samedi
    
- Janvier, février, mars, avril, mai, juin, juillet, août, septembre, octobre, novembre et décembre
    
Le tableau suivant décrit les restrictions de type de message. 
  
**Restriction de type de message**

|**Propriété**|**Exemple**|**Fonction**|
|:-----|:-----|:-----|
|Type  <br/> |Type : tâches  <br/> |Rechercher tous les éléments de tâche.  <br/> |
   
AQS dans EWS utilise la propriété **Kind** pour spécifier le type de message. La propriété Kind peut être utilisée avec les types d’élément suivants : 
  
- email
    
- réunions
    
- tasks
    
- notes
    
- documents
    
- feuilles
    
- contacts
    
- messagerie instantanée
    
Le tableau suivant décrit le regroupement logiques connecteurs.
  
**Regroupement logiques connecteurs**

|**Connecteur**|**Exemple**|**Fonction**|
|:-----|:-----|:-----|
|AND  <br/> |Objet : produit et subject : développement  <br/> Objet :(product AND development)  <br/> Objet :(product development)  <br/> |Rechercher des éléments avec des produits et de développement dans l’objet.  <br/> |
|OU  <br/> |Corps : projet ou corps : proposition  <br/> Corps :(project OR proposal)  <br/> |Rechercher des éléments avec le produit ou de développement dans le corps.  <br/> |
|NOT  <br/> |PAS de corps : proposition  <br/> Corps :(NOT proposal)  <br/> |Rechercher des messages sans proposition dans le corps.  <br/> |
   
ET est toujours le connecteur par défaut. Par exemple, subject : projet et corps : proposition est le même que le corps : proposition de sujet : projet. Connecteurs logiques respectent la casse. Par exemple, le corps :(project Or proposal) recherche des messages avec « projet », « ou » et « proposition' dans le corps au lieu de « projet » ou « proposition ». Le signe plus (+) est équivalent à and. Le symbole de trait d’union (-) est équivalente à ne pas. Par exemple, le corps :(project-proposal) recherche des messages avec « projet », mais sans 'proposition' dans le corps. 
  
La chaîne de requête peut également contenir les propriétés non indexées pour la recherche. Si la chaîne de requête contient les propriétés non indexées, la recherche peut effectuer une recherche Exchange sur les propriétés indexées et une banque de recherche sur les propriétés non indexées. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="example"></a>Exemple

L’exemple suivant montre une requête pour rechercher des messages dans la boîte de réception avec Autodiscover dans l’objet.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
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

L’exemple suivant montre une réponse positive à la demande.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="20" 
                         Version="Exchange2010" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération FindItem](finditem-operation.md)
  
[FindConversation Operation](findconversation-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)


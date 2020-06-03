---
title: Utiliser des filtres de recherche avec EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 20fc6d2d-41c2-4490-98b8-c52513977fef
description: Découvrez comment utiliser les filtres de recherche avec l’API managée EWS ou EWS dans Exchange.
localization_priority: Priority
ms.openlocfilehash: 04a74ec92d4bced8abd58d164a1c186d6405e679
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455834"
---
# <a name="use-search-filters-with-ews-in-exchange"></a>Utiliser des filtres de recherche avec EWS dans Exchange

Découvrez comment utiliser les filtres de recherche avec l’API managée EWS ou EWS dans Exchange.
  
Les filtres de recherche sont l’outil principal permettant d’exprimer des critères de recherche dans votre API managée EWS ou votre application EWS. Nous vous recommandons d’utiliser des filtres de recherche, par opposition aux [chaînes de requête](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md), pour effectuer les opérations suivantes :
  
- Recherche sur une propriété spécifique ou un ensemble de propriétés.  
- Recherche à l’aide de plusieurs critères de recherche.
    
Les filtres de recherche sont votre seule option si vous effectuez l’une des opérations suivantes :
  
- Recherche de propriétés personnalisées.  
- Effectuer des recherches de chaînes respectant la casse.  
- Exécution des recherches de préfixe ou de correspondance exacte. 
- Effectuer des recherches de masque de masques.
- Recherche des éléments dont la propriété spécifique est définie, quelle que soit la valeur.
- Recherche de dossiers.
- Création de dossiers de recherche.
    
## <a name="determine-what-type-of-search-filter-you-need"></a>Déterminer le type de filtre de recherche dont vous avez besoin
<a name="bk_SelectFilter"> </a>

Avant de créer un filtre de recherche, déterminez d’abord le type de filtre dont vous avez besoin. Les types de filtres sont implémentés en tant que classes descendantes de la classe [unsearchfilter](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter%28v=exchg.80%29.aspx) dans l’API managée EWS et en tant qu’éléments enfants de l’élément [restriction](https://msdn.microsoft.com/library/77f19014-d112-4999-8e83-ecc32a117a73%28Office.15%29.aspx) dans EWS. 
  
**Tableau 1. Types de filtres de recherche**

|**Type de filtre**|**Classe d’API managée EWS**|**Élément EWS**|**Description**|
|:-----|:-----|:-----|:-----|
|Contient un filtre  <br/> |[ContainsSubstring](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.containssubstring%28v=exchg.80%29.aspx) <br/> |[Contains](https://msdn.microsoft.com/library/476d059d-c243-43e9-b475-319fc413ade2%28Office.15%29.aspx) <br/> |Le meilleur type de filtre à utiliser pour les comparaisons de chaînes. Elle vous permet de contrôler le respect de la casse, d’ignorer les espaces blancs et de définir le mode d’imbrication.  <br/> |
|Filtre de masque binaire  <br/> |[ExcludesBitmask](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.excludesbitmask%28v=exchg.80%29.aspx) <br/> |[Exclut](https://msdn.microsoft.com/library/bbaeddf6-9a67-4ee0-af99-7a7a5bbdc0e1%28Office.15%29.aspx) <br/> |Vous permet de rechercher des propriétés entières en tant que masques et de renvoyer uniquement les résultats dont les bits correspondent au masque de bits spécifié non défini.  <br/> |
|Filtre existe  <br/> |[Exists](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.exists%28v=exchg.80%29.aspx) <br/> |[Exists](https://msdn.microsoft.com/library/55d568bd-8dbc-4d50-b9d7-54b74a54d4b5%28Office.15%29.aspx) <br/> |Renvoie tous les éléments pour lesquels la propriété spécifiée est présente, quelle que soit leur valeur.  <br/> |
|Filtre d’égalité  <br/> |[IsEqualTo](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.isequalto%28v=exchg.80%29.aspx) <br/> [IsNotEqualTo](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.isnotequalto%28v=exchg.80%29.aspx) <br/> |[IsEqualTo](https://msdn.microsoft.com/library/48e7e067-049c-4184-8026-071e6f558e8a%28Office.15%29.aspx) <br/> [IsNotEqualTo](https://msdn.microsoft.com/library/e2eff26c-3403-45cd-bb74-1eb98c7dbfcd%28Office.15%29.aspx) <br/> |Compare la valeur de la propriété spécifiée à une valeur de constante spécifiée ou à la valeur d’une autre propriété et renvoie tous les éléments ayant une valeur égale (dans le cas d’un filtre **IsEqualTo** ) ou une valeur non égale (dans le cas d’un filtre **IsNotEqualTo** ).  <br/> |
|Filtre de test relationnel  <br/> |[IsGreaterThan](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.isgreaterthan%28v=exchg.80%29.aspx) <br/> [IsGreaterThanOrEqualTo](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.isgreaterthanorequalto%28v=exchg.80%29.aspx) <br/> [IsLessThan](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.islessthan%28v=exchg.80%29.aspx) <br/> [IsLessThanOrEqualTo](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.islessthanorequalto%28v=exchg.80%29.aspx) <br/> |[IsGreaterThan](https://msdn.microsoft.com/library/a6e9d462-cfa7-40ec-903e-128c95050352%28Office.15%29.aspx) <br/> [IsGreaterThanOrEqualTo](https://msdn.microsoft.com/library/373cc954-314d-40e2-be03-cc08aefc0d5b%28Office.15%29.aspx) <br/> [IsLessThan](https://msdn.microsoft.com/library/2550469b-6e5d-45a5-9ecc-090d1b409296%28Office.15%29.aspx) <br/> [IsLessThanOrEqualTo](https://msdn.microsoft.com/library/b5d85eb2-5e15-4d01-ad49-6289e735ad8a%28Office.15%29.aspx) <br/> |Renvoie tous les éléments qui ont une valeur pour la propriété spécifiée dans la relation appropriée avec une valeur constante spécifiée ou une autre propriété. Par exemple, un filtre **IsGreaterThan** renvoie tous les éléments dont la valeur est supérieure à la valeur spécifiée dans la propriété spécifiée.  <br/> |
|Filtre de négation  <br/> |[Not](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.not%28v=exchg.80%29.aspx) <br/> |[Not](https://msdn.microsoft.com/library/1aa16318-7e90-4b19-bce8-dd1a20a66223%28Office.15%29.aspx) <br/> |Inverse le résultat des autres filtres.  <br/> |
|Filtre composé  <br/> |[Élément searchfiltercollectionpour](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx) <br/> |[And](https://msdn.microsoft.com/library/790246c2-37ad-49a8-91b9-6186d743b011%28Office.15%29.aspx) <br/> [Or](https://msdn.microsoft.com/library/4876d83a-73a3-4953-9d95-3048e6b76ccb%28Office.15%29.aspx) <br/> |Combine plusieurs filtres, ce qui permet d’obtenir des critères de recherche plus complexes.  <br/> |
   
### <a name="contains-filter"></a>Contient un filtre

Un filtre contient est le meilleur choix pour la recherche de propriétés de chaîne. Avec un filtre Contains, vous pouvez contrôler les aspects de la correspondance de chaînes, comme le respect de la casse et le mode de traitement des espaces blancs, en définissant le mode de relation contenant-contenu et le mode de comparaison.
  
#### <a name="contains-filter-in-the-ews-managed-api"></a>Contient un filtre dans l’API managée EWS
<a name="bk_ContainsEWSMA"> </a>

Si vous utilisez l’API managée EWS, vous définissez le mode d’imbrication à l’aide de la propriété [ContainmentMode](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.containssubstring.containmentmode%28v=exchg.80%29.aspx) de la classe [ContainsSubstring](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.containssubstring%28v=exchg.80%29.aspx) et vous définissez le mode de comparaison à l’aide de la propriété [ComparisonMode](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.containssubstring.comparisonmode%28v=exchg.80%29.aspx) de la classe **ContainsSubstring** L’exemple suivant montre comment créer un filtre de recherche qui recherche le champ Subject des éléments pour la sous-chaîne « notes de réunion ». Cet exemple ignore la casse, mais n’ignore pas les espaces blancs. 
  
```cs
// Find all items with a subject that contain the substring
// "meeting notes", regardless of case.
// Matches include:
//   - meeting notes
//   - Meeting Notes
//   - Here are my meeting notes
SearchFilter.ContainsSubstring subjectFilter = new SearchFilter.ContainsSubstring(ItemSchema.Subject,
    "meeting notes", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
```

#### <a name="contains-filter-in-ews"></a>Contient un filtre dans EWS
<a name="bk_ContainsEWSMA"> </a>

Dans EWS, vous définissez le mode de relation contenant-contenu à l’aide de l’attribut **ContainmentMode** de l’élément [Contains](https://msdn.microsoft.com/library/476d059d-c243-43e9-b475-319fc413ade2%28Office.15%29.aspx) , et vous définissez le mode de comparaison à l’aide de l’attribut **ContainmentComparison** de l’élément **Contains** . L’exemple suivant montre comment créer un filtre de recherche pour rechercher le champ Subject des éléments de la sous-chaîne « notes de réunion ». Cet exemple ignore la casse, mais n’ignore pas les espaces blancs. 
  
```XML
<t:Contains ContainmentMode="Substring" ContainmentComparison="IgnoreCase">
  <t:FieldURI FieldURI="item:Subject" />
  <t:Constant Value="meeting notes" />
</t:Contains>
```

### <a name="bitmask-filter"></a>Filtre de masque binaire

Un filtre de masque de bits vous permet de rechercher des propriétés entières en tant que masques et de renvoyer des résultats où des bits spécifiques ne sont pas définis dans la valeur de la propriété spécifiée.
  
#### <a name="bitmask-filter-in-the-ews-managed-api"></a>Filtre de masque de masque dans l’API managée EWS

L’exemple suivant montre comment utiliser l’API managée EWS pour créer un filtre de recherche pour renvoyer tous les éléments ayant une valeur dans la propriété personnalisée **itemIndex** (définie dans la section [exemple : Rechercher des éléments à l’aide d’un filtre de recherche et de l’API managée EWS](#bk_ExampleEWSMA) de cet article) qui n’ont pas le deuxième bit (10 en binaire) défini. 
  
```cs
// Find all items with a value of the custom property that does not
// have the second bit (0010) set.
// Matches include:
//   - Property not set
//   - 1 (0001)
//   - 4 (0100)
//   - 5 (0101)
//   - 8 (1000)
SearchFilter.ExcludesBitmask bit2NotSetFilter = 
    new SearchFilter.ExcludesBitmask(customPropDefinition, 2);
```

#### <a name="bitmask-filter-in-ews"></a>Filtre de masque de masque dans EWS

L’exemple suivant montre comment utiliser EWS pour créer un filtre de recherche pour renvoyer tous les éléments qui ont une valeur dans la propriété personnalisée **itemIndex** (définie dans la section [exemple : Rechercher des éléments à l’aide d’un filtre de recherche et de l’API managée EWS](#bk_ExampleEWSMA) de cet article) qui n’ont pas le deuxième bit (10 en binaire) défini. 
  
```XML
<t:Excludes>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:Bitmask Value="2" />
</t:Excludes>
```

### <a name="exists-filter"></a>Filtre existe

Un filtre Exists vous permet de rechercher des éléments sur lesquels une propriété spécifique est définie, quelle que soit la valeur.
  
#### <a name="exists-filter-in-the-ews-managed-api"></a>Filtre EXISTS dans l’API managée EWS

L’exemple suivant montre comment créer un filtre de recherche pour renvoyer tous les éléments dont la propriété personnalisée **itemIndex** est définie. 
  
```cs
// Find all items that have the custom property set.
SearchFilter.Exists customPropSetFilter =
    new SearchFilter.Exists(customPropDefinition);
```

#### <a name="exists-filter-in-ews"></a>Filtre EXISTS dans EWS

L’exemple suivant montre comment créer un filtre de recherche pour renvoyer tous les éléments dont la propriété personnalisée **itemIndex** est définie. 
  
```XML
<t:Exists>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
</t:Exists>
```

### <a name="equality-filter"></a>Filtre d’égalité

Les filtres d’égalité vous permettent de rechercher tous les éléments dont la valeur de la propriété spécifiée est égale à une valeur spécifique ou qui n’est pas égale à une valeur spécifique. La valeur avec laquelle comparer peut être une valeur constante ou la valeur d’une autre propriété sur chaque élément.
  
#### <a name="equality-filter-in-the-ews-managed-api"></a>Filtre d’égalité dans l’API managée EWS

L’exemple suivant montre comment utiliser l’API managée EWS pour créer un filtre de recherche pour retourner tous les éléments qui n’ont pas été lus.
  
```cs
// Find all items that are not marked as read.
SearchFilter.IsEqualTo unreadFilter =
    new SearchFilter.IsEqualTo(EmailMessageSchema.IsRead, false);
```

L’exemple suivant montre comment créer un filtre de recherche pour renvoyer tous les éléments dont la propriété **itemIndex** est différente de la taille de l’élément. 
  
```cs
// Find all items that are marked as read.
SearchFilter.IsNotEqualTo indexNotEqualToSizeFilter =
    new SearchFilter.IsNotEqualTo(customPropDefinition, ItemSchema.Size);
```

#### <a name="equality-filter-in-ews"></a>Filtre d’égalité dans EWS

L’exemple suivant montre comment utiliser EWS pour créer un filtre de recherche pour retourner tous les éléments qui n’ont pas été lus.
  
```XML
<t:IsEqualTo>
  <t:FieldURI FieldURI="message:IsRead" />
  <t:FieldURIOrConstant>
    <t:Constant Value="false" />
  </t:FieldURIOrConstant>
</t:IsEqualTo>
```

L’exemple suivant montre comment créer un filtre de recherche pour renvoyer tous les éléments dont la propriété **itemIndex** est différente de la taille de l’élément. 
  
```XML
<t:IsNotEqualTo>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:FieldURI FieldURI="item:Size" />
  </t:FieldURIOrConstant>
</t:IsNotEqualTo>
```

### <a name="relational-testing-filter"></a>Filtre de test relationnel

Les filtres de test relationnels vous permettent de rechercher tous les éléments dont la valeur de la propriété spécifiée est supérieure à ( \> ), est supérieur ou égal à ( \> =), inférieur à ( \< ) ou inférieur ou égal à ( \< =) une valeur spécifiée. La valeur avec laquelle comparer peut être une valeur constante ou la valeur d’une autre propriété sur chaque élément.
  
#### <a name="relational-testing-filter-in-the-ews-managed-api"></a>Filtre de test relationnel dans l’API managée EWS

L’exemple suivant montre comment utiliser l’API managée EWS pour créer des filtres de recherche afin de renvoyer tous les éléments avec une valeur de la propriété **itemIndex** qui a la relation spécifiée avec la valeur constante 3. 
  
```cs
// Find all items where the custom property value is > 3.
SearchFilter.IsGreaterThan greaterThanFilter =
    new SearchFilter.IsGreaterThan(customPropDefinition, 3);
// Find all items where the custom property value is >= 3.
SearchFilter.IsGreaterThanOrEqualTo greaterThanOrEqualFilter =
    new SearchFilter.IsGreaterThanOrEqualTo(customPropDefinition, ItemSchema.Size);
// Find all items where the custom property value is < 3.
SearchFilter.IsLessThan lessThanFilter =
    new SearchFilter.IsLessThan(customPropDefinition, 3);
// Find all items where the custom property value is <= 3.
SearchFilter.IsLessThanOrEqualTo lessThanOrEqualFilter =
    new SearchFilter.IsLessThanOrEqualTo(customPropDefinition, 3);
```

#### <a name="relational-testing-filter-in-ews"></a>Filtre de test relationnel dans EWS

L’exemple suivant montre comment utiliser EWS pour créer un filtre de recherche pour renvoyer tous les éléments dont la valeur de la propriété **itemIndex** est supérieure à la valeur de la constante 3. 
  
```XML
<t:IsGreaterThan>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:Constant Value="3" />
  </t:FieldURIOrConstant>
</t:IsGreaterThan>
```

L’exemple suivant montre comment créer un filtre de recherche pour renvoyer tous les éléments dont la valeur de la propriété **itemIndex** est supérieure ou égale à la valeur de la constante 3. 
  
```XML
<t:IsGreaterThanOrEqualTo>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:Constant Value="3" />
  </t:FieldURIOrConstant>
</t:IsGreaterThanOrEqualTo>
```

L’exemple suivant montre comment créer un filtre de recherche pour renvoyer tous les éléments dont la valeur de la propriété **itemIndex** est inférieure à la valeur de constante 3. 
  
```XML
<t:IsLessThan>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:Constant Value="3" />
  </t:FieldURIOrConstant>
</t:IsLessThan>
```

L’exemple suivant montre comment créer un filtre de recherche pour renvoyer tous les éléments dont la valeur de la propriété **itemIndex** est inférieure ou égale à la valeur de la constante 3. 
  
```XML
<t:IsLessThanOrEqualTo>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:Constant Value="3" />
  </t:FieldURIOrConstant>
</t:IsLessThanOrEqualTo>
```

### <a name="negating-filter"></a>Filtre de négation

Un filtre de négation vous permet de nier un autre filtre et d’obtenir les résultats de recherche opposés. Tandis que d’autres filtres renvoient des résultats répondant à des critères spécifiques, un filtre de négation renvoie des résultats qui ne correspondent pas aux critères spécifiés par le filtre auquel il est appliqué.
  
#### <a name="negating-filter-in-the-ews-managed-api"></a>Inversion du filtre dans l’API managée EWS

L’exemple suivant montre comment utiliser l’API managée EWS pour créer un filtre de recherche afin de renvoyer tous les éléments qui n’ont pas la sous-chaîne « notes de réunion » dans l’objet.
  
```cs
SearchFilter.ContainsSubstring subjectFilter = new SearchFilter.ContainsSubstring(ItemSchema.Subject,
    "meeting notes", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
SearchFilter.Not subjectNotFilter =
    new SearchFilter.Not(subjectFilter);
```

#### <a name="negating-filter-in-ews"></a>Inversion du filtre dans EWS

L’exemple suivant montre comment créer un filtre de recherche pour retourner tous les éléments qui n’ont pas la sous-chaîne « notes de réunion » dans l’objet.
  
```XML
<t:Not>
  <t:Contains ContainmentMode="ExactPhrase" ContainmentComparison="IgnoreCase">
    <t:FieldURI FieldURI="item:Subject" />
    <t:Constant Value="meeting notes" />
  </t:Contains>
</t:Not>
```

### <a name="compound-filter"></a>Filtre composé

Un filtre composé vous permet de combiner plusieurs filtres pour créer des critères de recherche plus complexes. Vous pouvez combiner les critères à l’aide des opérateurs logiques et ou ou. De cette manière, vous pouvez effectuer des recherches comme « tous les messages de Sadie Daniels qui contient «notes de réunion » dans l’objet».
  
#### <a name="compound-filter-in-the-ews-managed-api"></a>Filtre composé dans l’API managée EWS

L’exemple suivant montre comment utiliser l’API managée EWS pour créer un filtre de recherche qui renvoie tous les éléments envoyés à partir de Sadie Daniels et qui contiennent « notes de réunion » dans l’objet.
  
```cs
SearchFilter.ContainsSubstring subjectFilter = new SearchFilter.ContainsSubstring(ItemSchema.Subject,
    "meeting notes", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
EmailAddress manager = new EmailAddress("sadie@contoso.com");
SearchFilter.IsEqualTo fromManagerFilter =
    new SearchFilter.IsEqualTo(EmailMessageSchema.Sender, manager);
SearchFilter.SearchFilterCollection compoundFilter =
    new SearchFilter.SearchFilterCollection(LogicalOperator.And, subjectFilter, fromManagerFilter);
```

#### <a name="compound-filter-in-ews"></a>Filtre composé dans EWS

L’exemple suivant montre comment utiliser EWS pour créer un filtre de recherche qui renvoie tous les éléments envoyés à partir de Sadie Daniels et qui contiennent « notes de réunion » dans l’objet.
  
```XML
<t:And>
  <t:Contains ContainmentMode="Substring" ContainmentComparison="IgnoreCase">
    <t:FieldURI FieldURI="item:Subject" />
    <t:Constant Value="meeting notes" />
  </t:Contains>
  <t:IsEqualTo>
    <t:FieldURI FieldURI="message:Sender" />
    <t:FieldURIOrConstant>
      <t:Constant Value="sadie@fourthcoffee.com" />
    </t:FieldURIOrConstant>
  </t:IsEqualTo>
</t:And>
```

## <a name="example-find-items-by-using-a-search-filter-and-the-ews-managed-api"></a>Exemple : Rechercher des éléments à l’aide d’un filtre de recherche et de l’API managée EWS
<a name="bk_ExampleEWSMA"> </a>

Les méthodes d’API managée EWS suivantes utilisent des filtres de recherche :
  
- [ExchangeService. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
- [ExchangeService. FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)
- [Folder. FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)
- [Folder. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
L’exemple suivant utilise la méthode **ExchangeService. FindItems** ; Toutefois, les mêmes règles et concepts s’appliquent à toutes les méthodes. Dans cet exemple, une méthode appelée **SearchWithFilter** est définie. Il utilise un objet [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , un objet [WellKnownFolderName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) et un objet [unsearchfilter](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter%28v=exchg.80%29.aspx) comme paramètres. Cet exemple part du principe que l’objet **ExchangeService** a été initialisé avec des valeurs valides dans les [informations d’identification](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) et les propriétés de l' [URL](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) . La classe **unsearchfilter** est la classe de base pour tous les différents filtres de recherche. 
  
```cs
using Microsoft.Exchange.WebServices.Data
private static Guid SearchTestGUID = new Guid("{AA3DF801-4FC7-401F-BBC1-7C93D6498C2E}");
private static ExtendedPropertyDefinition customPropDefinition =
        new ExtendedPropertyDefinition(SearchTestGUID, "ItemIndex", MapiPropertyType.Integer);
static void SearchWithFilter(ExchangeService service, WellKnownFolderName folder, SearchFilter filter)
{
    // Limit the result set to 10 items.
    ItemView view = new ItemView(10);
    view.PropertySet = new PropertySet(ItemSchema.Subject, 
                                       ItemSchema.DateTimeReceived,
                                       EmailMessageSchema.IsRead,
                                       customPropDefinition);
    // Item searches do not support Deep traversal.
    view.Traversal = ItemTraversal.Shallow;
    // Sorting.
    view.OrderBy.Add(ItemSchema.DateTimeReceived, SortDirection.Descending);
    try
    {
        FindItemsResults<Item> results = service.FindItems(folder, filter, view);
        foreach (Item item in results.Items)
        {
            Console.WriteLine("Subject: {0}", item.Subject);
            Console.WriteLine("Id: {0}", item.Id.ToString());
            if (item.ExtendedProperties.Count > 0 &&
                 item.ExtendedProperties[0].PropertyDefinition == customPropDefinition)
            {
                Console.WriteLine("Search Index: {0}", item.ExtendedProperties[0].Value);
            }
            if (item is EmailMessage)
            {
                EmailMessage message = item as EmailMessage;
                Console.WriteLine("Read: {0}", message.IsRead.ToString());
            }
        }
    }
    catch (Exception ex)
    {
        Console.WriteLine("Exception while enumerating results: {0}", ex.Message);
    }
}
```

Vous pouvez utiliser cette fonction avec n’importe quel filtre de recherche présenté dans les exemples de cet article. Cet exemple utilise un filtre composé pour renvoyer tous les éléments de la boîte de réception à partir de Sadie Daniels avec « notes de réunion » dans l’objet.
  
```cs
SearchFilter.ContainsSubstring subjectFilter = new SearchFilter.ContainsSubstring(ItemSchema.Subject,
    "meeting notes", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
EmailAddress manager = new EmailAddress("sadie@contoso.com");
SearchFilter.IsEqualTo fromManagerFilter =
    new SearchFilter.IsEqualTo(EmailMessageSchema.Sender, manager);
SearchFilter.SearchFilterCollection compoundFilter =
    new SearchFilter.SearchFilterCollection(LogicalOperator.And, subjectFilter, greaterThanFilter);
SearchWithFilter(service, WellKnownFolderName.Inbox, compoundFilter);
```

## <a name="example-find-an-item-by-using-a-search-filter-and-ews"></a>Exemple : Rechercher un élément à l’aide d’un filtre de recherche et EWS
<a name="bk_ExampleEWS"> </a>

Les opérations EWS suivantes utilisent des filtres de recherche :
  
- [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
- [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    
L’exemple suivant utilise l’opération **FindItem** ; Toutefois, les mêmes règles et concepts s’appliquent aux deux opérations. Les filtres de recherche sont contenus dans l’élément de [restriction](https://msdn.microsoft.com/library/77f19014-d112-4999-8e83-ecc32a117a73%28Office.15%29.aspx) dans les demandes SOAP. Cet exemple envoie une demande SOAP équivalente à la recherche illustrée dans l’exemple d’API managée EWS précédent. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="item:DateTimeReceived" />
          <t:FieldURI FieldURI="message:IsRead" />
          <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="10" Offset="0" BasePoint="Beginning" />
      <m:Restriction>
        <t:And>
          <t:Contains ContainmentMode="Substring" ContainmentComparison="IgnoreCase">
            <t:FieldURI FieldURI="item:Subject" />
            <t:Constant Value="meeting notes" />
          </t:Contains>
          <t:IsEqualTo>
            <t:FieldURI FieldURI="message:Sender" />
            <t:FieldURIOrConstant>
              <t:Constant Value="sadie@contoso.com" />
            </t:FieldURIOrConstant>
          </t:IsEqualTo>
        </t:And>
      </m:Restriction>
      <m:SortOrder>
        <t:FieldOrder Order="Descending">
          <t:FieldURI FieldURI="item:DateTimeReceived" />
        </t:FieldOrder>
      </m:SortOrder>
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

L’exemple suivant montre la réponse du serveur, y compris les résultats de la recherche.
  
```XML
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="712" MinorBuildNumber="22" Version="V2_3" 
        xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="3" TotalItemsInView="3" IncludesLastItemInRange="true">
            <t:Items>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>meeting notes</t:Subject>
                <t:DateTimeReceived>2013-11-20T21:18:51Z</t:DateTimeReceived>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
                  <t:Value>5</t:Value>
                </t:ExtendedProperty>
                <t:IsRead>true</t:IsRead>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>Meeting Notes</t:Subject>
                <t:DateTimeReceived>2013-11-20T21:18:51Z</t:DateTimeReceived>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
                  <t:Value>6</t:Value>
                </t:ExtendedProperty>
                <t:IsRead>true</t:IsRead>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>Meeting notes</t:Subject>
                <t:DateTimeReceived>2013-11-20T21:18:51Z</t:DateTimeReceived>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
                  <t:Value>7</t:Value>
                </t:ExtendedProperty>
                <t:IsRead>true</t:IsRead>
              </t:Message>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="next-steps"></a>Étapes suivantes
<a name="bk_ExampleEWS"> </a>

Maintenant que vous êtes familiarisé avec l’utilisation des filtres de recherche dans les recherches de base, vous pouvez passer à des techniques de recherche plus avancées.
  
- [Effectuer des recherches groupées à l’aide d’EWS dans Exchange](how-to-perform-grouped-searches-by-using-ews-in-exchange.md)
    
- [Effectuer des recherches paginées à l’aide d’EWS dans Exchange](how-to-perform-paged-searches-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>Voir aussi

- [Recherche et EWS dans Exchange](search-and-ews-in-exchange.md)    
- [Effectuer une recherche AQS à l’aide d’EWS dans Exchange](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md)   
- [ExchangeService. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)    
- [ExchangeService. FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)    
- [Folder. FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)    
- [Folder. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)    
- [Opération FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)   
- [Opération FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    


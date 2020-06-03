---
title: ExtendedFieldURI
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExtendedFieldURI
api_type:
- schema
ms.assetid: b3c6ea3a-9ead-44b9-9d99-64ecf12bde23
description: L’élément ExtendedFieldURI identifie une propriété MAPI étendue.
ms.openlocfilehash: fd365010016c68236107991717ed538c97dc0d50
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526031"
---
# <a name="extendedfielduri"></a>ExtendedFieldURI

L’élément **ExtendedFieldURI** identifie une propriété MAPI étendue. 
  
```xml
<ExtendedFieldURI DistinguishedPropertySetId="" PropertySetId="" PropertyTag="" PropertyName="" PropertyId="" PropertyType="" />
```

**PathToExtendedFieldType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**DistinguishedPropertySetId** <br/> |Définit les ID des jeux de propriétés connus pour les propriétés MAPI étendues.<br/><br/>Si cet attribut est utilisé, les attributs **PropertySetId** et **PropertyTag** ne peuvent pas être utilisés. Cet attribut doit être utilisé avec l’attribut **PropertyId** ou **PropertyName** et l’attribut **PropertyType** .<br/><br/>La table d’attributs **DistinguishedPropertySetId** plus loin dans cette rubrique répertorie les valeurs possibles pour cet attribut.<br/><br/>Cet attribut est facultatif.  <br/> |
|**PropertySetId** <br/> |Identifie un jeu de propriétés étendues MAPI ou un espace de noms par son GUID d’identification.<br/><br/>Si cet attribut est utilisé, l’attribut **DistinguishedPropertySetId** et **PropertyTag** ne peut pas être utilisé. Cet attribut doit être utilisé avec l’attribut **PropertyId** ou **PropertyName** et l’attribut **PropertyType** .<br/><br/>Cet attribut est facultatif.  <br/> |
|**PropertyTag** <br/> |Identifie la balise de propriété sans la partie type de la balise. Le **PropertyTag** peut être représenté sous la forme d’un nombre entier hexadécimal ou court.<br/><br/>La plage comprise entre 0x8000 et 0xFFFE représente la plage de propriétés personnalisée. Lorsqu’une base de données de boîtes aux lettres rencontre une propriété personnalisée pour la première fois, elle affecte cette propriété personnalisée à une balise de propriété dans la plage de propriétés personnalisées de 0x8000-0xFFFE. Une balise de propriété personnalisée donnée est vraisemblablement différente d’une base de données à l’autres. Par conséquent, une requête de propriété personnalisée par balise de propriété peut renvoyer des propriétés différentes sur différentes bases de données. L’utilisation de l’attribut **PropertyTag** est interdite pour les propriétés personnalisées. À la place, utilisez l’attribut **PropertySetId** et l’attribut **PropertyName** ou **PropertyId** .<br/><br/>**Important**: accédez à n’importe quelle propriété personnalisée entre 0X8000 et 0xFFFE en utilisant le GUID + nom/ID. Si l’attribut **PropertyTag** est utilisé, les **attributs DistinguishedPropertySetId**, **PropertySetId**, **PropertyName**et **PropertyId** ne peuvent pas être utilisés.<br/><br/>Cet attribut est facultatif.<br/><br/>**Remarque**: vous ne pouvez pas utiliser un attribut de balise de propriété pour les propriétés au sein de la plage personnalisée 0X8000-0xFFFE. Dans ce cas, vous devez utiliser une propriété nommée.           |
|**PropertyName** <br/> |Identifie une propriété étendue par son nom. Cette propriété doit être associée à **DistinguishedPropertySetId** ou **PropertySetId**.<br/><br/>Si cet attribut est utilisé, les attributs **PropertyId** et **PropertyTag** ne peuvent pas être utilisés.<br/><br/>Cet attribut est facultatif.  <br/> |
|**PropertyId** <br/> |Identifie une propriété étendue par son ID de dispatch. L’ID de répartition peut être identifié dans des formats décimaux ou hexadécimaux. Cette propriété doit être associée à **DistinguishedPropertySetId** ou **PropertySetId**.<br/><br/>Si cet attribut est utilisé, les attributs **PropertyName** et **PropertyTag** ne peuvent pas être utilisés.<br/><br/>Cet attribut est facultatif.  <br/> |
|**PropertyType** <br/> |Représente le type de propriété d’une balise de propriété. Cela correspond au mot le moins significatif dans une balise de propriété.<br/><br/>La table d’attributs PropertyType plus loin dans cette rubrique contient les valeurs possibles pour cet attribut.<br/><br/>Cet attribut est obligatoire.  <br/> |
   
#### <a name="distinguishedpropertysetid-attribute"></a>Attribut DistinguishedPropertySetId

|**Valeur**|**Description**|
|:-----|:-----|
|Adresse  <br/> |Identifie l’ID de jeu de propriétés d’adresse par son nom.  <br/> |
|Rendez-vous  <br/> |Identifie l’ID de jeu de propriétés de rendez-vous par son nom.  <br/> |
|CalendarAssistant  <br/> |Identifie l’ID de jeu de propriétés de l’Assistant calendrier par son nom.  <br/> |
|Courant  <br/> |Identifie l’ID de jeu de propriétés commun par son nom.  <br/> |
|InternetHeaders  <br/> |Identifie l’ID de jeu de propriétés des en-têtes Internet par son nom.  <br/> |
|Satisfaire  <br/> |Identifie l’ID du jeu de propriétés de la réunion par son nom.  <br/> |
|Partage  <br/> | <br/> |
|PublicStrings  <br/> |Identifie l’ID de jeu de propriétés de chaînes publiques par son nom.  <br/> |
|Tâche  <br/> |Identifie l’ID de jeu de propriétés de la tâche par son nom.  <br/> |
|UnifiedMessaging  <br/> |Identifie l’ID de jeu de propriétés de messagerie unifiée par son nom.  <br/> |
   
#### <a name="propertytype-attribute"></a>PropertyType, attribut

|**Valeur**|**Description**|
|:-----|:-----|
|ApplicationTime  <br/> |Valeur de type double interprétée comme une date et une heure. Le composant entier est la date et la fraction le temps.  <br/> |
|ApplicationTimeArray  <br/> |Tableau de valeurs de type double qui sont interprétées comme une date et une heure.  <br/> |
|Binaire  <br/> |Valeur binaire codée en base64.  <br/> |
|BinaryArray  <br/> |Tableau de valeurs binaires codées en base64.  <br/> |
|Valeur booléenne  <br/> |Valeur booléenne **true** ou **false**.  <br/> |
|CLSID  <br/> |Chaîne de GUID.  <br/> |
|CLSIDArray  <br/> |Tableau de chaînes GUID.  <br/> |
|Devise  <br/> |Entier 64 bits qui est interprété comme le nombre de cents.  <br/> |
|CurrencyArray  <br/> |Tableau d’entiers 64 bits qui sont interprétés comme le nombre de cents.  <br/> |
|Double  <br/> |Valeur à virgule flottante 64 bits.  <br/> |
|DoubleArray  <br/> |Tableau de valeurs à virgule flottante 64 bits.  <br/> |
|Erreur  <br/> |Valeur SCODE ; entier non signé 32 bits.  <br/> Non utilisé pour les restrictions ou pour l’obtention ou la définition des valeurs. Ceci n’existe que pour la création de rapports.  <br/> |
|Flottant  <br/> |Valeur à virgule flottante 32 bits.  <br/> |
|FloatArray  <br/> |Tableau de valeurs à virgule flottante 32 bits.  <br/> |
|Entier  <br/> |Entier signé 32 bits (Int32).  <br/> |
|IntegerArray  <br/> |Tableau d’entiers 32 bits (Int32) signés.  <br/> |
|Entier long  <br/> |Entier de 64 bits (Int64) signé ou non signé.  <br/> |
|LongArray  <br/> |Tableau de nombres entiers signés ou non signés 64 bits (Int64).  <br/> |
|Null  <br/> |Indique qu’aucune valeur de propriété n’est ajoutée.  <br/> Non utilisé pour les restrictions ou pour l’obtention ou la définition des valeurs. Ceci n’existe que pour la création de rapports.  <br/> |
|Objet  <br/> |Pointeur vers un objet qui implémente l’interface IUnknown.  <br/> Non utilisé pour les restrictions ou pour l’obtention ou la définition des valeurs. Ceci n’existe que pour la création de rapports.  <br/> |
|ObjectArray  <br/> |Tableau de pointeurs vers des objets qui implémentent l’interface IUnknown.  <br/> Non utilisé pour les restrictions ou pour l’obtention ou la définition des valeurs. Ceci n’existe que pour la création de rapports.  <br/> |
|Nom court  <br/> |Entier signé 16 bits.  <br/> |
|ShortArray  <br/> |Tableau d’entiers 16 bits signés.  <br/> |
|SystemTime  <br/> |Valeur d’heure et de données entières 64 bits sous la forme d’une structure FILETIME.  <br/> |
|SystemTimeArray  <br/> |Tableau de valeurs de données de type Integer 64 bits et d’heures sous la forme d’une structure FILETIME.  <br/> |
|Chaîne  <br/> |Chaîne Unicode.  <br/> |
|StringArray  <br/> |Tableau de chaînes Unicode.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ExtendedProperty](extendedproperty.md) <br/> |Identifie les propriétés étendues sur les dossiers et les éléments.  <br/> |
|[AdditionalProperties](additionalproperties.md) <br/> | Identifie les propriétés supplémentaires.<br/><br/>Voici les expressions XPath de cet élément :<br/><br/>`/FindFolder/FolderShape/AdditionalProperties` <br/>  `/GetFolder/FolderShape/AdditionalProperties` <br/>  `/SyncFolderHierarchy/FolderShape/AdditionalProperties` <br/>  `/GetItem/ItemShape/AdditionalProperties` <br/>  `/FindItem/ItemShape/AdditionalProperties` <br/>  `/SyncFolderItems/ItemShape/AdditionalProperties` <br/>  `/GetAttachment/AttachmentShape/AdditionalProperties` <br/> |
|[SetItemField](setitemfield.md) <br/> |Représente une mise à jour d'une propriété unique d'un élément dans une [UpdateItem Operation](updateitem-operation.md).  <br/> |
|[SetFolderField](setfolderfield.md) <br/> |Représente une mise à jour d’une propriété unique sur un dossier dans une [opération UpdateFolder](updatefolder-operation.md).  <br/> |
|[DeleteItemField](deleteitemfield.md) <br/> |Représente une opération de suppression pour la suppression d’une propriété donnée d’un élément au cours d’une [opération UpdateItem](updateitem-operation.md).  <br/> |
|[DeleteFolderField](deletefolderfield.md) <br/> |Représente une opération de suppression pour la suppression d’une propriété donnée d’un dossier lors d’un appel UpdateFolder.  <br/> |
|[AppendToItemField](appendtoitemfield.md) <br/> |Identifie les données à ajouter à une propriété unique d’un élément au cours d’une [opération UpdateItem](updateitem-operation.md).  <br/> |
|[AppendToFolderField](appendtofolderfield.md) <br/> |Spécifie les données à ajouter à une propriété de dossier lors d’une [opération UpdateFolder](updatefolder-operation.md).  <br/> |
|[Exists](exists.md) <br/> |Représente une expression de recherche qui renvoie la **valeur true** si la propriété fournie existe sur un élément.  <br/> |
|[FieldURIOrConstant](fielduriorconstant.md) <br/> |Représente une propriété ou une valeur constante à utiliser lors de la comparaison avec une autre propriété.  <br/> |
|[IsEqualTo](isequalto.md) <br/> |Représente une expression de recherche qui compare une propriété à une valeur de constante ou à une autre propriété et donne la **valeur true** si elles sont égales.  <br/> |
|[IsGreaterThan](isgreaterthan.md) <br/> |Représente une expression de recherche qui compare une propriété avec une valeur de constante ou une autre propriété et renvoie la **valeur true** si la première propriété est supérieure.  <br/> |
|[IsGreaterThanOrEqualTo](isgreaterthanorequalto.md) <br/> |Représente une expression de recherche qui compare une propriété avec une valeur de constante ou une autre propriété et renvoie la **valeur true** si la première propriété est supérieure ou égale à la seconde.  <br/> |
|[IsLessThan](islessthan.md) <br/> |Représente une expression de recherche qui compare une propriété avec une constante ou une autre propriété et renvoie la **valeur true** si la première propriété est inférieure à la seconde.  <br/> |
|[IsLessThanOrEqualTo](islessthanorequalto.md) <br/> |Représente une expression de recherche qui compare une propriété avec une constante ou une autre propriété et renvoie la **valeur true** si la première propriété est inférieure à la seconde.  <br/> |
|[IsNotEqualTo](isnotequalto.md) <br/> |Représente une expression de recherche qui compare une propriété à une valeur de constante ou à une autre propriété et renvoie la **valeur true** si les valeurs ne sont pas identiques.  <br/> |
|[Exclut](excludes.md) <br/> |Effectue un masque de bits des propriétés.  <br/> |
|[Contains](contains.md) <br/> |Représente une expression de recherche qui détermine si une propriété donnée contient la valeur de chaîne de constante fournie.  <br/> |
|[FieldOrder](fieldorder.md) <br/> |Représente un champ unique par lequel trier les résultats et indique le sens du tri.  <br/> |
   
## <a name="remarks"></a>Remarques

Certains attributs ne peuvent pas être utilisés en combinaison avec d’autres attributs. Toute demande entrant dans une combinaison incorrecte d’attributs de propriété étendues génère un message d’erreur.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
> [!NOTE]
> Dans Microsoft .NET, un type long est un entier signé de 64 bits, tandis que dans MAPI et COM, un type long est un entier 32 bits. La plupart des développeurs utiliseront l’infrastructure Microsoft.NET pour développer des applications clientes de services Web Exchange. Par conséquent, l’affectation de noms .NET est utilisée à la place de l’appellation MAPI.
> 
> Par exemple, la propriété MAPI PR_MESSAGE_FLAGS, 0x0E07, est un \_ type PT long. Dans .NET, il est considéré comme un nombre entier. Une propriété étendue pour PR_MESSAGE_FLAGS est définie en tant que `<t:ExtendedFieldURI PropertyTag="0x0E07" PropertyType="Integer"/>` . 
  
## <a name="example"></a>Exemple

L’exemple suivant de requête crée un élément qui a deux propriétés personnalisées. La première propriété personnalisée est nommée **IsMyHouse** avec une valeur booléenne définie sur **true**. La deuxième propriété étendue personnalisée est nommée **HousePrices**. Elle contient un tableau de valeurs monétaires. 
  
```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" 
                  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
    MessageDisposition="SaveOnly">
      <SavedItemFolderId>
        <t:DistinguishedFolderId Id="inbox"/>
      </SavedItemFolderId>
      <Items>
        <t:Item>
          <t:ItemClass>IPM.Note</t:ItemClass>
          <t:Subject>Create an extended property</t:Subject>
          <t:Body BodyType="Text">Added info to extended props</t:Body>
          <t:ExtendedProperty>
            <t:ExtendedFieldURI DistinguishedPropertySetId="PublicStrings" 
                                PropertyName="IsMyHouse" 
                                PropertyType="Boolean"/>
            <t:Value>true</t:Value>
          </t:ExtendedProperty>
          <t:ExtendedProperty>
            <t:ExtendedFieldURI DistinguishedPropertySetId="PublicStrings" 
                                PropertyName="HousePrices" 
                                PropertyType="CurrencyArray"/>
            <t:Values>
              <t:Value>30000000</t:Value>
              <t:Value>40000000</t:Value>
              <t:Value>50000000</t:Value>
            </t:Values>
          </t:ExtendedProperty>
        </t:Item>
      </Items>
    </CreateItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [FieldURI](fielduri.md)
- [IndexedFieldURI](indexedfielduri.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)


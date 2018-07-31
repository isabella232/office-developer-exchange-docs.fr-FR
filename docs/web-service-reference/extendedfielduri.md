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
ms.openlocfilehash: 50ce46652863b0c534d09d58d4b9f7c8095deef2
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353790"
---
# <a name="extendedfielduri"></a>ExtendedFieldURI

L’élément **ExtendedFieldURI** identifie une propriété MAPI étendue. 
  
```xml
<ExtendedFieldURI DistinguishedPropertySetId="" PropertySetId="" PropertyTag="" PropertyName="" PropertyId="" PropertyType="" />
```

**PathToExtendedFieldType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**DistinguishedPropertySetId** <br/> |Définit le connu propriété définie des ID pour les propriétés MAPI étendues.<br/><br/>Si cet attribut est utilisé, les attributs **PropertySetId** et **PropertyTag** ne peut pas être utilisés. Cet attribut doit être utilisé avec le **PropertyName** **PropertyId** ou attribut et l’attribut **PropertyType** .<br/><br/>La table d’attributs **DistinguishedPropertySetId** plus loin dans cette rubrique répertorie les valeurs possibles de cet attribut.<br/><br/>Cet attribut est facultatif.  <br/> |
|**PropertySetId** <br/> |Identifie une MAPI étendue du jeu de propriétés ou d’espace de noms par son GUID identifiant.<br/><br/>Si cet attribut est utilisé, l’attribut **DistinguishedPropertySetId** et **PropertyTag** ne peut pas être utilisé. Cet attribut doit être utilisé avec le **PropertyName** **PropertyId** ou attribut et l’attribut **PropertyType** .<br/><br/>Cet attribut est facultatif.  <br/> |
|**PropertyTag** <br/> |Identifie la balise de propriété sans le composant de type de la balise. La **PropertyTag** peut être représenté comme un hexadécimal ou un entier court.<br/><br/>Comprise entre 0 x 8000 et 0xFFFE représente la plage de propriétés personnalisée. Lorsqu’une base de données de boîtes aux lettres rencontre une propriété personnalisée pour la première fois, il assigne propriété personnalisée à une balise de propriété au sein de la plage de la propriété personnalisée de 0 x 8000-0xFFFE. Une balise de propriété personnalisée donnée probablement diffèrent entre les bases de données. Par conséquent, une demande de propriété personnalisée à la balise de propriété peut renvoyer des propriétés différentes sur différentes bases de données. L’utilisation de l’attribut **PropertyTag** est interdite pour les propriétés personnalisées. Au lieu de cela, utilisez l’attribut **PropertySetId** et l’attribut **PropertyName** ou **PropertyId** .<br/><br/>**IMPORTANT**: accéder à n’importe quelle propriété personnalisée entre 0 x 8000 et 0xFFFE en utilisant le GUID + nom/ID. Si l’attribut **PropertyTag** est utilisé, les attributs **DistinguishedPropertySetId**, **PropertySetId**, **PropertyName**et **PropertyId** ne peut pas être utilisés.<br/><br/>Cet attribut est facultatif.<br/><br/>**Remarque**: vous ne pouvez pas utiliser un attribut de balise de propriété pour les propriétés dans la plage 0 x 8000-0xFFFE personnalisée. Vous devez utiliser une propriété nommée dans ce cas.           |
|**PropertyName** <br/> |Identifie une propriété étendue par son nom. Cette propriété doit être associée à le **DistinguishedPropertySetId** ou **PropertySetId**.<br/><br/>Si cet attribut est utilisé, les attributs **PropertyId** et **PropertyTag** ne peut pas être utilisés.<br/><br/>Cet attribut est facultatif.  <br/> |
|**PropertyId** <br/> |Identifie une propriété étendue par son ID de répartition. L’ID de répartition peut être identifié au format décimal ou hexadécimal. Cette propriété doit être associée à le **DistinguishedPropertySetId** ou **PropertySetId**.<br/><br/>Si cet attribut est utilisé, les attributs **PropertyName** et **PropertyTag** ne peut pas être utilisés.<br/><br/>Cet attribut est facultatif.  <br/> |
|**PropertyType** <br/> |Représente le type de propriété d’une balise de propriété. Ceci correspond au mot moins important dans une balise de propriété.<br/><br/>Le tableau PropertyType attribut plus loin dans cette rubrique contient les valeurs possibles de cet attribut.<br/><br/>Cet attribut est requis.  <br/> |
   
#### <a name="distinguishedpropertysetid-attribute"></a>Attribut DistinguishedPropertySetId

|**Valeur**|**Description**|
|:-----|:-----|
|Réunion  <br/> |Identifie la réunion propriété la valeur ID par un nom.  <br/> |
|Rendez-vous  <br/> |Identifie l’ID du jeu de propriété rendez-vous par nom.  <br/> |
|Common  <br/> |Identifie l’ID du jeu de propriété courantes par nom.  <br/> |
|PublicStrings  <br/> |Identifie l’ID du jeu de propriété publique chaînes par nom.  <br/> |
|Address  <br/> |Identifie l’ID du jeu de propriétés adresse par un nom.  <br/> |
|InternetHeaders  <br/> |Identifie l’ID du jeu de propriété en-têtes Internet par son nom.  <br/> |
|CalendarAssistant  <br/> |Identifie l’ID du jeu de propriété assistant calendrier par son nom.  <br/> |
|UnifiedMessaging  <br/> |Identifie l’ID du jeu de propriété messagerie unifiée par nom.  <br/> |
   
#### <a name="propertytype-attribute"></a>Attribut PropertyType

|**Valeur**|**Description**|
|:-----|:-----|
|ApplicationTime  <br/> |Une valeur de type double qui est interprétée comme une date et une heure. La partie entière correspond à la date et la partie fractionnaire est à la fois.  <br/> |
|ApplicationTimeArray  <br/> |Tableau de valeurs de type double qui est interprétée comme une date et une heure.  <br/> |
|Binaire  <br/> |Une valeur binaire codée en Base64.  <br/> |
|BinaryArray  <br/> |Tableau de valeurs binaires codé en Base64.  <br/> |
|Boolean  <br/> |Une valeur booléenne **true** ou **false**.  <br/> |
|CLSID  <br/> |Une chaîne en GUID.  <br/> |
|CLSIDArray  <br/> |Un tableau de chaînes GUID.  <br/> |
|Monnaie  <br/> |Entier 64 bits qui est interprété comme le nombre de centimes.  <br/> |
|CurrencyArray  <br/> |Tableau d’entiers 64 bits qui sont interprétées comme le nombre de centimes.  <br/> |
|Double  <br/> |Valeur à virgule flottante 64 bits.  <br/> |
|DoubleArray  <br/> |Tableau de valeurs à virgule flottante 64 bits.  <br/> |
|Error  <br/> |Valeur SCODE ; nombre entier non signé 32 bits.  <br/> Pas utilisé pour les restrictions ou pour les valeurs de l’obtention ou la définition. Il existe uniquement pour la création de rapports.  <br/> |
|Virgule flottante  <br/> |Valeur à virgule flottante 32 bits.  <br/> |
|FloatArray  <br/> |Tableau de valeurs à virgule flottante 32 bits.  <br/> |
|Entier  <br/> |Un nombre entier signé 32 bits (Int32).  <br/> |
|IntegerArray  <br/> |Tableau d’entiers signés de 32 bits (Int32).  <br/> |
|Long  <br/> |Un entier signé ou non signé 64 bits (Int64).  <br/> |
|LongArray  <br/> |Tableau de nombres entiers (Int64) 64 bits signés ou non signés.  <br/> |
|Null  <br/> |N’indique aucune valeur de propriété.  <br/> Pas utilisé pour les restrictions ou pour les valeurs de l’obtention ou la définition. Il existe uniquement pour la création de rapports.  <br/> |
|Objet  <br/> |Pointeur vers un objet qui implémente l’interface IUnknown.  <br/> Pas utilisé pour les restrictions ou pour les valeurs de l’obtention ou la définition. Il existe uniquement pour la création de rapports.  <br/> |
|ObjectArray  <br/> |Tableau de pointeurs vers des objets qui implémentent l’interface IUnknown.  <br/> Pas utilisé pour les restrictions ou pour les valeurs de l’obtention ou la définition. Il existe uniquement pour la création de rapports.  <br/> |
|Nom court  <br/> |Un entier signé de 16 bits.  <br/> |
|ShortArray  <br/> |Tableau d’entiers 16 bits signés.  <br/> |
|SystemTime  <br/> |Entier 64 bits et l’heure valeur sous la forme d’une structure FILETIME.  <br/> |
|SystemTimeArray  <br/> |Un tableau de valeurs de date et heure 64 bits entier sous la forme d’une structure FILETIME.  <br/> |
|String  <br/> |Une chaîne Unicode.  <br/> |
|StringArray  <br/> |Tableau de chaînes Unicode.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ExtendedProperty](extendedproperty.md) <br/> |Identifie les propriétés étendues sur les dossiers et les éléments.  <br/> |
|[AdditionalProperties](additionalproperties.md) <br/> | Identifie les propriétés supplémentaires.<br/><br/>Les expressions XPath pour cet élément sont les suivantes :<br/><br/>`/FindFolder/FolderShape/AdditionalProperties` <br/>  `/GetFolder/FolderShape/AdditionalProperties` <br/>  `/SyncFolderHierarchy/FolderShape/AdditionalProperties` <br/>  `/GetItem/ItemShape/AdditionalProperties` <br/>  `/FindItem/ItemShape/AdditionalProperties` <br/>  `/SyncFolderItems/ItemShape/AdditionalProperties` <br/>  `/GetAttachment/AttachmentShape/AdditionalProperties` <br/> |
|[SetItemField](setitemfield.md) <br/> |Représente une mise à jour d'une propriété unique d'un élément dans une [UpdateItem Operation](updateitem-operation.md).  <br/> |
|[SetFolderField](setfolderfield.md) <br/> |Représente une mise à jour d’une propriété donnée sur un dossier dans une [opération UpdateFolder](updatefolder-operation.md).  <br/> |
|[DeleteItemField](deleteitemfield.md) <br/> |Représente une opération delete pour supprimer une propriété donnée d’un élément pendant une [opération UpdateItem](updateitem-operation.md).  <br/> |
|[DeleteFolderField](deletefolderfield.md) <br/> |Représente une opération delete pour supprimer une propriété donnée d’un dossier pendant un appel UpdateFolder.  <br/> |
|[AppendToItemField](appendtoitemfield.md) <br/> |Identifie les données à ajouter à une propriété d’un élément pendant une [opération UpdateItem](updateitem-operation.md).  <br/> |
|[AppendToFolderField](appendtofolderfield.md) <br/> |Spécifie les données à ajouter à une propriété de dossier lors d’une [opération UpdateFolder](updatefolder-operation.md).  <br/> |
|[Exists](exists.md) <br/> |Représente une expression de recherche qui retourne la **valeur true** si la propriété fournie existe sur un élément.  <br/> |
|[FieldURIOrConstant](fielduriorconstant.md) <br/> |Représente une propriété ou une constante à utiliser lors de la comparaison avec une autre propriété.  <br/> |
|[IsEqualTo](isequalto.md) <br/> |Représente une expression de recherche qui compare une propriété avec une valeur constante ou une autre propriété et renvoie **la valeur true** si elles sont égales.  <br/> |
|[IsGreaterThan](isgreaterthan.md) <br/> |Représente une expression de recherche qui compare une propriété avec une valeur constante ou une autre propriété et renvoie **la valeur true** si la première propriété est supérieure.  <br/> |
|[IsGreaterThanOrEqualTo](isgreaterthanorequalto.md) <br/> |Représente une expression de recherche qui compare une propriété avec une valeur constante ou une autre propriété et renvoie **la valeur true** si la première propriété est supérieure ou égale à la seconde.  <br/> |
|[IsLessThan](islessthan.md) <br/> |Représente une expression de recherche qui compare une propriété avec une valeur constante ou une autre propriété et renvoie **la valeur true** si la première propriété est inférieure à la seconde.  <br/> |
|[IsLessThanOrEqualTo](islessthanorequalto.md) <br/> |Représente une expression de recherche qui compare une propriété avec une valeur constante ou une autre propriété et renvoie **la valeur true** si la première propriété est inférieure à la seconde.  <br/> |
|[IsNotEqualTo](isnotequalto.md) <br/> |Représente une expression de recherche qui compare une propriété avec une valeur constante ou une autre propriété et renvoie **la valeur true** si les valeurs ne sont pas identiques.  <br/> |
|[Excludes](excludes.md) <br/> |Effectue un masque de bits des propriétés.  <br/> |
|[Contient](contains.md) <br/> |Représente une expression de recherche qui détermine si une propriété donnée contient la valeur de chaîne constante fournie.  <br/> |
|[FieldOrder](fieldorder.md) <br/> |Représente un seul champ à utiliser pour trier les résultats et indique le sens du tri.  <br/> |
   
## <a name="remarks"></a>Remarques

Certains attributs ne peut pas être utilisés conjointement avec d’autres attributs. Toute demande qui comporte une combinaison des attributs de propriété étendue non valide génère un message d’erreur.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
> [!NOTE]
> Dans Microsoft .NET, une valeur Long est un entier signé de 64 bits, alors que dans MAPI et COM, une valeur Long est un entier 32 bits. La plupart des développeurs utilise Microsoft.NET Framework pour développer des applications clientes de Services Web Exchange. Par conséquent, l’affectation de noms .NET est utilisée à la place l’interface MAPI d’attribution de noms.
> 
> Par exemple, la propriété MAPI PR_MESSAGE_FLAGS, 0x0E07, est un PT\_tapez LONG. Dans .NET, il est considéré comme un entier. Une propriété étendue pour PR_MESSAGE_FLAGS est définie en tant que `<t:ExtendedFieldURI PropertyTag="0x0E07" PropertyType="Integer"/>`. 
  
## <a name="example"></a>Exemple

Une demande de l’exemple suivant crée un élément qui possède deux propriétés personnalisées. La première propriété personnalisée est nommée **IsMyHouse** avec une valeur de type Boolean définie sur **true**. La seconde propriété étendue personnalisée nommée **HousePrices**. Il contient un tableau de valeurs monétaires. 
  
```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" 
                  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
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
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [FieldURI](fielduri.md)
- [IndexedFieldURI](indexedfielduri.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)


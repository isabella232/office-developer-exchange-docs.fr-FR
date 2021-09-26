---
title: ExtendedFieldURI
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ExtendedFieldURI
api_type:
- schema
ms.assetid: b3c6ea3a-9ead-44b9-9d99-64ecf12bde23
description: L’élément ExtendedFieldURI identifie une propriété MAPI étendue.
ms.openlocfilehash: 0cf3926c900e1b1f35018c6706cfe99ebefbe76f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542315"
---
# <a name="extendedfielduri"></a>ExtendedFieldURI

**L’élément ExtendedFieldURI** identifie une propriété MAPI étendue. 
  
```xml
<ExtendedFieldURI DistinguishedPropertySetId="" PropertySetId="" PropertyTag="" PropertyName="" PropertyId="" PropertyType="" />
```

**PathToExtendedFieldType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**DistinguishedPropertySetId** <br/> |Définit les ID de jeu de propriétés connus pour les propriétés MAPI étendues.<br/><br/>Si cet attribut est utilisé, les attributs **PropertySetId** et **PropertyTag** ne peuvent pas être utilisés. Cet attribut doit être utilisé avec l’attribut **PropertyId** ou **PropertyName** et **l’attribut PropertyType.**<br/><br/>Le **tableau DistinguishedPropertySetId** Attribute plus loin dans cette rubrique répertorie les valeurs possibles pour cet attribut.<br/><br/>Cet attribut est facultatif.  <br/> |
|**PropertySetId** <br/> |Identifie un jeu de propriétés étendu MAPI ou un espace de noms par son GUID d’identification.<br/><br/>Si cet attribut est utilisé, les **attributs DistinguishedPropertySetId** et **PropertyTag** ne peuvent pas être utilisés. Cet attribut doit être utilisé avec l’attribut **PropertyId** ou **PropertyName** et **l’attribut PropertyType.**<br/><br/>Cet attribut est facultatif.  <br/> |
|**PropertyTag** <br/> |Identifie la balise de propriété sans la partie type de la balise. PropertyTag **peut** être représenté en tant qu’un hexadécimal ou un petit integer.<br/><br/>La plage entre 0x8000 et 0xFFFE représente la plage personnalisée de propriétés. Lorsqu’une base de données de boîtes aux lettres rencontre une propriété personnalisée pour la première fois, elle affecte à cette propriété personnalisée une balise de propriété dans la plage de propriétés personnalisées 0x8000-0xFFFE. Une balise de propriété personnalisée donnée sera probablement différente d’une base de données à l’autre. Par conséquent, une demande de propriété personnalisée par balise de propriété peut renvoyer différentes propriétés sur différentes bases de données. L’utilisation de **l’attribut PropertyTag** est interdite pour les propriétés personnalisées. Utilisez plutôt **l’attribut PropertySetId** et l’attribut **PropertyName** ou **PropertyId.**<br/><br/>**IMPORTANT**: accéder à toute propriété personnalisée entre 0x8000 et 0xFFFE à l’aide du GUID + nom/ID. Si **l’attribut PropertyTag** est utilisé, les attributs **DistinguishedPropertySetId**, **PropertySetId**, **PropertyName** et **PropertyId** ne peuvent pas être utilisés.<br/><br/>Cet attribut est facultatif.<br/><br/>**REMARQUE**: vous ne pouvez pas utiliser un attribut de balise de propriété pour les propriétés dans la plage personnalisée 0x8000-0xFFFE. Vous devez utiliser une propriété nommée dans ce cas.           |
|**PropertyName** <br/> |Identifie une propriété étendue par son nom. Cette propriété doit être couplée à **DistinguishedPropertySetId** ou **PropertySetId**.<br/><br/>Si cet attribut est utilisé, les attributs **PropertyId** et **PropertyTag** ne peuvent pas être utilisés.<br/><br/>Cet attribut est facultatif.  <br/> |
|**PropertyId** <br/> |Identifie une propriété étendue par son ID de distribution. L’ID de répartition peut être identifié au format décimal ou hexadécimal. Cette propriété doit être couplée à **DistinguishedPropertySetId** ou **PropertySetId**.<br/><br/>Si cet attribut est utilisé, les attributs **PropertyName** et **PropertyTag** ne peuvent pas être utilisés.<br/><br/>Cet attribut est facultatif.  <br/> |
|**PropertyType** <br/> |Représente le type de propriété d’une balise de propriété. Cela correspond au mot le moins significatif dans une balise de propriété.<br/><br/>Le tableau PropertyType Attribute plus loin dans cette rubrique contient les valeurs possibles pour cet attribut.<br/><br/>Cet attribut est obligatoire.  <br/> |
   
#### <a name="distinguishedpropertysetid-attribute"></a>Attribut DistinguishedPropertySetId

|**Valeur**|**Description**|
|:-----|:-----|
|Adresse  <br/> |Identifie l’ID de jeu de propriétés d’adresse par nom.  <br/> |
|Rendez-vous  <br/> |Identifie l’ID de jeu de propriétés de rendez-vous par nom.  <br/> |
|CalendarAssistant  <br/> |Identifie l’ID de jeu de propriétés de l’Assistant Calendrier par son nom.  <br/> |
|Courant  <br/> |Identifie l’ID de jeu de propriétés commun par nom.  <br/> |
|InternetHeaders  <br/> |Identifie l’ID de jeu de propriétés d’en-têtes Internet par nom.  <br/> |
|Réunion  <br/> |Identifie l’ID de jeu de propriétés de réunion par nom.  <br/> |
|Partage  <br/> | <br/> |
|PublicStrings  <br/> |Identifie l’ID de jeu de propriétés de chaînes publiques par nom.  <br/> |
|Tâche  <br/> |Identifie l’ID de jeu de propriétés de tâche par nom.  <br/> |
|UnifiedMessaging  <br/> |Identifie l’ID de jeu de propriétés de messagerie unifiée par nom.  <br/> |
   
#### <a name="propertytype-attribute"></a>Attribut PropertyType

|**Valeur**|**Description**|
|:-----|:-----|
|ApplicationTime  <br/> |Valeur double interprétée comme une date et une heure. La partie de nombres longs est la date et la partie fraction représente l’heure.  <br/> |
|ApplicationTimeArray  <br/> |Tableau de valeurs doubles interprétées comme une date et une heure.  <br/> |
|Binaire  <br/> |Valeur binaire codée en Base64.  <br/> |
|BinaryArray  <br/> |Tableau de valeurs binaires codées en Base64.  <br/> |
|Valeur booléenne  <br/> |Valeur Boolean **true** ou **false**.  <br/> |
|CLSID  <br/> |Chaîne GUID.  <br/> |
|CLSIDArray  <br/> |Tableau de chaînes GUID.  <br/> |
|Devise  <br/> |Un nombre d’nombres integer 64 bits qui est interprété comme le nombre de sous-titres.  <br/> |
|CurrencyArray  <br/> |Tableau d’nombres d’nombres integers 64 bits interprétés comme le nombre de sous-titres.  <br/> |
|Double  <br/> |Valeur à valeur à valeur flottante 64 bits.  <br/> |
|DoubleArray  <br/> |Tableau de valeurs à valeurs à valeurs flottantes 64 bits.  <br/> |
|Erreur  <br/> |Valeur SCODE ; Integer non signé 32 bits.  <br/> Non utilisé pour les restrictions ou pour obtenir/définir des valeurs. Cela n’existe que pour les rapports.  <br/> |
|Flottant  <br/> |Valeur à valeur à valeur flottante 32 bits.  <br/> |
|FloatArray  <br/> |Tableau de valeurs à valeurs à valeurs flottantes 32 bits.  <br/> |
|Entier  <br/> |Un integer 32 bits signé (Int32).  <br/> |
|IntegerArray  <br/> |Tableau d’integers signés 32 bits (Int32).  <br/> |
|Entier long  <br/> |Un integer 64 bits (Int64) signé ou non signé.  <br/> |
|LongArray  <br/> |Tableau d’nombres d’integers 64 bits (Int64) signés ou non signés.  <br/> |
|Null  <br/> |Indique aucune valeur de propriété.  <br/> Non utilisé pour les restrictions ou pour obtenir/définir des valeurs. Cela n’existe que pour les rapports.  <br/> |
|Objet  <br/> |Pointeur vers un objet qui implémente l’interface IUnknown.  <br/> Non utilisé pour les restrictions ou pour obtenir/définir des valeurs. Cela n’existe que pour les rapports.  <br/> |
|ObjectArray  <br/> |Tableau de pointeurs vers des objets qui implémentent l’interface IUnknown.  <br/> Non utilisé pour les restrictions ou pour obtenir/définir des valeurs. Cela n’existe que pour les rapports.  <br/> |
|Nom court  <br/> |Un integer signé 16 bits.  <br/> |
|ShortArray  <br/> |Tableau d’nombres integers signés 16 bits.  <br/> |
|SystemTime  <br/> |Nombre entière de 64 bits et valeur de temps sous la forme d’une structure FILETIME.  <br/> |
|SystemTimeArray  <br/> |Tableau de données entières 64 bits et de valeurs d’heure sous la forme d’une structure FILETIME.  <br/> |
|Chaîne  <br/> |Chaîne Unicode.  <br/> |
|StringArray  <br/> |Tableau de chaînes Unicode.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ExtendedProperty](extendedproperty.md) <br/> |Identifie les propriétés étendues sur les dossiers et les éléments.  <br/> |
|[AdditionalProperties](additionalproperties.md) <br/> | Identifie les propriétés supplémentaires.<br/><br/>Les expressions XPath de cet élément sont les suivantes :<br/><br/>`/FindFolder/FolderShape/AdditionalProperties` <br/>  `/GetFolder/FolderShape/AdditionalProperties` <br/>  `/SyncFolderHierarchy/FolderShape/AdditionalProperties` <br/>  `/GetItem/ItemShape/AdditionalProperties` <br/>  `/FindItem/ItemShape/AdditionalProperties` <br/>  `/SyncFolderItems/ItemShape/AdditionalProperties` <br/>  `/GetAttachment/AttachmentShape/AdditionalProperties` <br/> |
|[SetItemField](setitemfield.md) <br/> |Représente une mise à jour d'une propriété unique d'un élément dans une [UpdateItem Operation](updateitem-operation.md).  <br/> |
|[SetFolderField](setfolderfield.md) <br/> |Représente une mise à jour d’une propriété unique sur un dossier dans une [opération UpdateFolder](updatefolder-operation.md).  <br/> |
|[DeleteItemField](deleteitemfield.md) <br/> |Représente une opération de suppression pour supprimer une propriété donnée d’un élément pendant une [opération UpdateItem](updateitem-operation.md).  <br/> |
|[DeleteFolderField](deletefolderfield.md) <br/> |Représente une opération de suppression pour supprimer une propriété donnée d’un dossier pendant un appel UpdateFolder.  <br/> |
|[AppendToItemField](appendtoitemfield.md) <br/> |Identifie les données à append à une propriété unique d’un élément lors d’une [opération UpdateItem](updateitem-operation.md).  <br/> |
|[AppendToFolderField](appendtofolderfield.md) <br/> |Spécifie les données à appendre à une propriété de dossier lors d’une [opération UpdateFolder](updatefolder-operation.md).  <br/> |
|[Exists](exists.md) <br/> |Représente une expression de recherche qui renvoie **la valeur true** si la propriété fournie existe sur un élément.  <br/> |
|[FieldURIOrConstant](fielduriorconstant.md) <br/> |Représente une propriété ou une valeur constante à utiliser lors de la comparaison avec une autre propriété.  <br/> |
|[IsEqualTo](isequalto.md) <br/> |Représente une expression de recherche qui compare une propriété avec une valeur constante ou une autre propriété et qui est évaluée à **true** si elles sont égales.  <br/> |
|[IsGreaterThan](isgreaterthan.md) <br/> |Représente une expression de recherche qui compare une propriété avec une valeur constante ou une autre propriété et renvoie **true** si la première propriété est supérieure.  <br/> |
|[IsGreaterThanOrEqualTo](isgreaterthanorequalto.md) <br/> |Représente une expression de recherche qui compare une propriété avec une valeur constante ou une autre propriété et renvoie la valeur **true** si la première propriété est supérieure ou égale à la seconde.  <br/> |
|[IsLessThan](islessthan.md) <br/> |Représente une expression de recherche qui compare une propriété avec une valeur constante ou une autre propriété et renvoie la valeur **true** si la première propriété est inférieure à la seconde.  <br/> |
|[IsLessThanOrEqualTo](islessthanorequalto.md) <br/> |Représente une expression de recherche qui compare une propriété avec une valeur constante ou une autre propriété et renvoie la valeur **true** si la première propriété est inférieure à la seconde.  <br/> |
|[IsNotEqualTo](isnotequalto.md) <br/> |Représente une expression de recherche qui compare une propriété avec une valeur constante ou une autre propriété et renvoie **true** si les valeurs ne sont pas identiques.  <br/> |
|[Excludes](excludes.md) <br/> |Effectue un masque de propriétés au sens du bit.  <br/> |
|[Contains](contains.md) <br/> |Représente une expression de recherche qui détermine si une propriété donnée contient la valeur de chaîne constante fournie.  <br/> |
|[FieldOrder](fieldorder.md) <br/> |Représente un champ unique par lequel trier les résultats et indique le sens du tri.  <br/> |
   
## <a name="remarks"></a>Remarques

Certains attributs ne peuvent pas être utilisés en combinaison avec d’autres attributs. Toute demande qui insérait une combinaison non valide d’attributs de propriété étendue génère un message d’erreur.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
> [!NOTE]
> Dans Microsoft .NET, un long est un integer signé 64 bits, tandis que dans MAPI et COM, un long est un integer 32 bits. La plupart des développeurs utiliseront Microsoft.NET Framework pour développer Exchange applications clientes des services Web. Par conséquent, l’appellation .NET est utilisée à la place de l’appellation MAPI.
> 
> Par exemple, la PR_MESSAGE_FLAGS MAPI, 0x0E07, est un \_ type PT LONG. Dans .NET, il s’agit d’un chiffre. Une propriété étendue pour PR_MESSAGE_FLAGS est définie comme `<t:ExtendedFieldURI PropertyTag="0x0E07" PropertyType="Integer"/>` . 
  
## <a name="example"></a>Exemple

L’exemple suivant d’une requête crée un élément qui possède deux propriétés personnalisées. La première propriété personnalisée est nommée **IsMyHouse** avec une valeur boolé locale définie sur **true**. La deuxième propriété étendue personnalisée est nommée **HousePrices**. Il contient un tableau de valeurs Monétaires. 
  
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


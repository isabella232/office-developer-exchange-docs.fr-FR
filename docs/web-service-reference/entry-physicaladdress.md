---
title: Entrée (PhysicalAddress)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Entry
api_type:
- schema
ms.assetid: 9e5b6515-453e-4f4c-b55e-6ffefe23c31b
description: L’élément Entry décrit une adresse physique unique pour un élément de contact.
ms.openlocfilehash: b951c8c099a9653635e8fa95fe06204659b7d1fd
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517104"
---
# <a name="entry-physicaladdress"></a>Entrée (PhysicalAddress)

**L’élément Entry** décrit une adresse physique unique pour un élément de contact. 
  
```xml
<Entry Key="">
   <Street/>
   <City/>
   <State/>
   <Country/>
   <PostalCode/>
</Entry>
```

 **PhysicalAddressDictionaryEntryType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**Clé** <br/> | Identifie une adresse physique.<br/><br/> Les valeurs possibles pour cet attribut sont les suivantes :<br/>  <br/>- Entreprise  <br/>- Accueil  <br/>- Autre  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Street](street.md) <br/> |Représente une adresse de rue pour un élément de contact.  <br/> |
|[City](city.md) <br/> |Représente le nom de la ville associé à un contact.  <br/> |
|[State](state-ex15websvcsotherref.md) <br/> |Représente l’état de résidence d’un élément de contact.  <br/> |
|[CountryOrRegion](countryorregion.md) <br/> |Représente le pays ou la région d’une adresse physique donnée.  <br/> |
|[PostalCode](postalcode.md) <br/> |Représente le code postal d’un élément de contact.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[PhysicalAddresses](physicaladdresses.md) <br/> |Contient une collection d'adresses physiques associées à un contact.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML EWS dans Exchange](ews-xml-elements-in-exchange.md)
- [Création de Contacts (Services Web Exchange)](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)  
- [Updating Contacts](https://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)  
- [Deleting Contacts](https://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)


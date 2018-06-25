---
title: Entrée (PhysicalAddress)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Entry
api_type:
- schema
ms.assetid: 9e5b6515-453e-4f4c-b55e-6ffefe23c31b
description: L’élément d’entrée décrit une seule adresse physique pour un élément de contact.
ms.openlocfilehash: 4551e6117e5f91d901fe160f37e8f67cb1bc5ac7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756195"
---
# <a name="entry-physicaladdress"></a>Entrée (PhysicalAddress)

L’élément **d’entrée** décrit une seule adresse physique pour un élément de contact. 
  
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

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**Clé** <br/> | Identifie une adresse physique.<br/><br/> Les valeurs possibles de cet attribut sont les suivantes :<br/>  <br/>-Business  <br/>-Accueil  <br/>-Autres  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Street](street.md) <br/> |Représente une adresse postale pour un élément de contact.  <br/> |
|[Ville](city.md) <br/> |Représente le nom de la ville qui est associé à un contact.  <br/> |
|[State](state-ex15websvcsotherref.md) <br/> |Représente l’état de résidence pour un élément de contact.  <br/> |
|[Countryorregion définit](countryorregion.md) <br/> |Représente le pays ou la région pour l’adresse physique donnée.  <br/> |
|[Code postal](postalcode.md) <br/> |Représente le code postal pour un élément de contact.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[PhysicalAddresses](physicaladdresses.md) <br/> |Contient une collection d'adresses physiques associées à un contact.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)
- [Creating Contacts (Exchange Web Services)](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)  
- [Updating Contacts](http://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)  
- [Deleting Contacts](http://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)


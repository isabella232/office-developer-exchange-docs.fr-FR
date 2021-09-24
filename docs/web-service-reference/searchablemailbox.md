---
title: SearchableMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 339005cd-a3b9-47dd-bc7b-a860b699625b
description: L’élément SearchableMailbox spécifie une boîte aux lettres renvoyée par une demande GetSearchableMailboxes.
ms.openlocfilehash: 75d5680de8b0776b1ecf441ff71266ee74c4aa66
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524426"
---
# <a name="searchablemailbox"></a>SearchableMailbox

**L’élément SearchableMailbox spécifie** une boîte aux lettres renvoyée par une **demande GetSearchableMailboxes.** 
  
```XML
<SearchableMailbox>
   <Guid/>
   <PrimarySmtpAddress/>
   <IsExternalMailbox/>
   <ExternalEmailAddress/>
   <DisplayName/>
   <IsMembershipGroup/>
   <ReferenceId/>
</SearchableMailbox>
```

 **SearchableMailboxType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

[Guid](guid-ex15websvcsotherref.md)  |  [PrimarySmtpAddress (string)](primarysmtpaddress-string.md)  |  [IsExternalMailbox](isexternalmailbox.md)  |  [ExternalEmailAddress](externalemailaddress.md)  |  [DisplayName (chaîne)](displayname-string.md)  |  [IsMembershipGroup](ismembershipgroup.md)  |  [ReferenceId](referenceid.md)
  
### <a name="parent-elements"></a>Éléments parents

[SearchableMailboxes](searchablemailboxes.md)
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> ||
   


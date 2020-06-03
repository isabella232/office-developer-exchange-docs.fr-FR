---
title: Expéditeurs
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 69d88bb1-397c-4fb8-bd2b-21cccc5bb35d
description: L’élément Senders spécifie un tableau d’adresses SMTP (Simple Mail Transfer Protocol).
ms.openlocfilehash: 125d448be53b2ae297cd1e7249a04da6eda5d960
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530571"
---
# <a name="senders"></a>Expéditeurs

L’élément **Senders** spécifie un tableau d’adresses SMTP (Simple Mail Transfer Protocol). 
  
```XML
<Senders>
   <SmtpAddress/>
</Senders>
```

 **ArrayOfSmtpAddressType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

[SmtpAddress](smtpaddress.md)
  
### <a name="parent-elements"></a>Éléments parents

[FindMailboxStatisticsByKeywords](findmailboxstatisticsbykeywords.md)
  
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
   


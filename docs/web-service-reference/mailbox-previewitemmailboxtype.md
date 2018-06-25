---
title: Boîte aux lettres (PreviewItemMailboxType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e898d737-b6e4-4403-9c2c-aec52a48a83d
description: L’élément de boîte aux lettres contient l’identificateur de la boîte aux lettres et l’adresse SMTP Simple Mail Transfer Protocol () principale de l’utilisateur.
ms.openlocfilehash: 1b6669928015bc880806479d294a4063034a559f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828255"
---
# <a name="mailbox-previewitemmailboxtype"></a>Boîte aux lettres (PreviewItemMailboxType)

L’élément de **boîte aux lettres** contient l’identificateur de la boîte aux lettres et l’adresse SMTP Simple Mail Transfer Protocol () principale de l’utilisateur. 
  
```XML
<Mailbox>
   <MailboxId/>
   <PrimarySmtpAddress/>
</Mailbox>
```

**PreviewItemMailboxType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

[MailboxId](mailboxid.md) | [PrimarySmtpAddress (chaîne)](primarysmtpaddress-string.md)
  
### <a name="parent-elements"></a>Éléments parents

[SearchPreviewItem](searchpreviewitem.md)
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |false  <br/> |
   


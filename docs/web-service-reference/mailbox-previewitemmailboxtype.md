---
title: Boîte aux lettres (PreviewItemMailboxType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e898d737-b6e4-4403-9c2c-aec52a48a83d
description: L’élément Mailbox contient l’identificateur de boîte aux lettres et l’adresse SMTP (Simple Mail Transfer Protocol) principale de l’utilisateur.
ms.openlocfilehash: 4dc5ee45c00945c30a699daa0158c96679189ab1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463894"
---
# <a name="mailbox-previewitemmailboxtype"></a>Boîte aux lettres (PreviewItemMailboxType)

L’élément **Mailbox** contient l’identificateur de boîte aux lettres et l’adresse SMTP (Simple Mail Transfer Protocol) principale de l’utilisateur. 
  
```XML
<Mailbox>
   <MailboxId/>
   <PrimarySmtpAddress/>
</Mailbox>
```

**PreviewItemMailboxType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

[MailboxId](mailboxid.md)  |  [PrimarySmtpAddress (String)](primarysmtpaddress-string.md)
  
### <a name="parent-elements"></a>Éléments parents

[SearchPreviewItem](searchpreviewitem.md)
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |false  <br/> |
   


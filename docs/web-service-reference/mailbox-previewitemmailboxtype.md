---
title: Mailbox (PreviewItemMailboxType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: e898d737-b6e4-4403-9c2c-aec52a48a83d
description: L’élément Mailbox contient l’identificateur de boîte aux lettres et l’adresse SMTP (Simple Mail Transfer Protocol) principale de l’utilisateur.
ms.openlocfilehash: 1a2dcc08d3e1595aede21e6982b36a60e6efafb5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514297"
---
# <a name="mailbox-previewitemmailboxtype"></a>Mailbox (PreviewItemMailboxType)

**L’élément Mailbox** contient l’identificateur de boîte aux lettres et l’adresse SMTP (Simple Mail Transfer Protocol) principale de l’utilisateur. 
  
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

[MailboxId](mailboxid.md)  |  [PrimarySmtpAddress (string)](primarysmtpaddress-string.md)
  
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
   


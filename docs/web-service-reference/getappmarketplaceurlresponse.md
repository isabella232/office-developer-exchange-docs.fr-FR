---
title: GetAppMarketplaceUrlResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: dc3368ec-78c2-4f8d-8394-4891e90dafd2
description: L’élément GetAppMarketplaceUrlResponse spécifie la réponse à une demande GetAppMarketplaceUrl.
ms.openlocfilehash: 14ab39add46441080fc7ae88264c79ef1bc8d98f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59530001"
---
# <a name="getappmarketplaceurlresponse"></a>GetAppMarketplaceUrlResponse

**L’élément GetAppMarketplaceUrlResponse** spécifie la réponse à une **demande GetAppMarketplaceUrl.** 
  
```XML
<GetAppMarketplaceUrlResponse ResponseClass=" Success | Warning | Error ">
    <AppMarketplaceUrl/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</GetAppMarketplaceUrlResponse>
```

 **GetAppMarketplaceUrlResponseMessageType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|ResponseClass  <br/> |Indique la classe de la réponse.  <br/> |
   
#### <a name="responseclass"></a>ResponseClass

|**Valeur**|**Description**|
|:-----|:-----|
|Opération réussie  <br/> |Indique la réussite.  <br/> |
|Avertissement  <br/> |Indique un avertissement.  <br/> |
|Erreur  <br/> |Indique une erreur.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[AppMarketplaceUrl](appmarketplaceurl.md) <br/> |Spécifie l’URL de l’application.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |Actuellement inutilisé et réservé pour une utilisation ultérieure.  <br/> |
|[MessageText](messagetext.md) <br/> |Fournit une description textuelle de l’état de la réponse.  <br/> |
|[MessageXml](messagexml.md) <br/> |Fournit des informations supplémentaires sur la réponse aux erreurs.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Fournit des informations d’état sur la demande.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Contient les messages de réponse pour une demande Exchange services Web.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma des messages  <br/> |
|Fichier de validation  <br/> |messages.xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)


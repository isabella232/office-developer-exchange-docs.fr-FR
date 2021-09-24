---
title: OrganizationRelationshipSettings (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 917481bb-46fc-4b88-8683-4cf812dcb0ab
description: L’élément OrganizationRelationshipSettings représente une liste de relations d’organisation pour une seule organisation. L’élément OrganizationRelationshipSettings est uniquement à usage interne. Cet élément n’est pas utilisé par les clients.
ms.openlocfilehash: bff515456d6f86648417070008845b7b5caa6d8a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514248"
---
# <a name="organizationrelationshipsettings-soap"></a>OrganizationRelationshipSettings (SOAP)

**L’élément OrganizationRelationshipSettings** représente une liste de relations d’organisation pour une seule organisation. **L’élément OrganizationRelationshipSettings est** uniquement à usage interne. Cet élément n’est pas utilisé par les clients. 
  
```XML
<OrganizationRelationshipSettings>
    <DeliveryReportEnabled/>
    <DomainNames/>
    <FreeBusyAccessEnabled/>
    <FreeBusyAccessLevel/>
    <MailTipsAccessEnabled/>
    <MailTipsAccessLevel/>
    <MailboxMoveEnabled/>
    <Name/>
    <TargetApplicationUri/>
    <TargetAudodiscoverEpr/>
    <TargetSharingEpr/>
</OrganizationRelationshipSettings>
```

 **OrganizationRelationshipSettings**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[DeliveryReportEnabled (SOAP)](deliveryreportenabled-soap.md) <br/> |Représente [l’indicateur DeliveryReportEnabled().](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.DeliveryReportEnabled.aspx)  <br/> |
|[DomainNames (SOAP)](domainnames-soap.md) <br/> |Représente la collection de noms de domaine.  <br/> |
|[FreeBusyAccessEnabled (SOAP)](freebusyaccessenabled-soap.md) <br/> |Représente [l’indicateur FreeBusyAccessEnabled().](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.FreeBusyAccessEnabled.aspx)  <br/> |
|[FreeBusyAccessLevel (SOAP)](freebusyaccesslevel-soap.md) <br/> |Représente la [propriété FreeBusyAccessLevel.](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.FreeBusyAccessLevel.aspx)  <br/> |
|[MailTipsAccessEnabled (SOAP)](mailtipsaccessenabled-soap.md) <br/> |Représente [l’indicateur MailTipsAccessEnabled().](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.MailTipsAccessEnabled.aspx)  <br/> |
|[MailTipsAccessLevel (SOAP)](mailtipsaccesslevel-soap.md) <br/> |Représente la [propriété MailTipsAccessLevel.](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.MailTipsAccessLevel.aspx)  <br/> |
|[MailboxMoveEnabled (SOAP)](mailboxmoveenabled-soap.md) <br/> |Représente [l’indicateur MailboxMoveEnabled().](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.MailboxMoveEnabled.aspx)  <br/> |
|[Name (SOAP)](name-soap.md) <br/> |Représente le nom de la relation d’organisation.  <br/> |
|[TargetApplicationUri (SOAP)](targetapplicationuri-soap.md) <br/> |Définit l’URI de l’application cible.  <br/> |
|[TargetAutodiscoverEpr (SOAP)](targetautodiscoverepr-soap.md) <br/> |Représente la [propriété TargetAutodiscoverEpr.](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.TargetAutodiscoverEpr.aspx)  <br/> |
|[TargetSharingEpr (SOAP)](targetsharingepr-soap.md) <br/> |Représente la [propriété TargetSharingEpr.](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.TargetSharingEpr.aspx)  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[OrganizationRelationshipSettingsCollection (SOAP)](organizationrelationshipsettingscollection-soap.md) <br/> |Représente une liste des relations d’organisation qui correspondent à la requête.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucune.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   


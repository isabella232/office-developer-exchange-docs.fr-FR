---
title: Opération GetUserRetentionPolicyTags
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 57c6ff23-5c2c-42ee-824b-5a1b6dafab8c
description: Opération de recherche plus d’informations sur la GetUserRetentionPolicyTags EWS.
ms.openlocfilehash: 2b1267ce6822c7bad05ad2ef88547ba75c632ab0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827700"
---
# <a name="getuserretentionpolicytags-operation"></a>Opération GetUserRetentionPolicyTags

Trouvez des informations sur l’opération EWS **GetUserRetentionPolicyTags** . 
  
L’opération **GetUserRetentionPolicyTags** Obtient une liste de tous les par défaut, dossier système et des balises personnelles qui sont associés à un utilisateur à l’aide d’une stratégie système ou qui ont été appliquées par l’utilisateur. 
  
Cette opération est une nouveauté d’Exchange Server 2013.
  
## <a name="using-the-getuserretentionpolicytags-operation"></a>Utilisation de l’opération GetUserRetentionPolicyTags

Cette opération renvoie le nom complet, ID de rétention, période de rétention, type de rétention, action de rétention et des balises description et les valeurs des propriétés **IsVisible**, **OptedInto**et **IsArchive** . 
  
### <a name="getuserretentionpolicytags-operation-soap-headers"></a>En-têtes SOAP GetUserRetentionPolicyTags opération

L’opération **GetUserRetentionPolicyTags** permettre utiliser les en-têtes SOAP qui sont répertoriés dans le tableau suivant. 
  
|**Nom de l'en-tête**|**Élément**|**Description**|
|:-----|:-----|:-----|
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifie la version du schéma pour la requête d’opération. Ceci s’applique à une demande.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifie la version du serveur qui a répondu à la demande. Cela s’applique à une réponse.  <br/> |
   
## <a name="getuserretentionpolicytags-operation-request-example"></a>Exemple de requête d’opération GetUserRetentionPolicyTags

Une demande d’opération **GetUserRetentionPolicyTags** l’exemple suivant montre comment obtenir la liste des balises pour l’utilisateur actuel. 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body>
      <m:GetUserRetentionPolicyTags />
   </soap:Body>
</soap:Envelope>
```

La demande SOAP body contienne l’élément suivant :
  
- [GetUserRetentionPolicyTags](getuserretentionpolicytags.md)
    
## <a name="successful-getuserretentionpolicytags-operation-response"></a>Réponse d’opération GetUserRetentionPolicyTags réussie

L’exemple suivant montre une réponse positive à une demande d’opération **GetUserRetentionPolicyTags** . 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="179" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetUserRetentionPolicyTagsResponse ResponseClass="Success" 
                                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <RetentionPolicyTags>
            <RetentionPolicyTag xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <DisplayName>1 Year Delete</DisplayName>
               <RetentionId>e66252f9-794f-4b36-b55e-d6d95fdf87a3</RetentionId>
               <RetentionPeriod>365</RetentionPeriod>
               <Type>Personal</Type>
               <RetentionAction>DeleteAndAllowRecovery</RetentionAction>
               <Description/>
               <IsVisible>true</IsVisible>
               <OptedInto>false</OptedInto>
               <IsArchive>false</IsArchive>
            </RetentionPolicyTag>
            <RetentionPolicyTag xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <DisplayName>Personal 1 year move to archive</DisplayName>
               <RetentionId>b2a29464-649c-4174-932b-6aaac9811c89</RetentionId>
               <RetentionPeriod>365</RetentionPeriod>
               <Type>Personal</Type>
               <RetentionAction>MoveToArchive</RetentionAction>
               <Description/>
               <IsVisible>true</IsVisible>
               <OptedInto>false</OptedInto>
               <IsArchive>true</IsArchive>
            </RetentionPolicyTag>
            <RetentionPolicyTag xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <DisplayName>Sent Items</DisplayName>
               <RetentionId>b0d32f1b-fbd0-4c1d-ba3e-ddd1086ea1d3</RetentionId>
               <RetentionPeriod>365</RetentionPeriod>
               <Type>SentItems</Type>
               <RetentionAction>DeleteAndAllowRecovery</RetentionAction>
               <Description/>
               <IsVisible>false</IsVisible>
               <OptedInto>false</OptedInto>
               <IsArchive>false</IsArchive>
            </RetentionPolicyTag>
            <RetentionPolicyTag xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <DisplayName>Default 1 year delete</DisplayName>
               <RetentionId>29fc9b9d-98b0-4c01-acf8-3996e2afce98</RetentionId>
               <RetentionPeriod>365</RetentionPeriod>
               <Type>All</Type>
               <RetentionAction>DeleteAndAllowRecovery</RetentionAction>
               <Description/>
               <IsVisible>false</IsVisible>
               <OptedInto>false</OptedInto>
               <IsArchive>false</IsArchive>
            </RetentionPolicyTag>
            <RetentionPolicyTag xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <DisplayName>Two Year Retention</DisplayName>
               <RetentionId>a1a38957-2557-404e-9f32-53d77c948f62</RetentionId>
               <RetentionPeriod>730</RetentionPeriod>
               <Type>Personal</Type>
               <RetentionAction>DeleteAndAllowRecovery</RetentionAction>
               <Description>Use this tag for all items to be retained for two years.</Description>
               <IsVisible>true</IsVisible>
               <OptedInto>true</OptedInto>
               <IsArchive>false</IsArchive>
            </RetentionPolicyTag>
            <RetentionPolicyTag xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <DisplayName>Default two year move to archive</DisplayName>
               <RetentionId>75bc8dbe-a0e8-4e09-9fa3-fd4c21f49318</RetentionId>
               <RetentionPeriod>730</RetentionPeriod>
               <Type>All</Type>
               <RetentionAction>MoveToArchive</RetentionAction>
               <Description/>
               <IsVisible>false</IsVisible>
               <OptedInto>false</OptedInto>
               <IsArchive>true</IsArchive>
            </RetentionPolicyTag>
         </RetentionPolicyTags>
      </GetUserRetentionPolicyTagsResponse>
   </s:Body>
</s:Envelope>

```

La réponse SOAP body contient les éléments suivants :
  
- [GetUserRetentionPolicyTagsResponse](getuserretentionpolicytagsresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [RetentionPolicyTags](retentionpolicytags.md)
    
- [RetentionPolicyTag](retentionpolicytag.md)
    
- [DisplayName (chaîne)](displayname-string.md)
    
- [RetentionId](retentionid.md)
    
- [RetentionPeriod](retentionperiod.md)
    
- [Type (ElcFolderType)](type-elcfoldertype.md)
    
- [RetentionAction](retentionaction.md)
    
- [Description](description.md)
    
- [IsVisible](isvisible.md)
    
- [OptedInto](optedinto.md)
    
- [IsArchive](isarchive.md)
    
## <a name="getuserretentionpolicytags-operation-error-response"></a>Réponse d’erreur d’opération GetUserRetentionPolicyTags

Pour les codes d’erreur qui sont génériques pour EWS, voir [ResponseCode](responsecode.md).
  
## <a name="see-also"></a>Voir aussi



[Stratégies de rétention dans EWS](http://msdn.microsoft.com/library/a132872f-0228-4bcb-aac2-bf64fb07e58e%28Office.15%29.aspx)


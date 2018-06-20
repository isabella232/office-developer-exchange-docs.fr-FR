---
title: Opération ArchiveItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1af216b3-13ea-498e-b4fc-23513755d731
description: Opération de recherche plus d’informations sur la ArchiveItem EWS.
ms.openlocfilehash: 954943acefef8da61e92de5f8857ca023ca4fc9f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755317"
---
# <a name="archiveitem-operation"></a>Opération ArchiveItem

Trouvez des informations sur l’opération EWS **ArchiveItem** . 
  
L’opération **ArchiveItem** déplace un élément dans la boîte aux lettres d’archive boîte aux lettres. 
  
Cette opération est une nouveauté d’Exchange Server 2013.
  
## <a name="using-the-archiveitem-operation"></a>Utilisation de l’opération ArchiveItem

L’opération **ArchiveItem** prend deux arguments dans la demande qui identifient les éléments à déplacer vers la boîte aux lettres d’archivage et le dossier de destination pour ces éléments. Une boîte aux lettres d’archivage doit être activé pour cette opération travailler. Pour plus d’informations sur la façon d’activer une boîte aux lettres d’archivage, voir [Gérer les Archives locales](http://technet.microsoft.com/en-us/library/jj651146.aspx).
  
### <a name="archiveitem-operation-soap-headers"></a>En-têtes SOAP ArchiveItem opération

L’opération **ArchiveItem** permettre utiliser les en-têtes SOAP qui sont répertoriés dans le tableau suivant. 
  
|**Nom de l'en-tête**|**Élément**|**Description**|
|:-----|:-----|:-----|
|**Emprunt d’identité** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifie l’utilisateur emprunte l’identité de l’application cliente. Cet en-tête est applicable à une demande.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifie la culture, comme défini dans RFC 3066, **des balises pour l’Identification des langues**à utiliser pour accéder à la boîte aux lettres. Cet en-tête est applicable à une demande.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifie la version du schéma pour la requête d’opération. Cet en-tête est applicable à une demande.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifie la version du serveur qui a répondu à la demande. Cet en-tête est applicable à une réponse.  <br/> |
   
## <a name="archiveitem-operation-request-example-move-an-item-to-the-archive-inbox-folder"></a>Exemple de requête d’opération ArchiveItem : déplacer un élément vers le dossier boîte de réception d’archivage

Une requête d’opération **ArchiveItem** l’exemple suivant montre comment déplacer un élément vers le dossier boîte de réception de l’archive. 
  
> [!NOTE]
> Tous les identificateurs d’article et modifier des clés dans cet article ont été réduits afin de préserver la lisibilité. 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013"/>
   </soap:Header>
   <soap:Body>
      <m:ArchiveItem>
         <m:ArchiveSourceFolderId>
            <t:DistinguishedFolderId Id="inbox"/>
         </m:ArchiveSourceFolderId>
         <m:ItemIds>
            <t:ItemId Id="AQMkG5BBwrQAAAxoAAAA=" ChangeKey="CQAAAHCtAAAAAAB7"/>
         </m:ItemIds>
      </m:ArchiveItem>
   </soap:Body>
</soap:Envelope>
```

La demande SOAP body contient les éléments suivants :
  
- [ArchiveItem](archiveitem.md)    
- [ArchiveSourceFolderId](archivesourcefolderid.md)    
- [DistinguishedFolderId](distinguishedfolderid.md)    
- [ItemId](itemids.md)   
- [ID d’élément](itemid.md)
    
## <a name="successful-archiveitem-operation-response"></a>Réponse d’opération ArchiveItem réussie

L’exemple suivant montre une réponse positive à une demande d’opération **ArchiveItem** pour déplacer un élément vers une boîte aux lettres d’archive. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:ArchiveItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                             xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:ArchiveItemResponseMessage ResponseClass="Success">
               <m:ResponseCode>NoError</m:ResponseCode>
               <m:Items/>
            </m:ArchiveItemResponseMessage>
         </m:ResponseMessages>
      </m:ArchiveItemResponse>
   </s:Body>
</s:Envelope>
```

La réponse SOAP body contient les éléments suivants :
  
- [ArchiveItemResponse](archiveitemresponse.md)    
- [ResponseMessages](responsemessages.md)   
- [ArchiveItemResponseMessage](archiveitemresponsemessage.md)    
- [ResponseCode](responsecode.md)    
- [Items](items.md)
    
## <a name="archiveitem-operation-error-response"></a>Réponse d’erreur d’opération ArchiveItem

L’exemple suivant montre une réponse d’erreur à une demande d’opération **ArchiveItem** . Il s’agit d’une réponse à une demande d’archiver un élément lorsqu’une boîte aux lettres d’archivage n’est pas activée pour un utilisateur valide. 
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:ArchiveItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                             xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:ArchiveItemResponseMessage ResponseClass="Error">
               <m:MessageText>Archive mailbox is not enabled for this user.</m:MessageText>
               <m:ResponseCode>ErrorInvalidOperation</m:ResponseCode>
               <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
               <m:Items/>
            </m:ArchiveItemResponseMessage>
         </m:ResponseMessages>
      </m:ArchiveItemResponse>
   </s:Body>
</s:Envelope>
```

La réponse d’erreur corps SOAP contient les éléments suivants :
  
- [ArchiveItemResponse](archiveitemresponse.md)    
- [ResponseMessages](responsemessages.md)    
- [ArchiveItemResponseMessage](archiveitemresponsemessage.md)    
- [MessageText](messagetext.md)    
- [ResponseCode](responsecode.md)    
- [DescriptiveLinkKey](descriptivelinkkey.md)    
- [Items](items.md)
    
Pour les codes d’erreur générique à EWS, spécifiques à cette opération, consultez la rubrique [ResponseCode](responsecode.md).
  
## <a name="see-also"></a>Voir aussi

- [Opérations EWS dans Exchange](ews-operations-in-exchange.md) 
- [L'archivage dans EWS dans Exchange](http://msdn.microsoft.com/library/78ae179b-ae4f-4f64-911a-e0c70e0fa314%28Office.15%29.aspx)
    


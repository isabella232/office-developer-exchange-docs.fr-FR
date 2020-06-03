---
title: Créer des groupes de contacts à l’aide d’EWS dans Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: acec6e73-c016-419d-be1a-8ec5d993addb
description: Découvrez comment créer un groupe de contacts à l’aide de l’API managée EWS ou EWS dans Exchange.
ms.openlocfilehash: 1da876bbda72f5bea08fd9855aa3f554135d54aa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528138"
---
# <a name="create-contact-groups-by-using-ews-in-exchange"></a>Créer des groupes de contacts à l’aide d’EWS dans Exchange

Découvrez comment créer un groupe de contacts à l’aide de l’API managée EWS ou EWS dans Exchange.
  
Vous pouvez créer un groupe de contacts, qui est un [groupe de distribution](distribution-groups-and-ews-in-exchange.md)privé, à l’aide de l’API managée EWS ou d’EWS. Pour créer des groupes de contacts, utilisez les méthodes de la classe de l’API managée EWS [ContactGroup](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.contactgroup%28v=exchg.80%29.aspx) ou utilisez l’opération EWS de [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) . 
  
Notez que vous ne pouvez pas utiliser l’API managée EWS ou EWS pour créer un groupe de distribution ou un groupe de sécurité universel. Pour créer un groupe de distribution universel ou un groupe de sécurité, vous pouvez utiliser la cmdlet [New-DistributionGroup](https://technet.microsoft.com/library/aa998856%28v=exchg.150%29.aspx)[Exchange Management Shell](https://msdn.microsoft.com/library/ff326159%28v=exchg.140%29.aspx). 
  
## <a name="create-a-contact-group-by-using-the-ews-managed-api"></a>Créer un groupe de contacts à l’aide de l’API managée EWS
<a name="bk_EWSMA"> </a>

Pour créer un groupe de contacts, vous avez besoin de quelques informations : un nom pour le groupe et les membres à ajouter au groupe. L’exemple suivant montre comment créer un groupe de contacts simple qui contient deux membres de groupe.
  
```cs
// Create a new contact group object.
ContactGroup myContactGroup = new ContactGroup(service);
// Give the group a name.
myContactGroup.DisplayName = "My Contact Group";
// Add some members to the group.
myContactGroup.Members.Add(new GroupMember("sadie@contoso.com"));
myContactGroup.Members.Add(new GroupMember("alfred@contoso.com"));
// Save the group.
myContactGroup.Save();

```

## <a name="create-a-contact-group-by-using-ews"></a>Créer un groupe de contacts à l’aide d’EWS
<a name="bk_EWSMA"> </a>

Il peut prendre quelques lignes de code supplémentaires, mais vous pouvez créer un groupe de contacts à l’aide de l’opération EWS de [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) . L’exemple de requête XML suivant montre comment vous pouvez créer un groupe de contacts. Il s’agit également de la requête XML qui est envoyée lorsque vous [Utilisez l’API managée EWS pour créer un groupe de contacts](#bk_EWSMA).
  
```XML
<?xml version="1.0" encoding="utf-8"?>
   <CreateItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" 
MessageDisposition="SaveOnly">
      <Items xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
         <DistributionList xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
            <DisplayName xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               My Contact Group
            </DisplayName>
            <Members xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <Member xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
                  <Mailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
                     <EmailAddress xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
                        sadie@contoso.com
                     </EmailAddress>
                  </Mailbox>
               </Member>
               <Member xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
                  <Mailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
                     <EmailAddress xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
                        alfred@contoso.com
                     </EmailAddress>
                  </Mailbox>
               </Member>
            </Members>
         </DistributionList>
      </Items>
   </CreateItem>
```

Voici un exemple de réponse XML réussie à la demande. Notez que les valeurs renvoyées incluent un ID d’élément pour le nouveau groupe de contacts et une clé de modification que vous pouvez utiliser dans un autre code pour modifier le groupe de contacts ou développer le groupe pour afficher les membres. L’ID d’élément est raccourci pour des raisons de lisibilité.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
   <CreateItemResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseMessages xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <CreateItemResponseMessage ResponseClass="Success" 
             xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
            <ResponseCode xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
               NoError
            </ResponseCode>
            <Items xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
               <DistributionList xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
                  <ItemId xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                          Id="AAMkADBlY…" 
                          ChangeKey="EgAAABYAAAAD7hO1SJPWTbICFWZ4U3NMAABXzQiK" />
               </DistributionList>
            </Items>
         </CreateItemResponseMessage>
      </ResponseMessages>
   </CreateItemResponse>
```

## <a name="see-also"></a>Voir aussi


- [Les groupes de distribution et EWS dans Exchange](distribution-groups-and-ews-in-exchange.md)
    
- [Développer des groupes de distribution à l’aide d’EWS dans Exchange 2013](how-to-expand-distribution-groups-by-using-ews-in-exchange-2013.md)
    


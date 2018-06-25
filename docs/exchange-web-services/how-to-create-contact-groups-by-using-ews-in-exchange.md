---
title: Créer des groupes de contacts à l’aide de EWS dans Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: acec6e73-c016-419d-be1a-8ec5d993addb
description: Découvrez comment créer un groupe de contacts à l’aide de l’API managée EWS ou EWS dans Exchange.
ms.openlocfilehash: b3357f24e07a9c1b3b37ccb63b0f4f0d0a1d6fcf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754818"
---
# <a name="create-contact-groups-by-using-ews-in-exchange"></a>Créer des groupes de contacts à l’aide de EWS dans Exchange

Découvrez comment créer un groupe de contacts à l’aide de l’API managée EWS ou EWS dans Exchange.
  
Vous pouvez créer un groupe de contacts, qui est un [groupe de distribution](distribution-groups-and-ews-in-exchange.md)privé, à l’aide de l’API managée EWS ou EWS. Pour créer des groupes de contacts, utilisez les méthodes de la classe d’API managées [ContactGroup](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.contactgroup%28v=exchg.80%29.aspx) , ou l’opération EWS [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) . 
  
Notez que vous ne pouvez pas utiliser les API managées EWS pour créer un groupe de distribution universel ou un groupe de sécurité. Pour créer un groupe de distribution universel ou un groupe de sécurité, vous pouvez utiliser[l’applet de commande Exchange Management Shell](http://msdn.microsoft.com/en-us/library/ff326159%28v=exchg.140%29.aspx)de [New-DistributionGroup](http://technet.microsoft.com/en-us/library/aa998856%28v=exchg.150%29.aspx). 
  
## <a name="create-a-contact-group-by-using-the-ews-managed-api"></a>Créer un groupe de contacts à l’aide de l’API managée EWS
<a name="bk_EWSMA"> </a>

Pour créer un groupe de contacts, vous devez simplement quelques éléments d’information : un nom pour le groupe, ainsi que les membres à ajouter au groupe. L’exemple suivant montre comment créer un groupe de contacts simple qui contient deux membres du groupe.
  
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

## <a name="create-a-contact-group-by-using-ews"></a>Créer un groupe de contacts à l’aide de EWS
<a name="bk_EWSMA"> </a>

Elle peut prendre quelques lignes de code, mais vous pouvez créer un groupe de contacts à l’aide de l’opération EWS [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) . L’exemple de requête XML suivant montre comment vous pouvez créer un groupe de contacts. C’est également la demande XML qui est envoyée lorsque vous [Utilisez l’API managée EWS pour créer un groupe de contacts](#bk_EWSMA).
  
```XML
<?xml version="1.0" encoding="utf-8"?>
   <CreateItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" 
MessageDisposition="SaveOnly">
      <Items xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
         <DistributionList xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
            <DisplayName xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               My Contact Group
            </DisplayName>
            <Members xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <Member xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
                  <Mailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
                     <EmailAddress xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
                        sadie@contoso.com
                     </EmailAddress>
                  </Mailbox>
               </Member>
               <Member xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
                  <Mailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
                     <EmailAddress xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
                        alfred@contoso.com
                     </EmailAddress>
                  </Mailbox>
               </Member>
            </Members>
         </DistributionList>
      </Items>
   </CreateItem>
```

Voici un exemple d’une réponse XML positive à la demande. Notez que les valeurs renvoyées incluent un ID d’élément pour le nouveau groupe de contacts et une clé de modification que vous pouvez utiliser dans un autre code pour modifier le groupe de contacts ou de développer le groupe pour afficher les membres. L’ID de l’élément est réduite pour une meilleure lisibilité.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
   <CreateItemResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseMessages xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <CreateItemResponseMessage ResponseClass="Success" 
             xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
            <ResponseCode xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
               NoError
            </ResponseCode>
            <Items xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
               <DistributionList xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
                  <ItemId xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
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
    
- [Développez les groupes de distribution à l’aide EWS dans Exchange 2013](how-to-expand-distribution-groups-by-using-ews-in-exchange-2013.md)
    


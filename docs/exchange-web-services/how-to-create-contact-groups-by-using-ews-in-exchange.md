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
# <a name="create-contact-groups-by-using-ews-in-exchange"></a><span data-ttu-id="b1e3c-103">Créer des groupes de contacts à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b1e3c-103">Create contact groups by using EWS in Exchange</span></span>

<span data-ttu-id="b1e3c-104">Découvrez comment créer un groupe de contacts à l’aide de l’API managée EWS ou EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="b1e3c-104">Learn how to create a contact group by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="b1e3c-105">Vous pouvez créer un groupe de contacts, qui est un [groupe de distribution](distribution-groups-and-ews-in-exchange.md)privé, à l’aide de l’API managée EWS ou d’EWS.</span><span class="sxs-lookup"><span data-stu-id="b1e3c-105">You can create a contact group, which is a private [distribution group](distribution-groups-and-ews-in-exchange.md), by using the EWS Managed API or EWS.</span></span> <span data-ttu-id="b1e3c-106">Pour créer des groupes de contacts, utilisez les méthodes de la classe de l’API managée EWS [ContactGroup](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.contactgroup%28v=exchg.80%29.aspx) ou utilisez l’opération EWS de [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="b1e3c-106">To create contact groups, use the methods in the [ContactGroup](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.contactgroup%28v=exchg.80%29.aspx) EWS Managed API class, or use the [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS operation.</span></span> 
  
<span data-ttu-id="b1e3c-107">Notez que vous ne pouvez pas utiliser l’API managée EWS ou EWS pour créer un groupe de distribution ou un groupe de sécurité universel.</span><span class="sxs-lookup"><span data-stu-id="b1e3c-107">Note that you can't use the EWS Managed API or EWS to create a universal distribution group or security group.</span></span> <span data-ttu-id="b1e3c-108">Pour créer un groupe de distribution universel ou un groupe de sécurité, vous pouvez utiliser la cmdlet [New-DistributionGroup](https://technet.microsoft.com/library/aa998856%28v=exchg.150%29.aspx)[Exchange Management Shell](https://msdn.microsoft.com/library/ff326159%28v=exchg.140%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="b1e3c-108">To create a universal distribution group or security group, you can use the [New-DistributionGroup](https://technet.microsoft.com/library/aa998856%28v=exchg.150%29.aspx)[Exchange Management Shell cmdlet](https://msdn.microsoft.com/library/ff326159%28v=exchg.140%29.aspx).</span></span> 
  
## <a name="create-a-contact-group-by-using-the-ews-managed-api"></a><span data-ttu-id="b1e3c-109">Créer un groupe de contacts à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="b1e3c-109">Create a contact group by using the EWS Managed API</span></span>
<span data-ttu-id="b1e3c-110"><a name="bk_EWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="b1e3c-110"><a name="bk_EWSMA"> </a></span></span>

<span data-ttu-id="b1e3c-111">Pour créer un groupe de contacts, vous avez besoin de quelques informations : un nom pour le groupe et les membres à ajouter au groupe.</span><span class="sxs-lookup"><span data-stu-id="b1e3c-111">To create a contact group, you just need a couple pieces of information: a name for the group, and the members to add to the group.</span></span> <span data-ttu-id="b1e3c-112">L’exemple suivant montre comment créer un groupe de contacts simple qui contient deux membres de groupe.</span><span class="sxs-lookup"><span data-stu-id="b1e3c-112">The following example shows how to create a simple contact group that contains a couple of group members.</span></span>
  
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

## <a name="create-a-contact-group-by-using-ews"></a><span data-ttu-id="b1e3c-113">Créer un groupe de contacts à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="b1e3c-113">Create a contact group by using EWS</span></span>
<span data-ttu-id="b1e3c-114"><a name="bk_EWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="b1e3c-114"><a name="bk_EWSMA"> </a></span></span>

<span data-ttu-id="b1e3c-115">Il peut prendre quelques lignes de code supplémentaires, mais vous pouvez créer un groupe de contacts à l’aide de l’opération EWS de [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="b1e3c-115">It might take a few more lines of code, but you can create a contact group by using the [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS operation.</span></span> <span data-ttu-id="b1e3c-116">L’exemple de requête XML suivant montre comment vous pouvez créer un groupe de contacts.</span><span class="sxs-lookup"><span data-stu-id="b1e3c-116">The following XML request example shows how you can create a contact group.</span></span> <span data-ttu-id="b1e3c-117">Il s’agit également de la requête XML qui est envoyée lorsque vous [Utilisez l’API managée EWS pour créer un groupe de contacts](#bk_EWSMA).</span><span class="sxs-lookup"><span data-stu-id="b1e3c-117">This is also the XML request that is sent when you [use the EWS Managed API to create a contact group](#bk_EWSMA).</span></span>
  
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

<span data-ttu-id="b1e3c-118">Voici un exemple de réponse XML réussie à la demande.</span><span class="sxs-lookup"><span data-stu-id="b1e3c-118">The following is an example of a successful XML response to the request.</span></span> <span data-ttu-id="b1e3c-119">Notez que les valeurs renvoyées incluent un ID d’élément pour le nouveau groupe de contacts et une clé de modification que vous pouvez utiliser dans un autre code pour modifier le groupe de contacts ou développer le groupe pour afficher les membres.</span><span class="sxs-lookup"><span data-stu-id="b1e3c-119">Notice that the values returned include an item ID for the new contact group and a change key that you can use in other code to modify the contact group or expand the group to see the members.</span></span> <span data-ttu-id="b1e3c-120">L’ID d’élément est raccourci pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="b1e3c-120">The item ID is shortened for readability.</span></span>
  
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

## <a name="see-also"></a><span data-ttu-id="b1e3c-121">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b1e3c-121">See also</span></span>


- [<span data-ttu-id="b1e3c-122">Les groupes de distribution et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b1e3c-122">Distribution groups and EWS in Exchange</span></span>](distribution-groups-and-ews-in-exchange.md)
    
- [<span data-ttu-id="b1e3c-123">Développer des groupes de distribution à l’aide d’EWS dans Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="b1e3c-123">Expand distribution groups by using EWS in Exchange 2013</span></span>](how-to-expand-distribution-groups-by-using-ews-in-exchange-2013.md)
    


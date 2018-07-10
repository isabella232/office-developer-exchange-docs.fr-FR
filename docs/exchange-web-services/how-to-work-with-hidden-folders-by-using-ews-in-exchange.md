---
title: Utilisation de dossiers cachés à l’aide de EWS dans Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 7ae7c045-cd90-4c9f-baf5-0464d5058f45
description: Découvrez comment créer un dossier masqué et les dossiers cachés à l’aide de l’API managée EWS ou EWS dans Exchange.
ms.openlocfilehash: 72efc16ecc247d307b7300526e7d345fe6bdd3ac
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754962"
---
# <a name="work-with-hidden-folders-by-using-ews-in-exchange"></a><span data-ttu-id="6bcc2-103">Utilisation de dossiers cachés à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="6bcc2-103">Work with hidden folders by using EWS in Exchange</span></span>

<span data-ttu-id="6bcc2-104">Découvrez comment créer un dossier masqué et les dossiers cachés à l’aide de l’API managée EWS ou EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="6bcc2-104">Learn how to make a folder hidden and find hidden folders by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="6bcc2-105">Avec une exception, les dossiers à la racine d’une boîte aux lettres Exchange (la sous-arborescence non-IPM) sont masquées à partir de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="6bcc2-105">With one exception, folders in the root of an Exchange mailbox (the non-IPM subtree) are hidden from the user.</span></span> <span data-ttu-id="6bcc2-106">Inversement, tous les dossiers dans le **MsgFolderRoot** (la sous-arborescence IPM) sont visibles par l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="6bcc2-106">Conversely, all folders in the **MsgFolderRoot** (the IPM subtree) are visible to the user.</span></span> <span data-ttu-id="6bcc2-107">Comment masquer un dossier sous le **MsgFolderRoot**?</span><span class="sxs-lookup"><span data-stu-id="6bcc2-107">So how do you hide a folder under the **MsgFolderRoot**?</span></span> <span data-ttu-id="6bcc2-108">Il n’est pas difficile à : il s’agit de seule propriété, la propriété [PidTagAttributeHidden](http://msdn.microsoft.com/fr-fr/library/cc433490%28v=exchg.80%29.aspx) (0x10F4000B) étendu.</span><span class="sxs-lookup"><span data-stu-id="6bcc2-108">It's not that tricky — it comes down to just one property, the [PidTagAttributeHidden](http://msdn.microsoft.com/fr-fr/library/cc433490%28v=exchg.80%29.aspx) (0x10F4000B) extended property.</span></span> <span data-ttu-id="6bcc2-109">Lorsque cette propriété est définie sur **true**, Outlook ou un autre client qui utilise la propriété pour déterminer la visibilité des dossiers masque le dossier d’affichage de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="6bcc2-109">When this property is set to **true**, Outlook or another client that uses the property to determine folder visibility will hide the folder from the user's view.</span></span> <span data-ttu-id="6bcc2-110">Il s’agit d’une propriété étendue, il est plus complexe à utiliser que votre propriété moyenne des dossiers, afin que cet article vous guidera dans les principaux scénarios.</span><span class="sxs-lookup"><span data-stu-id="6bcc2-110">Because this is an extended property, it's more complex to use than your average folder property, so this article will walk you through the main scenarios.</span></span>
  
<span data-ttu-id="6bcc2-111">**Le tableau 1. Méthodes d’API managées et opérations EWS pour travailler avec des dossiers cachés**</span><span class="sxs-lookup"><span data-stu-id="6bcc2-111">**Table 1. EWS Managed API methods and EWS operations for working with hidden folders**</span></span>

|<span data-ttu-id="6bcc2-112">**Tâche**</span><span class="sxs-lookup"><span data-stu-id="6bcc2-112">**Task**</span></span>|<span data-ttu-id="6bcc2-113">**Méthode d'API managée EWS**</span><span class="sxs-lookup"><span data-stu-id="6bcc2-113">**EWS Managed API method**</span></span>|<span data-ttu-id="6bcc2-114">**Opération EWS**</span><span class="sxs-lookup"><span data-stu-id="6bcc2-114">**EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="6bcc2-115">Masquer un dossier</span><span class="sxs-lookup"><span data-stu-id="6bcc2-115">Hide a folder</span></span>  <br/> |<span data-ttu-id="6bcc2-116">[Folder.Bind](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) suivi [Folder.Update](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="6bcc2-116">[Folder.Bind](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) followed by [Folder.Update](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="6bcc2-117">[GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) suivi [UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="6bcc2-117">[GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) followed by [UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx)</span></span> <br/> |
|<span data-ttu-id="6bcc2-118">Dossiers cachés</span><span class="sxs-lookup"><span data-stu-id="6bcc2-118">Find hidden folders</span></span>  <br/> |[<span data-ttu-id="6bcc2-119">FindFolders</span><span class="sxs-lookup"><span data-stu-id="6bcc2-119">FindFolders</span></span>](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="6bcc2-120">FindFolder</span><span class="sxs-lookup"><span data-stu-id="6bcc2-120">FindFolder</span></span>](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> |
   
<span data-ttu-id="6bcc2-121">Vous vous demandez ce qui est la seule exception — autrement dit, quel dossier à la racine est visible pour les utilisateurs ?</span><span class="sxs-lookup"><span data-stu-id="6bcc2-121">Are you wondering what the one exception is — that is, what folder in the root IS visible to users?</span></span> <span data-ttu-id="6bcc2-122">Il est le dossier de recherche (également connu sous la valeur d’énumération **SearchFolders**[WellKnownFolder](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) , ou la valeur de l’élément[DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) **searchfolders**), qui contient les dossiers de recherche des utilisateurs.</span><span class="sxs-lookup"><span data-stu-id="6bcc2-122">It's the Finder folder (also known as the **SearchFolders**[WellKnownFolder](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) enumeration value, or the **searchfolders**[DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) element value), which contains users' search folders.</span></span> <span data-ttu-id="6bcc2-123">Dossiers de recherche créés dans le dossier de recherche sont visibles par les utilisateurs d’Outlook.</span><span class="sxs-lookup"><span data-stu-id="6bcc2-123">Search folders created in the Finder folder are visible to Outlook users.</span></span> <span data-ttu-id="6bcc2-124">Si vous avez besoin créer un dossier de recherche n’est pas visible pour les utilisateurs, la déplacer sous le dossier racine pour le masquer.</span><span class="sxs-lookup"><span data-stu-id="6bcc2-124">If you need to create a search folder that is not visible to users, move it under the root folder to hide it.</span></span> <span data-ttu-id="6bcc2-125">Contrairement à d’autres dossiers, la définition de la propriété **PidTagAttributeHidden** sur **true** ne masque pas un dossier de recherche dans le dossier de recherche.</span><span class="sxs-lookup"><span data-stu-id="6bcc2-125">Unlike for other folders, setting the **PidTagAttributeHidden** property to **true** will not hide a search folder in the Finder folder.</span></span> 
  
## <a name="hide-a-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="6bcc2-126">Masquer un dossier à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="6bcc2-126">Hide a folder by using the EWS Managed API</span></span>
<span data-ttu-id="6bcc2-127"><a name="bk_hideewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="6bcc2-127"></span></span>

<span data-ttu-id="6bcc2-128">Vous pouvez [créer un dossier existant](how-to-work-with-folders-by-using-ews-in-exchange.md#bk_createfolderewsma) un dossier masqué en modifiant le [PidTagAttributeHidden](http://msdn.microsoft.com/fr-fr/library/cc433490%28v=exchg.80%29.aspx) étendu propriété la **valeur true**.</span><span class="sxs-lookup"><span data-stu-id="6bcc2-128">You can [make an existing folder](how-to-work-with-folders-by-using-ews-in-exchange.md#bk_createfolderewsma) a hidden folder by changing the [PidTagAttributeHidden](http://msdn.microsoft.com/fr-fr/library/cc433490%28v=exchg.80%29.aspx) extended property to **true**.</span></span> <span data-ttu-id="6bcc2-129">Tout d’abord, créez une [définition de la propriété étendue pour la propriété](properties-and-extended-properties-in-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="6bcc2-129">First, create an [extended property definition for the property](properties-and-extended-properties-in-ews-in-exchange.md).</span></span> <span data-ttu-id="6bcc2-130">Ensuite, utilisez la méthode [lier](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) pour accéder au dossier, puis mettre à jour la valeur de la propriété **PidTagAttributeHidden** sur true et utilisez la méthode [Update](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) pour enregistrer les modifications.</span><span class="sxs-lookup"><span data-stu-id="6bcc2-130">Next, use the [Bind](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) method to get to the folder, then update the value of the **PidTagAttributeHidden** property to true, and use the [Update](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) method to save the changes.</span></span> 
  
<span data-ttu-id="6bcc2-131">Cet exemple suppose que ce **service** est un valide [ExchangeService](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) d’objet pour le propriétaire de boîte aux lettres, que l’utilisateur a été authentifié sur un serveur Exchange, et ce **folderId** est un [Folder.Id](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) valide qui identifie le dossier masquer.</span><span class="sxs-lookup"><span data-stu-id="6bcc2-131">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for the mailbox owner, that the user has been authenticated to an Exchange server, and that **folderId** is a valid [Folder.Id](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) that identifies the folder to hide.</span></span> 
  
```cs
private static void MakeHidden(FolderId folderId, ExchangeService service)
{
    // Create an extended property definition for the PidTagAttributeHidden property.
    ExtendedPropertyDefinition isHiddenProp = new ExtendedPropertyDefinition(0x10f4, MapiPropertyType.Boolean);
    PropertySet propSet = new PropertySet(isHiddenProp);
    // Bind to a folder and retrieve the PidTagAttributeHidden property.
    Folder folder = Folder.Bind(service, folderId, propSet);
    // Set the PidTagAttributeHidden property to true.
    folder.SetExtendedProperty(isHiddenProp, true);
    // Save the changes.
    folder.Update();
}
```

## <a name="hide-a-folder-by-using-ews"></a><span data-ttu-id="6bcc2-132">Masquer un dossier à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="6bcc2-132">Hide a folder by using EWS</span></span>
<span data-ttu-id="6bcc2-133"><a name="bk_hideews"> </a></span><span class="sxs-lookup"><span data-stu-id="6bcc2-133"></span></span>

<span data-ttu-id="6bcc2-134">Vous pouvez utiliser EWS pour [rendre un dossier existant](how-to-work-with-folders-by-using-ews-in-exchange.md#bk_createfolderewsma) un dossier masqué en modifiant le [PidTagAttributeHidden](http://msdn.microsoft.com/fr-fr/library/cc433490%28v=exchg.80%29.aspx) étendu propriété la **valeur true**.</span><span class="sxs-lookup"><span data-stu-id="6bcc2-134">You can use EWS to [make an existing folder](how-to-work-with-folders-by-using-ews-in-exchange.md#bk_createfolderewsma) a hidden folder by changing the [PidTagAttributeHidden](http://msdn.microsoft.com/fr-fr/library/cc433490%28v=exchg.80%29.aspx) extended property to **true**.</span></span> <span data-ttu-id="6bcc2-135">Tout d’abord, utilisez l’opération de [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) pour accéder au dossier, puis récupérer la propriété **PidTagAttributeHidden** en incluant l’élément [ExtendedFieldURI](http://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) et en définissant la valeur de **PropertyTag** à 4340 et le **PropertyType **valeur de type Boolean.</span><span class="sxs-lookup"><span data-stu-id="6bcc2-135">First, use the [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) operation to get to the folder, then retrieve the **PidTagAttributeHidden** property by including the [ExtendedFieldURI](http://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) element, and setting the **PropertyTag** value to 4340 and the **PropertyType** value to Boolean.</span></span> 
  
<span data-ttu-id="6bcc2-136">C’est également la demande XML qui envoie de l’API managée EWS lorsque vous utilisez la méthode **Bind** pour obtenir un dossier avant de le [rendre un dossier masqué](#bk_hideewsma).</span><span class="sxs-lookup"><span data-stu-id="6bcc2-136">This is also the XML request that the EWS Managed API sends when you use the **Bind** method to get a folder before [making it a hidden folder](#bk_hideewsma).</span></span>
  
<span data-ttu-id="6bcc2-137">La valeur [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) est raccourcie pour une meilleure lisibilité.</span><span class="sxs-lookup"><span data-stu-id="6bcc2-137">The [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) value is shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:GetFolder>
      <m:FolderShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:ExtendedFieldURI PropertyTag="4340"
                              PropertyType="Boolean" />
        </t:AdditionalProperties>
      </m:FolderShape>
      <m:FolderIds>
        <t:FolderId Id="IQywAAAA==" />
      </m:FolderIds>
    </m:GetFolder>
  </soap:Body>
</soap:Envelope>
```

Le serveur répond à la demande **GetFolder** avec un message [GetFolderResponse](http://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) qui contient une valeur élément [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, ce qui indique que le dossier a été récupéré correctement. La réponse inclut également une [valeur](http://msdn.microsoft.com/library/196278d4-5e77-4e0a-8af6-8ac065610510%28Office.15%29.aspx) pour [ExtendedProperty](http://msdn.microsoft.com/library/f9701409-b620-4afe-b9ee-4c1e95507af7%28Office.15%29.aspx). <span data-ttu-id="6bcc2-140">Dans cet exemple, la **valeur** est définie sur **false**, ce qui signifie que le dossier n’est pas actuellement masqué.</span><span class="sxs-lookup"><span data-stu-id="6bcc2-140">In this example, the **Value** is set to **false**, which means that the folder is currently not hidden.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="898"
                         MinorBuildNumber="23"
                         Version="V2_10"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="IQywAAAA=="
                          ChangeKey="AQAAABYAAAD32nSTjepyT63rYH17n9THAAAAABED" />
              <t:ExtendedProperty>
                <t:ExtendedFieldURI PropertyTag="0x10f4"
                                    PropertyType="Boolean" />
                <t:Value>false</t:Value>
              </t:ExtendedProperty>
            </t:Folder>
          </m:Folders>
        </m:GetFolderResponseMessage>
      </m:ResponseMessages>
    </m:GetFolderResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="6bcc2-141">Pour modifier la valeur de **ExtendedProperty** sur true, utilisez l’opération [UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="6bcc2-141">To change the value of the **ExtendedProperty** to true, use the [UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) operation.</span></span> <span data-ttu-id="6bcc2-142">Inclure les éléments **ExtendedProperty**, **ExtendedFieldURI**et la **valeur** pour le **PidTagAttributeHidden** propriété étendue et définissez l’élément de la **valeur** sur **true** masquer le dossier.</span><span class="sxs-lookup"><span data-stu-id="6bcc2-142">Include the **ExtendedProperty**, **ExtendedFieldURI**, and **Value** elements for the **PidTagAttributeHidden** extended property, and set the **Value** element to **true** to hide the folder.</span></span> 
  
<span data-ttu-id="6bcc2-143">C’est également la demande XML qui envoie de l’API managée EWS lorsque vous utilisez la méthode **Update** pour mettre à jour un dossier pour le [rendre un dossier masqué](#bk_hideewsma).</span><span class="sxs-lookup"><span data-stu-id="6bcc2-143">This is also the XML request that the EWS Managed API sends when you use the **Update** method to update a folder to [make it a hidden folder](#bk_hideewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:UpdateFolder>
      <m:FolderChanges>
        <t:FolderChange>
          <t:FolderId Id="IQywAAAA=="
                      ChangeKey="AQAAABYAAAD32nSTjepyT63rYH17n9THAAAAABED" />
          <t:Updates>
            <t:SetFolderField>
              <t:ExtendedFieldURI PropertyTag="4340"
                                  PropertyType="Boolean" />
              <t:Folder>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="4340"
                                      PropertyType="Boolean" />
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:Folder>
            </t:SetFolderField>
          </t:Updates>
        </t:FolderChange>
      </m:FolderChanges>
    </m:UpdateFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="6bcc2-144">Le serveur répond à la demande **UpdateFolder** avec un message [UpdateFolderResponse](http://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) qui contient une valeur élément [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, ce qui indique que le dossier a été correctement mis à jour et est masqué.</span><span class="sxs-lookup"><span data-stu-id="6bcc2-144">The server responds to the **UpdateFolder** request with an [UpdateFolderResponse](http://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the folder was updated successfully, and is now hidden.</span></span>
  
## <a name="find-all-hidden-folders-by-using-the-ews-managed-api"></a><span data-ttu-id="6bcc2-145">Rechercher tous les dossiers cachés à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="6bcc2-145">Find all hidden folders by using the EWS Managed API</span></span>
<span data-ttu-id="6bcc2-146"><a name="bk_findhiddenewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="6bcc2-146"></span></span>

<span data-ttu-id="6bcc2-147">Vous pouvez trouver tous les dossiers cachés dans un dossier parent en créant une [définition de la propriété étendue](properties-and-extended-properties-in-ews-in-exchange.md) pour la **PidTagAttributeHidden** propriété étendue, puis en utilisant la méthode [FindFolders](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) pour rechercher les dossiers avec une ** PidTagAttributeHidden** valeur est définie sur **true**.</span><span class="sxs-lookup"><span data-stu-id="6bcc2-147">You can find all hidden folders under a parent folder by creating an [extended property definition](properties-and-extended-properties-in-ews-in-exchange.md) for the **PidTagAttributeHidden** extended property, and then using the [FindFolders](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) method to find folders with a **PidTagAttributeHidden** value that is set to **true**.</span></span> <span data-ttu-id="6bcc2-148">Cet exemple utilise la MsgFolderRoot, également connu sous le haut de la banque d’informations, ou sous-arbre IPM, en tant que dossier parent pour la recherche sous.</span><span class="sxs-lookup"><span data-stu-id="6bcc2-148">This example uses the MsgFolderRoot, also known as the Top of Information Store, or IPM Subtree, as the parent folder to search under.</span></span>
  
<span data-ttu-id="6bcc2-149">Cet exemple suppose que ce **service** est un objet [ExchangeService](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide pour le propriétaire de boîte aux lettres, et que l’utilisateur a été authentifié sur un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="6bcc2-149">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for the mailbox owner, and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
private static void FindHiddenFolders(ExchangeService service)
{
    // Create an extended property definition for the PidTagAttributeHidden property.
    ExtendedPropertyDefinition isHiddenProp = new ExtendedPropertyDefinition(0x10f4, MapiPropertyType.Boolean);
    // Create a folder view to retrieve up to 100 folders and 
    // retrieve only the PidTagAttributeHidden and the display name.
    FolderView folderView = new FolderView(100);
    folderView.PropertySet = new PropertySet(isHiddenProp, FolderSchema.DisplayName);
    // Indicate a Traversal value of Deep, so that all subfolders are retrieved.
    folderView.Traversal = FolderTraversal.Deep;
    // Find all hidden folders under the MsgFolderRoot.
    // This call results in a FindFolder call to EWS.
    FindFoldersResults findFolder = service.FindFolders(WellKnownFolderName.MsgFolderRoot,
            new SearchFilter.IsEqualTo(isHiddenProp, true), folderView);
    // Display the folder ID and display name of each hidden folder.
    foreach (Folder folder in findFolder)
    {
        Console.WriteLine("FolderId: {0}", folder.Id);
        Console.WriteLine("DisplayName: {0}", folder.DisplayName);
        Console.WriteLine("\r\n");
    }
}
```

## <a name="find-all-hidden-folders-by-using-ews"></a><span data-ttu-id="6bcc2-150">Rechercher tous les dossiers cachés à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="6bcc2-150">Find all hidden folders by using EWS</span></span>
<span data-ttu-id="6bcc2-151"><a name="bk_findhiddenews"> </a></span><span class="sxs-lookup"><span data-stu-id="6bcc2-151"></span></span>

<span data-ttu-id="6bcc2-152">Vous pouvez utiliser EWS pour rechercher tous les dossiers cachés sous un dossier existant en appelant l’opération [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) et recherche de dossiers dont [PidTagAttributeHidden](http://msdn.microsoft.com/fr-fr/library/cc433490%28v=exchg.80%29.aspx) propriété étendue est définie sur **true**.</span><span class="sxs-lookup"><span data-stu-id="6bcc2-152">You can use EWS to find all hidden folders under an existing folder by calling the [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) operation and searching for folders whose [PidTagAttributeHidden](http://msdn.microsoft.com/fr-fr/library/cc433490%28v=exchg.80%29.aspx) extended property is set to **true**.</span></span> <span data-ttu-id="6bcc2-153">Pour ce faire, incluez un [plutôt IsEqualTo](http://msdn.microsoft.com/library/48e7e067-049c-4184-8026-071e6f558e8a%28Office.15%29.aspx)[Restriction](http://msdn.microsoft.com/library/77f19014-d112-4999-8e83-ecc32a117a73%28Office.15%29.aspx) qui recherche l’élément [ExtendedFieldURI](http://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) pour la propriété **PidTagAttributeHidden** (valeur **PropertyTag** 4243 et la valeur **PropertyType** booléenne), comme indiqué dans la requête suivante.</span><span class="sxs-lookup"><span data-stu-id="6bcc2-153">To do this, include an [IsEqualTo](http://msdn.microsoft.com/library/48e7e067-049c-4184-8026-071e6f558e8a%28Office.15%29.aspx)[Restriction](http://msdn.microsoft.com/library/77f19014-d112-4999-8e83-ecc32a117a73%28Office.15%29.aspx) that searches for the [ExtendedFieldURI](http://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) element for the **PidTagAttributeHidden** property ( **PropertyTag** value to 4243 and the **PropertyType** value to Boolean), as shown in the following request.</span></span> <span data-ttu-id="6bcc2-154">Cet exemple utilise la MsgFolderRoot, également connu sous le haut de la banque d’informations, ou sous-arbre IPM, en tant que dossier parent pour la recherche sous.</span><span class="sxs-lookup"><span data-stu-id="6bcc2-154">This example uses the MsgFolderRoot, also known as the Top of Information Store, or IPM Subtree, as the parent folder to search under.</span></span> 
  
<span data-ttu-id="6bcc2-155">C’est également la demande XML qui envoie de l’API managée EWS lorsque vous utilisez la méthode **FindFolders** pour [Rechercher tous les dossiers cachés](#bk_findhiddenewsma).</span><span class="sxs-lookup"><span data-stu-id="6bcc2-155">This is also the XML request that the EWS Managed API sends when you use the **FindFolders** method to [find all hidden folders](#bk_findhiddenewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Central Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:FindFolder Traversal="Deep">
      <m:FolderShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:ExtendedFieldURI PropertyTag="4340"
                              PropertyType="Boolean" />
          <t:FieldURI FieldURI="folder:DisplayName" />
        </t:AdditionalProperties>
      </m:FolderShape>
      <m:IndexedPageFolderView MaxEntriesReturned="100"
                               Offset="0"
                               BasePoint="Beginning" />
      <m:Restriction>
        <t:IsEqualTo>
          <t:ExtendedFieldURI PropertyTag="4340"
                              PropertyType="Boolean" />
          <t:FieldURIOrConstant>
            <t:Constant Value="true" />
          </t:FieldURIOrConstant>
        </t:IsEqualTo>
      </m:Restriction>
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="msgfolderroot" />
      </m:ParentFolderIds>
    </m:FindFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="6bcc2-156">Le serveur répond à la demande **FindFolder** avec un message [FindFolderResponse](http://msdn.microsoft.com/library/f5dd813c-9698-4a39-8fca-3a825df365ed%28Office.15%29.aspx) qui contient une valeur élément [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, ce qui indique que la recherche de dossier a réussi, ainsi que tout le texte masqué dossiers sous le dossier racine des messages.</span><span class="sxs-lookup"><span data-stu-id="6bcc2-156">The server responds to the **FindFolder** request with a [FindFolderResponse](http://msdn.microsoft.com/library/f5dd813c-9698-4a39-8fca-3a825df365ed%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the folder search was successful, as well as all the hidden folders under the root message folder.</span></span>
  
<span data-ttu-id="6bcc2-157">Les valeurs [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) sont limitent pour une meilleure lisibilité.</span><span class="sxs-lookup"><span data-stu-id="6bcc2-157">The [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) values are shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="898"
                         MinorBuildNumber="23"
                         Version="V2_10"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="6"
                        TotalItemsInView="6"
                        IncludesLastItemInRange="true">
            <t:Folders>
              <t:ContactsFolder>
                <t:FolderId Id="IBHgAAAA=="
                            ChangeKey="AwAAABYAAAD32nSTjepyT63rYH17n9THAAAAAACz" />
                <t:DisplayName>{06967759-274D-40B2-A3EB-D7F9E73727D7}</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean" />
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:ContactsFolder>
              <t:ContactsFolder>
                <t:FolderId Id="IBHwAAAA=="
                            ChangeKey="AwAAABYAAAD32nSTjepyT63rYH17n9THAAAAAAC7" />
                <t:DisplayName>{A9E2BC46-B3A0-4243-B315-60D991004455}</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean" />
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:ContactsFolder>
              <t:ContactsFolder>
                <t:FolderId Id="IBIQAAAA=="
                            ChangeKey="AwAAABYAAAD32nSTjepyT63rYH17n9THAAAAAADO" />
                <t:DisplayName>GAL Contacts</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean" />
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:ContactsFolder>
              <t:ContactsFolder>
                <t:FolderId Id="IBHQAAAA=="
                            ChangeKey="AwAAABYAAAD32nSTjepyT63rYH17n9THAAAAAACa" />
                <t:DisplayName>Recipient Cache</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean" />
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:ContactsFolder>
              <t:Folder>
                <t:FolderId Id="HAAAAA=="
                            ChangeKey="AQAAABYAAAD32nSTjepyT63rYH17n9THAAAAAACS" />
                <t:DisplayName>Conversation Action Settings</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean" />
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:Folder>
              <t:Folder>
                <t:FolderId Id="IQywAAAA=="
                            ChangeKey="AQAAABYAAAD32nSTjepyT63rYH17n9THAAAeZIBf" />
                <t:DisplayName>TestFolder</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean" />
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:Folder>
            </t:Folders>
          </m:RootFolder>
        </m:FindFolderResponseMessage>
      </m:ResponseMessages>
    </m:FindFolderResponse>
  </s:Body>
</s:Envelope>
```

## 
<span data-ttu-id="6bcc2-158"><a name="bk_findhiddenews"> </a></span><span class="sxs-lookup"><span data-stu-id="6bcc2-158"></span></span>

<span data-ttu-id="6bcc2-159">Une fois que vous avez masqué ou dossiers non masqués, vous voudrez peut-être obtenir la hiérarchie de dossiers ou [synchroniser la hiérarchie de dossiers](how-to-synchronize-folders-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="6bcc2-159">After you have hidden or unhidden folders, you might want to get the folder hierarchy or [synchronize the folder hierarchy](how-to-synchronize-folders-by-using-ews-in-exchange.md).</span></span> <span data-ttu-id="6bcc2-160">Les exemples qui montrent que comment [obtenir une hiérarchie de dossiers à l’aide de l’API managée EWS](how-to-work-with-folders-by-using-ews-in-exchange.md#bk_getfolderhierarchyewsma) ou [obtenir une hiérarchie de dossiers à l’aide de EWS](how-to-work-with-folders-by-using-ews-in-exchange.md#bk_getfolderhierarchyews) également indiquer les dossiers dans la hiérarchie sont masquées.</span><span class="sxs-lookup"><span data-stu-id="6bcc2-160">The examples that show you how to [get a folder hierarchy by using the EWS Managed API](how-to-work-with-folders-by-using-ews-in-exchange.md#bk_getfolderhierarchyewsma) or [get a folder hierarchy by using EWS](how-to-work-with-folders-by-using-ews-in-exchange.md#bk_getfolderhierarchyews) also indicate which folders in the hierarchy are hidden.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="6bcc2-161">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="6bcc2-161">See also</span></span>


- [<span data-ttu-id="6bcc2-162">Dossiers et éléments dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="6bcc2-162">Folders and items in EWS in Exchange</span></span>](folders-and-items-in-ews-in-exchange.md)
    
- [<span data-ttu-id="6bcc2-163">Utilisation de dossiers à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="6bcc2-163">Work with folders by using EWS in Exchange</span></span>](how-to-work-with-folders-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="6bcc2-164">Utilisation de dossiers de recherche à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="6bcc2-164">Work with search folders by using EWS in Exchange</span></span>](how-to-work-with-search-folders-by-using-ews-in-exchange.md)
    


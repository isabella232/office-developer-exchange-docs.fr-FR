---
title: Les pièces jointes et les services EWS d’Exchange
manager: sethgros
ms.date: 7/11/2016
ms.audience: Developer
localization_priority: Normal
ms.assetid: 8e4289a4-ec9d-4502-9854-c593c95d5f98
description: Découvrez comment des API managées EWS dans Exchange client représente les et les pièces jointes.
ms.openlocfilehash: e4a97873798b8252e6fc14003519ce8a0eab7ec8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754763"
---
# <a name="attachments-and-ews-in-exchange"></a>Les pièces jointes et les services EWS d’Exchange

Découvrez comment des API managées EWS dans Exchange client représente les et les pièces jointes.
  
En règle générale, les pièces jointes sont associés à des éléments de messagerie électronique, mais en fait, tous les éléments EWS : email messages, éléments de calendrier, contacts, tâches, peuvent inclure des pièces jointes.
  
## <a name="types-of-attachments"></a>Types de pièces jointes

EWS catégorise les pièces jointes en deux groupes : les pièces jointes et des pièces jointes d’éléments du fichier.
  
- **Pièces jointes d’élément :** Fortement typé [éléments EWS](folders-and-items-in-ews-in-exchange.md), tels que des messages électroniques et des éléments de calendrier, attachés à un autre élément EWS fortement typé. N’importe quel élément fortement typé qui peut être créé à l’aide de l’API managée EWS ou EWS peut être utilisé en tant que pièce jointe d’un élément. Le contenu de pièce jointe d’un élément est l’élément fortement typé, qui fournit un accès facile à toutes ses propriétés. Pièces jointes d’élément peuvent avoir leurs propres pièces jointes d’élément, une hiérarchie de pièces jointes d’éléments (ou l’imbrication des pièces jointes) possible.
    
- **Les pièces jointes :** N’importe quel fichier, .txt, .jpg, .zip, .pdf, ou même un fichier .msg. Une pièce jointe a uniquement quelques propriétés, y compris le contenu codé en base 64 du fichier. 
    
- **Référencer les pièces jointes :** Une pièce jointe est référencé par un fournisseur de fichier, tel qu’un fichier situé dans le nuage. Une pièce jointe peut être provenant de plusieurs fournisseurs. 
    
Lorsque vous ajoutez ou récupérer les pièces jointes d’un élément, vous allez le faire différemment selon s’il s’agit d’une pièce jointe ou une pièce jointe d’élément. Par exemple, pour ajouter une pièce jointe à un élément, vous pouvez seulement passer à l’emplacement du fichier. Pour ajouter un élément existant en tant que pièce jointe d’un élément, vous avez fait copier les propriétés ou le contenu MIME de l’élément existant vers une nouvelle pièce jointe d’élément ; Vous ne pouvez pas simplement lier à l’élément existant. Pour faire la distinction entre les deux types de pièces jointes est importante. Plus d’informations sur les différences entre les pièces jointes d’éléments et les pièces jointes sont décrits dans les articles [de cette section](#bk_inthissection).
  
## <a name="how-are-attachments-represented-programmatically"></a>Comment sont jointes représentés par programme ?

Pièces jointes sont stockés dans une collection de l’élément EWS. La collection attachments est composée de pièces jointes ou de pièces jointes d’élément. Métadonnées relatives à la collection de pièces jointes sont disponible lorsque vous obtenez un élément à l’aide de la méthode API managées [Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) ou l’opération EWS [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) , mais les appels supplémentaires sont requis pour récupérer le contenu des pièces jointes. 
  
**Le tableau 1. Métadonnées d’élément relative aux pièces jointes**

|**Entité de métadonnées**|**Propriété API managées**|**Élément EWS**|
|:-----|:-----|:-----|
|Indicateur de pièce jointe (ne signale pas les pièces jointes en ligne)  <br/> |[Item.HasAttachments](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.hasattachments%28v=exchg.80%29.aspx) <br/> |[HasAttachments](http://msdn.microsoft.com/library/538b7a85-11d7-4daa-8458-09b540760e8b%28Office.15%29.aspx) <br/> |
|Collection de pièces jointes  <br/> |[Item.Attachments](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.attachments%28v=exchg.80%29.aspx) <br/> |[Pièces jointes](http://msdn.microsoft.com/library/b470e614-34bb-44f0-8790-7ddbdcbbd29d%28Office.15%29.aspx) <br/> |
|ID des pièces jointes  <br/> |[Attachment.Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachment.id%28v=exchg.80%29.aspx) <br/> |[AttachmentId](http://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) <br/> |
   
**Le tableau 2. Entités de pièce jointe**

|**Type de pièce jointe**|**Classe de l’API managée EWS**|**Élément EWS**|
|:-----|:-----|:-----|
|Pièce jointe  <br/> |[FileAttachment](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.fileattachment%28v=exchg.80%29.aspx) <br/> |[FileAttachment](http://msdn.microsoft.com/library/3ecea174-73d1-47fd-8917-6065cef1d565%28Office.15%29.aspx) <br/> |
|Pièce jointe d’élément  <br/> |[ItemAttachment](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemattachment%28v=exchg.80%29.aspx) <br/> [ItemAttachment\<TItem\>](http://msdn.microsoft.com/en-us/library/dd635165%28v=exchg.80%29.aspx) <br/> |[ItemAttachment](http://msdn.microsoft.com/library/089ee599-f45e-46f5-a18a-5cfb3d2851ff%28Office.15%29.aspx) <br/> |
|Pièce jointe de référence  <br/> |[Type complexe ReferenceAttachmentType (EWS)](http://msdn.microsoft.com/library/18bfa012-e903-d7f3-528a-31ccceb65463%28Office.15%29.aspx) <br/> |[ReferenceAttachment](http://msdn.microsoft.com/library/b9bde862-6b75-4a81-8033-00a47be4dc2f%28Office.15%29.aspx) <br/> |
   
## <a name="inline-attachments"></a>Pièces jointes en ligne

Pièces jointes en ligne sont un type spécial de pièce jointe. Les deux pièces jointes et pièces jointes d’éléments peuvent être des pièces jointes en ligne. Une pièce jointe incorporée s’affiche dans le cadre du contenu du corps et conserve sa position par rapport au reste du contenu dans l’élément. 
  
Une pièce jointe est une pièce jointe incorporée si la propriété API managées [IsInline](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachment.isinline%28v=exchg.80%29.aspx) ou l’élément EWS [IsInline](http://msdn.microsoft.com/library/5e7712c8-372a-4a16-be64-360c5ff3961a%28Office.15%29.aspx) est définie sur true. Pièces jointes en ligne utilisent les propriétés facultatives suivantes et les éléments pour identifier l’emplacement d’une pièce jointe incorporée : 
  
- API managées — [ContentId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachment.contentid%28v=exchg.80%29.aspx) ou [ContentLocation](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachment.contentlocation%28v=exchg.80%29.aspx) propriétés. 
    
- EWS — [ContentId](http://msdn.microsoft.com/library/bc59100d-6079-414b-a6e0-7c15feaa3184%28Office.15%29.aspx) ou [ContentLocation](http://msdn.microsoft.com/library/d91cf587-24e3-4c13-8784-5ca29787cca7%28Office.15%29.aspx) élément. 
    
Notez que la propriété API managées [HasAttachments](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.hasattachments%28v=exchg.80%29.aspx) et l’élément EWS [HasAttachments](http://msdn.microsoft.com/library/538b7a85-11d7-4daa-8458-09b540760e8b%28Office.15%29.aspx) ne reflètent pas l’existence des pièces jointes en ligne et qui a pourquoi les pièces jointes en ligne sont également appelées masquée pièces jointes. Si vous définissez la propriété API managées [IsInline](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachment.isinline%28v=exchg.80%29.aspx) ou l’élément EWS [IsInline](http://msdn.microsoft.com/library/5e7712c8-372a-4a16-be64-360c5ff3961a%28Office.15%29.aspx) sur true, et aucune autre pièces jointes, **HasAttachments** a la valeur false. Si votre client utilise **HasAttachments** pour remplir un indicateur de pièce jointe ou l’icône d’un message électronique, n’oubliez pas que l’icône n’apparaît pas pour les courriers électroniques avec les pièces jointes en ligne. 
  
## <a name="in-this-section"></a>Dans cette section
<a name="bk_inthissection"> </a>

- [Ajouter des pièces jointes à l’aide de EWS dans Exchange](how-to-add-attachments-by-using-ews-in-exchange.md)
    
- [Obtenir des pièces jointes à l’aide de EWS dans Exchange](how-to-get-attachments-by-using-ews-in-exchange.md)
    
- [Supprimez les pièces jointes à l’aide de EWS dans Exchange](how-to-delete-attachments-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>Voir aussi
<a name="bk_additionalresources"> </a>

- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)
    
- [Dossiers et éléments dans EWS dans Exchange](folders-and-items-in-ews-in-exchange.md)
    
- [Courrier électronique et les services EWS d'Exchange](email-and-ews-in-exchange.md)
    


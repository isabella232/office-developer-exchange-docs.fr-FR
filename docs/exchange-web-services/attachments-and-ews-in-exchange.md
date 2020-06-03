---
title: Pièces jointes et EWS dans Exchange
manager: sethgros
ms.date: 7/11/2016
ms.audience: Developer
ms.assetid: 8e4289a4-ec9d-4502-9854-c593c95d5f98
description: Découvrez les pièces jointes et comment votre API managée EWS ou EWS dans le client Exchange les représente.
localization_priority: Priority
ms.openlocfilehash: d37fef9ea14a3b42a0eed0240724fe69c8531c93
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528488"
---
# <a name="attachments-and-ews-in-exchange"></a>Pièces jointes et EWS dans Exchange

Découvrez les pièces jointes et comment votre API managée EWS ou EWS dans le client Exchange les représente.
  
En règle générale, les pièces jointes sont associées à des éléments de courrier électronique, mais en fait, tous les éléments EWS (messages électroniques, éléments de calendrier, contacts, tâches) peuvent inclure des pièces jointes.
  
## <a name="types-of-attachments"></a>Types de pièces jointes

EWS classe les pièces jointes en deux groupes : fichiers joints et pièces jointes.
  
- **Pièces jointes d’éléments :** Des [éléments EWS](folders-and-items-in-ews-in-exchange.md)fortement typés, tels que des messages électroniques et des éléments de calendrier, qui sont attachés à un autre élément EWS fortement typé. Tout élément fortement typé pouvant être créé à l’aide de l’API managée EWS ou EWS peut être utilisé en tant que pièce jointe d’un élément. Le contenu d’une pièce jointe d’un élément est l’élément fortement typé, qui permet d’accéder facilement à toutes ses propriétés. Les pièces jointes d’élément peuvent avoir leurs propres pièces jointes, de sorte qu’une hiérarchie de pièces jointes d’éléments (ou l’imbrication de pièces jointes) est possible.
    
- **Pièces jointes :** Tout fichier, par exemple un fichier. txt,. jpg,. zip,. pdf ou même un fichier. msg. Une pièce jointe possède seulement quelques propriétés, dont l’une est le contenu encodé en base 64 du fichier. 
    
- **Pièces jointes de référence :** Toute pièce jointe référencée par un fournisseur de fichiers, telle qu’un fichier situé dans le Cloud. Une pièce jointe peut provenir de plusieurs fournisseurs. 
    
Lorsque vous ajoutez ou récupérez des pièces jointes à partir d’un élément, vous pouvez le faire différemment selon qu’il s’agit d’une pièce jointe de fichier ou d’une pièce jointe d’élément. Par exemple, pour ajouter un fichier en pièce jointe à un élément, vous pouvez simplement transmettre l’emplacement du fichier. Pour ajouter un élément existant en tant que pièce jointe d’un élément, vous devez copier les propriétés ou le contenu MIME de l’élément existant vers une nouvelle pièce jointe d’élément ; vous ne pouvez pas établir une liaison avec l’élément existant. Il est donc important d’établir une distinction entre les deux types de pièces jointes. Vous trouverez plus d’informations sur les différences entre les pièces jointes d’éléments et les pièces jointes dans les articles [de cette section](#bk_inthissection).
  
## <a name="how-are-attachments-represented-programmatically"></a>Comment les pièces jointes sont-elles représentées par programme ?

Les pièces jointes sont stockées dans une collection sur l’élément EWS. La collection attachments est constituée de pièces jointes de fichiers et/ou de pièces jointes d’éléments. Les métadonnées relatives à la collection de pièces jointes sont disponibles lorsque vous obtenez un élément à l’aide de l’élément de l’API managée EWS [. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) ou de l’opération EWS [GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) , mais les appels supplémentaires sont requis pour récupérer le contenu des pièces jointes. 
  
**Tableau 1. Métadonnées d’élément relatives aux pièces jointes**

|**Entité de métadonnées**|**Propriété de l’API managée EWS**|**Élément EWS**|
|:-----|:-----|:-----|
|Indicateur d’attachement (ne marque pas les pièces jointes en ligne)  <br/> |[Item. HasAttachments](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.hasattachments%28v=exchg.80%29.aspx) <br/> |[HasAttachments](https://msdn.microsoft.com/library/538b7a85-11d7-4daa-8458-09b540760e8b%28Office.15%29.aspx) <br/> |
|Collection de pièces jointes  <br/> |[Item. Attachments](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.attachments%28v=exchg.80%29.aspx) <br/> |[Attachments](https://msdn.microsoft.com/library/b470e614-34bb-44f0-8790-7ddbdcbbd29d%28Office.15%29.aspx) <br/> |
|ID des pièces jointes  <br/> |[Attachment.Id](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.attachment.id%28v=exchg.80%29.aspx) <br/> |[AttachmentId](https://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) <br/> |
   
**Tableau 2. Entités de pièces jointes**

|**Type de pièce jointe**|**Classe d’API managée EWS**|**Élément EWS**|
|:-----|:-----|:-----|
|Pièce jointe  <br/> |[FileAttachment](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.fileattachment%28v=exchg.80%29.aspx) <br/> |[FileAttachment](https://msdn.microsoft.com/library/3ecea174-73d1-47fd-8917-6065cef1d565%28Office.15%29.aspx) <br/> |
|Pièce jointe d’élément  <br/> |[ItemAttachment](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemattachment%28v=exchg.80%29.aspx) <br/> [ItemAttachment\<TItem\>](https://msdn.microsoft.com/library/dd635165%28v=exchg.80%29.aspx) <br/> |[ItemAttachment](https://msdn.microsoft.com/library/089ee599-f45e-46f5-a18a-5cfb3d2851ff%28Office.15%29.aspx) <br/> |
|Pièce jointe de référence  <br/> |[ComplexType ReferenceAttachmentType (EWS)](https://msdn.microsoft.com/library/18bfa012-e903-d7f3-528a-31ccceb65463%28Office.15%29.aspx) <br/> |[ReferenceAttachment](https://msdn.microsoft.com/library/b9bde862-6b75-4a81-8033-00a47be4dc2f%28Office.15%29.aspx) <br/> |
   
## <a name="inline-attachments"></a>Pièces jointes en ligne

Les pièces jointes incorporées sont une race spéciale. Les pièces jointes et les pièces jointes des éléments peuvent être des pièces jointes. Une pièce jointe incorporée apparaît dans le corps du contenu et conserve sa position par rapport au reste du contenu de l’élément. 
  
Une pièce jointe est une pièce jointe incorporée si la propriété [IsInline](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.attachment.isinline%28v=exchg.80%29.aspx) de l’API managée EWS ou l’élément [IsInline](https://msdn.microsoft.com/library/5e7712c8-372a-4a16-be64-360c5ff3961a%28Office.15%29.aspx) EWS est définie sur true. Les pièces jointes incorporées utilisent les éléments et les propriétés facultatifs suivants pour identifier l’emplacement d’une pièce jointe incorporée : 
  
- API managée EWS — propriétés [contentid](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.attachment.contentid%28v=exchg.80%29.aspx) ou [ContentLocation](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.attachment.contentlocation%28v=exchg.80%29.aspx) . 
    
- EWS — élément [contentid](https://msdn.microsoft.com/library/bc59100d-6079-414b-a6e0-7c15feaa3184%28Office.15%29.aspx) ou [ContentLocation](https://msdn.microsoft.com/library/d91cf587-24e3-4c13-8784-5ca29787cca7%28Office.15%29.aspx) . 
    
Notez que la propriété [HasAttachments](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.hasattachments%28v=exchg.80%29.aspx) de l’API managée EWS et l’élément EWS [HasAttachments](https://msdn.microsoft.com/library/538b7a85-11d7-4daa-8458-09b540760e8b%28Office.15%29.aspx) ne reflètent pas l’existence de pièces jointes incorporées, et c’est pourquoi les pièces jointes incorporées sont également appelées pièces jointes masquées. Par conséquent, si vous définissez la propriété [IsInline](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.attachment.isinline%28v=exchg.80%29.aspx) de l’API managée EWS ou l’élément [IsInline](https://msdn.microsoft.com/library/5e7712c8-372a-4a16-be64-360c5ff3961a%28Office.15%29.aspx) EWS sur true, et que l’élément n’a pas d’autres pièces jointes, **HasAttachments** prend la valeur false. Si votre client utilise **HasAttachments** pour remplir un indicateur ou une icône de pièce jointe dans un message électronique, sachez que l’icône n’apparaît pas pour les messages électroniques contenant des pièces jointes incorporées. 
  
## <a name="in-this-section"></a>Dans cette section
<a name="bk_inthissection"> </a>

- [Récupérer des pièces jointes à l’aide d’EWS dans Exchange](how-to-add-attachments-by-using-ews-in-exchange.md)
    
- [Récupérer des pièces jointes à l’aide d’EWS dans Exchange](how-to-get-attachments-by-using-ews-in-exchange.md)
    
- [Supprimer des pièces jointes à l'aide de EWS dans Exchange](how-to-delete-attachments-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>Voir aussi
<a name="bk_additionalresources"> </a>

- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)
    
- [Dossiers et éléments dans EWS dans Exchange](folders-and-items-in-ews-in-exchange.md)
    
- [Courrier électronique et les services EWS d'Exchange](email-and-ews-in-exchange.md)
    


---
title: Identificateurs EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 39b6b20b-e081-4347-9e15-9b8cf829fdf0
description: Découvrez les identificateurs dans Exchange et comment vous pouvez les utiliser dans votre API managées et des applications EWS.
ms.openlocfilehash: fbf6d7756f73b1c5d345f3b34deeb7ea8a347986
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353972"
---
# <a name="ews-identifiers-in-exchange"></a>Identificateurs EWS dans Exchange

Découvrez les identificateurs dans Exchange et comment vous pouvez les utiliser dans votre API managées et des applications EWS.
  
Chaque objet dans la banque d’informations Exchange possède un identificateur unique. Vous pouvez utiliser l’identificateur d’un objet pour faire référence à l’objet et pour différencier des autres objets. Les deux identificateurs les plus courantes que vous pouvez utiliser avec sont dossier et les identificateurs de l’élément. 
  
Afin de comprendre les identificateurs et la façon dont ils sont importantes pour votre application, il est utile de comprendre la relation entre les objets dans Exchange. Lorsque votre API managées ou les applications EWS communiquant avec Exchange, vous travaillez avec une hiérarchie d’objets qui inclut une boîte aux lettres, de dossiers et objets d’élément. Un magasin peut être l’une de ces types d’objets. En règle générale, il s’agit d’une boîte aux lettres sur le serveur Exchange, mais il peut également être un dossier public sur le serveur Exchange. (N’oubliez pas que dans Exchange Online, Exchange Online dans le cadre d’Office 365 et les versions d’Exchange commençant par Exchange 2013, les dossiers publics sont tout autre type de boîte aux lettres et non un autre type de banque). Le magasin contient les dossiers et les dossiers contiennent des éléments et chacun de ces dossiers et les éléments possède un identificateur, comme le montre la figure suivante. 
  
**La figure 1. Boîte aux lettres, dossier et la hiérarchie d’élément**

![Illustration montrant la hiérarchie d’objets à partir de la boîte aux lettres. La boîte aux lettres est située au niveau supérieur et le dossier Boîte de réception est situé au niveau suivant. Le diagramme montre un dossier contenant des messages électroniques. Les identificateurs et les touches de modification sont répertoriés pour chaque objet et sont raccourcis.](media/Ex15_Identifier_diagram.png)
  
## <a name="ews-identifiers"></a>Identificateurs EWS
<a name="bk_CommonIdentifiers"> </a>

Identificateurs EWS utilise des dossiers et des éléments sont appelées identificateurs EWS ou EwsIds. EwsIds vous trouverez dans nombreux objets différents dans EWS, mais sont appelées quelque chose de différent pour différents objets. Étant donné que vous pouvez utiliser ces objets dans votre application, vous souhaiterez comprendre comment les identificateurs de ces objets sont liés à la EwsId. 
  
Les identificateurs dans EWS sont applicables à l’API managées également. Dans l’API managée EWS, les identificateurs sont les propriétés des objets et sont gérées en interne pour mapper aux éléments EWS.
  
**Le tableau 1. Identificateurs d’objets dans les services EWS**

|**Objet**|**Identifier**|**Comment le liés à EwsId ?**|
|:-----|:-----|:-----|
|[CalendarItem](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) <br/> |L’élément enfant [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) contient l’identificateur unique de l’élément de calendrier.  <br/> |L’élément enfant [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) est identique à la EwsId de cet élément.  <br/> |
|[ConversationId](http://msdn.microsoft.com/library/d5f1ddb3-9af3-4677-a6ba-111b304a951e%28Office.15%29.aspx) <br/> |L’attribut **Id** contient l’identificateur de la conversation faisant partie de cet élément.  <br/> |L’attribut **Id** est identique à la EwsId de cet élément.  <br/> |
|[AttachmentId](http://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) <br/> |Fournit l’identificateur unique de la pièce jointe. L’attribut [RootItemId](http://msdn.microsoft.com/library/f613c705-17ce-48ce-aa64-4dc2cea25e31%28Office.15%29.aspx) contient l’identificateur unique de l’élément racine du magasin à laquelle la pièce jointe est associée.  <br/> |Pièces jointes peuvent être autres éléments dans la banque d’informations Exchange, auquel cas [AttachmentId](http://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) est identique à la EwsId. Dans tous les cas, le [RootItemId](http://msdn.microsoft.com/library/f613c705-17ce-48ce-aa64-4dc2cea25e31%28Office.15%29.aspx) est une EwsId car il fait référence à un élément dans le magasin.  <br/> |
|[PersonaId](http://msdn.microsoft.com/library/eec3a468-afd5-4d72-a61e-cd1964fb686c%28Office.15%29.aspx) <br/> |L’attribut **Id** renvoie une chaîne qui contient l’identificateur du personnage.  <br/> |L’attribut **Id** est identique à la EwsId pour le personnage.  <br/> |
|[ContactId](http://msdn.microsoft.com/library/86f66275-1e39-48ed-bd89-ac3bffc465a7%28Office.15%29.aspx) <br/> |L’attribut **Id** renvoie une chaîne qui contient l’identificateur du contact.  <br/> |L’attribut **Id** est identique à la EwsId pour le contact.  <br/> |
|[GroupId](http://msdn.microsoft.com/library/656d9b9a-8a65-4a75-8466-5b0d96512dab%28Office.15%29.aspx) <br/> |L’attribut **Id** renvoie une chaîne qui contient l’identificateur du groupe.  <br/> |L’attribut **Id** est identique à la EwsId pour le groupe.  <br/> |
|[AssociatedCalendarItemId](http://msdn.microsoft.com/library/5b29898c-ea59-4e6a-914c-c011ec754032%28Office.15%29.aspx) <br/> |L’attribut **Id** identifie l’élément de calendrier qui est associé à un [MeetingMessage](http://msdn.microsoft.com/library/c95956a8-7505-44b4-bea4-11d1f5182796%28Office.15%29.aspx), [MeetingRequest](http://msdn.microsoft.com/library/c44f8804-a355-473d-a837-48cc91617251%28Office.15%29.aspx), [MeetingResponse](http://msdn.microsoft.com/library/9f798e79-dafd-4d4d-9967-95fd8e5c0502%28Office.15%29.aspx)ou [MeetingCancellation](http://msdn.microsoft.com/library/a9c61f7f-2ecd-4b21-9dce-24d9f61aeeea%28Office.15%29.aspx).  <br/> |L’attribut **Id** est identique à la EwsId pour l’élément de calendrier.  <br/> |
|[UserConfigurationProperties](http://msdn.microsoft.com/library/c143a6ec-62ad-4d48-b844-b1ad88054bc1%28Office.15%29.aspx) <br/> |La valeur de **l’Id** de cet élément spécifie la propriété de l’identificateur.  <br/> |Cet identificateur ne directement correspond à la EwsId puisqu’il un identificateur de la propriété et non un élément.  <br/> |
|[OccurrenceItemId](http://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) <br/> |L’attribut **RecurringMasterId** identifie la forme de base d’un élément périodique.  <br/> |La valeur **OccurrenceItemId** ne correspond pas directement à la EwsId, contrairement à la **RecurringMasterId** car il fait référence à l’objet de niveau supérieur de l’élément périodique.  <br/> |
|[StoreEntryId](http://msdn.microsoft.com/library/f536e264-8c4d-4cc5-bab8-22a4fa38de39%28Office.15%29.aspx) <br/> |Contient l’identificateur de la banque Exchange d’un élément.  <br/> |La valeur **StoreEntryId** ne correspond pas à la EwsId, mais il l’identificateur de la banque dans laquelle les éléments sont conservés.  <br/> |
   
## <a name="working-with-identifiers"></a>Utilisation des identificateurs
<a name="bk_WorkingWithIdentifiers"> </a>

Le serveur Exchange gère les identificateurs d’un lot de différentes manières. Considérez les points suivants lorsque vous développez des applications EWS API managées :
  
- La valeur de l’élément **ItemID** des dossiers et des éléments respecte la casse. Si vous examinez l’ID d’élément d’un dossier ou un élément qui est retourné par l' [opération FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) (ou la méthode d’API managées [FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) ), si vous pensez qu’il est un double d’un autre ID d’élément ; Cependant, un ou plusieurs caractères dans l’élément ID pour les deux éléments auront une casse différente. 
    
- Si vous souhaitez stocker le ID d’élément dans une base de données à récupérer ultérieurement, il est recommandé que la taille du champ à 512 octets, afin qu’il soit suffisante pour contenir le GUID.
    
- Ne supposent que votre ID sera toujours valide si vous avez besoin extraire l’élément à une date ultérieure. Si un élément est déplacé dans le magasin, l’ID peut changer en raison de la manière dont un déplacement est géré. Un élément est copié réellement, et qu’un nouvel ID est généré, puis [l’élément d’origine est supprimé](deleting-items-by-using-ews-in-exchange.md).
    
- Les identificateurs dans Exchange sont opaques. Par exemple, le EwsId est créé à partir de plusieurs éléments d’information qui ne sont pas importantes pour vous en tant que développeur, mais qui sont importantes pour Exchange.
    
- Lorsque vous travaillez avec des éléments dans Exchange, une autre valeur à prendre en compte est l’attribut **ChangeKey** . Cette valeur, en plus de l’ID d’élément, est utilisée pour suivre l’état d’un élément. Chaque fois qu’un élément est modifié, une nouvelle clé de modification est générée. Lorsque vous effectuez une [opération UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx), par exemple, vous pouvez utiliser l’attribut **ChangeKey** pour informer le serveur que votre mise à jour est appliquée à la version la plus récente de l’élément. Si une autre application apporté une modification à l’élément que vous mettez à jour, les touches de modification ne correspondront pas et vous ne pourrez pas effectuer la mise à jour. 
    
## <a name="distinguished-folder-ids"></a>ID de dossier unique
<a name="bk_DistinguishedFolderIds"> </a>

Exchange inclut un nombre de dossiers de boîte aux lettres prédéfinis, chacun d'entre eux se voit attribuer un identificateur, appelé l’ID de dossier unique. Elles sont définies par l’énumération d’API managées [WellKnownFolderName](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) et l’élément EWS [DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) . Vous pouvez utiliser ces ID unique dossier référence plus facilement d’un des dossiers prédéfinis. Par exemple, pour le dossier boîte de réception, vous pouvez simplement utiliser « boîte de réception » pour l’identificateur, plutôt que de déterminer l’identificateur de dossier. 
  
Autres dossiers que vous créez afin d’organiser des éléments de messagerie électronique ont également un ID unique pour ce dossier. Cet ID ne change pas même si vous modifiez d’autres propriétés sur le dossier.
  
Vous pouvez utiliser l’ID de dossier unique comme point d’entrée pour l’accès délégué. Lorsque vous lancez l’accès délégué, vous les éléments ou les dossiers de recherche et fournissez l’ID de dossier unique pour spécifier l’emplacement de la recherche. Lorsqu’un utilisateur délégué accède au serveur, un élément de [boîte aux lettres](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) qui est un enfant de l’élément **DistinguishedFolderId** est utilisé pour spécifier explicitement le délégué pour accéder à la boîte aux lettres. 
  
## <a name="handling-errors"></a>Gestion des erreurs
<a name="bk_DealingWithErrors"> </a>

Chaque programme est lié à obtenir une erreur et et des applications EWS ne font pas exception (jeu de mots). Vous pouvez recevoir des erreurs liées aux identificateur dans l’élément EWS [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) ou dans le cadre de la de l’énumération d’API managées [constatez](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.serviceerror%28v=exchg.80%29.aspx) . 
  
Les erreurs suivantes peuvent se produire dans des applications EWS API managées. Si vous travaillez avec une application d’API managées, les erreurs sont généralement problèmes avec les valeurs de propriété ; pour les applications EWS, les erreurs sont associés avec les valeurs des éléments XML ou des opérations.
  
**Le tableau 2. Erreurs liées aux identificateur**

|**Erreur**|**Cet événement se produit lorsque...**|**Description**|
|:-----|:-----|:-----|
|ErrorCalendarCannotUseIdForOccurrenceId  <br/> |La valeur de **OccurenceID** ne correspond pas à un élément de calendrier périodique valide.  <br/> |La valeur de **OccurenceId** qui a été spécifié dans la demande peut être valide dans la structure, mais la demande ne peut pas faire correspondre à une forme de base périodique existante. L’élément périodique peut être supprimée à partir du calendrier. Vérifiez que l’élément existe toujours et que vous utilisez l’identificateur approprié.  <br/> |
|ErrorCalendarCannotUseIdForRecurringMasterId  <br/> |L’attribut **RecurringMasterId** ne correspond pas à une occurrence de l’élément **ID d’occurrence** valide.  <br/> |La valeur de la **RecurringMasterId** qui a été spécifié dans la demande peut être valide dans la structure, mais la demande ne peut pas faire correspondre à une occurrence de l’élément existante. L’occurrence de l’élément peut être supprimée à partir du calendrier. Vérifiez que l’élément existe toujours et que vous utilisez l’identificateur approprié.  <br/> |
|ErrorCannotUseFolderIdForItemId  <br/> |L' **ID** qui a été passée représente un dossier au lieu d’un élément.  <br/> |L’identificateur peut être valide dans le format, mais pas le serveur n’était attendue pour l’opération. Vérifiez que vous faites référence à l’identificateur approprié pour l’opération.  <br/> |
|ErrorCannotUseItemIdForFolderId  <br/> |L' **ID** qui a été passée dans représente un élément au lieu d’un dossier.  <br/> |L’identificateur peut être valide dans le format, mais pas le serveur n’était attendue pour l’opération. Vérifiez que vous faites référence à **l’ID** correct pour l’opération.  <br/> |
|ErrorChangeKeyRequiredForWriteOperations  <br/> |Une clé de changement valide doit être fournie lorsque vous effectuez certaines opérations de mise à jour.  <br/> |Soit vous avez omis une valeur **ChangeKey** lorsque vous avez demandé une mise à jour ou modifier la clé est incorrecte. Vérifiez que vous disposez de la clé de rechange correct lorsque vous effectuez les opérations de mise à jour.  <br/> |
|ErrorInvalidAttachmentId  <br/> |La pièce jointe est introuvable dans la collection attachments de l’élément.  <br/> |Vous pouvez recevoir ce code de réponse si vous avez un **ID** pièce jointe et puis la pièce jointe est supprimée et que vous essayez d’appeler l' [opération GetAttachment](http://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx) sur l’ID de pièce jointe. Vérifier l’existence de la pièce jointe dans la collection de pièces jointes.  <br/> |
|ErrorInvalidChangeKey  <br/> |Une clé de changement non valide a été passée.  <br/> |Notez que de nombreuses méthodes et opérations ne nécessitent pas une clé de modification à transmettre. Toutefois, si vous ne fournissez pas de clé de modification, il doit être valide, bien qu’il ne dispose pas nécessairement être à jour.  <br/> |
|ErrorInvalidFolderId  <br/> |**L’ID** dossier est endommagé.  <br/> |Vérifiez que vous disposez d’un identificateur valid et correctement mise en forme.  <br/> |
|ErrorInvalidId  <br/> |La structure de la clé **ID** et/ou de modification est incohérente.  <br/> |Exchange a rencontré un problème avec l' **ID** d’une fois qu’il a été analysé. Il peut-être une erreur lors de la conversion. Cela peut se produire, par exemple, si vous avez un **IdFormatType.HexEntryId** pour un élément dans Outlook, mais vous convertissez un raisonnement EwsId il était un format **IdFormatType.EntryId** . Vérifiez que vous utilisez le type de conversion correcte.  <br/> |
|ErrorInvalidIdEmpty  <br/> |L’application spécifiée à un **ID** qui est vide.  <br/> |Votre application passé dans une chaîne vide pour l’identificateur. Vérifiez que vous disposez d’un identificateur valid et correctement mise en forme.  <br/> |
|ErrorInvalidIdMalformed  <br/> |La structure de l' **ID** est incohérente.  <br/> |Exchange a rencontré un problème avec l' **ID** d’une fois qu’il a été analysé. L’ID n’a ne peut-être pas déjà converti correctement. Vérifiez que vous utilisez le type de conversion correcte.  <br/> |
|ErrorInvalidIdMalformedEwsLegacyIdFormat  <br/> |Un dossier ou un élément **ID** qui utilise le format d’Exchange 2007 a été spécifié pour une demande avec une version d’Exchange 2007 SP1 ou version ultérieure.  <br/> |Vous ne pouvez pas utiliser Exchange 2007 ID dans Exchange 2007 SP1 ou version ultérieure demandes. Vous devez utiliser l’opération EWS [ConvertId](http://msdn.microsoft.com/library/47d96cf6-9e2f-4fc0-9682-7258d3fbf918%28Office.15%29.aspx) ou la méthode d’API managées [ConvertId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.convertid%28v=exchg.80%29.aspx) pour convertir en premier.  <br/> |
|ErrorInvalidIdNotAnItemAttachmentId  <br/> |La propriété **AttachmentId** ne fait pas référence à la pièce jointe d’un élément.  <br/> |L’identificateur peut être valide dans le format, mais pas le serveur n’était attendue pour l’opération. Vérifiez que vous faites référence à l’identificateur approprié pour l’opération.  <br/> |
|ErrorInvalidIdReturnedByResolveNames  <br/> |Un contact dans votre boîte aux lettres est endommagé.  <br/> |L’opération EWS [ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) ou la méthode API managées [ResolveName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) renvoyée un ou plusieurs identificateurs, mais ils ne sont pas valides. Vous devrez peut-être recréer le contact.  <br/> |
|ErrorInvalidIdStoreObjectIdTooLong  <br/> |La structure de l' **ID** est incohérente.  <br/> |Exchange a rencontré un problème avec l' **ID** d’une fois qu’il a été analysé. L' **ID** n’a ne peut-être pas déjà converti correctement. Vérifiez que vous utilisez le type de conversion correcte.  <br/> |
|ErrorInvalidIdTooManyAttachmentLevels  <br/> |Les hiérarchies de la pièce jointe dépassent le maximum de 255 niveaux.  <br/> |La valeur de la propriété **AttachmentId** qui a été spécifiée dans la demande peut être valide dans la structure, mais la pièce jointe demandée est trop élevée dans la hiérarchie. Votre code peut a tenté de joindre un élément au-delà de la limite de 255 niveaux.  <br/> |
|ErrorInvalidImContactId  <br/> |Cette erreur peut être renvoyée lorsque le contact est introuvable dans le groupe de messagerie instantanée lorsque vous utilisez l' [opération RemoveImContactFromGroup](http://msdn.microsoft.com/library/a190bbec-c71b-4e6a-880b-55854c724d8c%28Office.15%29.aspx). Cette erreur s’applique aux clients qui ciblent Exchange Online et versions d’Exchange commençant par Exchange 2013.  <br/> |La valeur de la propriété **ContactId** qui a été spécifiée dans la demande peut être valide dans la structure, mais aucun contact dans la boîte aux lettres correspond à cette structure. Le contact a peut-être été supprimé déjà.  <br/> |
|ErrorInvalidImGroupId  <br/> |Cette erreur peut être renvoyée lorsque le groupe est introuvable dans la boîte aux lettres lorsque vous utilisez l' [opération RemoveImGroup](http://msdn.microsoft.com/library/5e788016-68e0-4a3f-9243-03f6b6c6b389%28Office.15%29.aspx). Cette erreur s’applique aux clients qui ciblent Exchange Online et versions d’Exchange commençant par Exchange 2013.  <br/> |La valeur de la propriété **GroupId** qui a été spécifiée dans la demande peut être valide dans la structure, mais pas de groupes dans la boîte aux lettres correspond à cette structure. Le groupe a peut-être été supprimé déjà.  <br/> |
|ErrorInvalidReferenceItem  <br/> |Identificateur de l’élément référencé n’est pas un **MessageType** ou **ExchangeWebServices.CalendarItemTypeType**ou l’une de leurs descendants. L’identificateur d’élément de référence est un objet **CalendarItemType** et l’organisateur essaie de répondre ou répondre à tous.  <br/> |L’identificateur peut être valide dans le format, mais pas le serveur n’était attendue pour l’opération. Vérifiez que vous faites référence à l’identificateur approprié pour l’opération.  <br/> |
|ErrorMissingManagedFolderId  <br/> |La propriété ID de la stratégie, la balise de propriété 0x6732, pour le dossier est manquant.  <br/> |Le dossier est endommagé. Prendre en compte la recréation.  <br/> |
   
## <a name="converting-identifiers"></a>Conversion des identificateurs
<a name="bk_ConvertingIdentifiers"> </a>

Vous devrez peut-être convertir un identificateur d’un format vers un autre. Par exemple, vous devrez peut-être convertir un identificateur extérieur EWS, par exemple un identificateur provient d’une connexion MAPI, dans un format que votre application peut utiliser. Pour ce faire, vous pouvez utiliser l’opération EWS [ConvertId](http://msdn.microsoft.com/library/47d96cf6-9e2f-4fc0-9682-7258d3fbf918%28Office.15%29.aspx) ou la méthode d’API managées [ConvertId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.convertid%28v=exchg.80%29.aspx) . 
  
Par exemple, un propriété EntryID est un identificateur unique généré par la banque de messages MAPI qui est affectée par la banque lorsque l’élément est enregistré. Pour utiliser un EntryID dans votre application, vous devez tout d’abord le convertir en un EwsId. 
  
Outlook Web App utilise sa propre version des identificateurs, appelé OwaId, dans URL pour accéder aux dossiers et éléments. Si votre application a besoin d’accéder aux éléments dans Outlook Web App, vous devez convertir la OwaId un EwsId.
  
Vous pouvez utiliser la méthode ou l’opération **ConvertId** pour convertir l’identificateur de différents formats. 
  
**Le tableau 3. Identificateur convertible formats dans Exchange**

|**Format**|**Description**|
|:-----|:-----|
|EwsLegacyId  <br/> |EwsId qui s’applique à Exchange 2007.  <br/> |
|EwsId  <br/> |EwsId qui s’applique à Exchange Online et versions d’Exchange commençant par Exchange 2007 SP1.  <br/> |
|StoreId  <br/> |Identificateur de la banque Exchange où sont stockés les dossiers et éléments.  <br/> |
|OwaId  <br/> |L’identificateur d’Outlook Web App utilisé avec Outlook Web App dans Exchange 2007 et Exchange 2010. <br/><br/>**Remarque**: Exchange Online et versions d’Exchange commençant par Exchange 2013 utilisent le EwsId pour Outlook Web App.           |
|Propriété EntryId  <br/> |Un identificateur MAPI est connu en tant que la propriété **PR_ENTRYID** d’un message MAPI.  <br/> |
|HexEntryId  <br/> |Représentation de la propriété **PR_ENTRYID** qui est utilisée pour l’identificateur d’événement disponibilité calendrier codé en hexadécimal. C’est également le format d’identificateur qui utilise Outlook.  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)  
- [Opération ConvertId](http://msdn.microsoft.com/library/47d96cf6-9e2f-4fc0-9682-7258d3fbf918%28Office.15%29.aspx)  
- [Énumération constatez](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.serviceerror%28v=exchg.80%29.aspx) 
- [Suppression d’éléments à l’aide de EWS dans Exchange](deleting-items-by-using-ews-in-exchange.md)
    


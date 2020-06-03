---
title: Identificateurs EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 39b6b20b-e081-4347-9e15-9b8cf829fdf0
description: Découvrez les identificateurs dans Exchange et comment vous pouvez les utiliser dans votre API managée EWS et vos applications EWS.
localization_priority: Priority
ms.openlocfilehash: 9fa2e31a3c67b0b4291b1e3f32a775655e2bf80a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528425"
---
# <a name="ews-identifiers-in-exchange"></a>Identificateurs EWS dans Exchange

Découvrez les identificateurs dans Exchange et comment vous pouvez les utiliser dans votre API managée EWS et vos applications EWS.
  
Chaque objet de la Banque d’Exchange a un identificateur unique. Vous pouvez utiliser l’identificateur d’un objet pour faire référence à l’objet et le différencier des autres objets. Les deux identificateurs les plus courants que vous pouvez utiliser sont les identificateurs de dossier et d’élément. 
  
Pour comprendre les identificateurs et la façon dont ils sont importants pour votre application, il est utile de comprendre la relation entre les objets dans Exchange. Lorsque votre API managée EWS ou votre application EWS communique avec Exchange, vous travaillez avec une hiérarchie d’objets qui inclut des objets boîte aux lettres, dossier et élément. Un magasin peut être l’un de ces types d’objet. Le plus souvent, il s’agit d’une boîte aux lettres sur le serveur Exchange, mais il peut également s’agir d’un dossier public sur le serveur Exchange. (Gardez à l’esprit que dans Exchange Online, Exchange Online dans le cadre d’Office 365 et versions d’Exchange à partir d’Exchange 2013, les dossiers publics sont simplement un autre type de boîte aux lettres et non un autre type de banque.) Le magasin contient des dossiers et les dossiers contiennent des éléments, et chacun de ces dossiers et éléments a un identificateur, comme illustré dans la figure suivante. 
  
**Figure 1. Hiérarchie de boîtes aux lettres, de dossiers et d’éléments**

![Illustration montrant la hiérarchie d’objets à partir de la boîte aux lettres. La boîte aux lettres est située au niveau supérieur et le dossier Boîte de réception est situé au niveau suivant. Le diagramme montre un dossier contenant des messages électroniques. Les identificateurs et les touches de modification sont répertoriés pour chaque objet et sont raccourcis.](media/Ex15_Identifier_diagram.png)
  
## <a name="ews-identifiers"></a>Identificateurs EWS
<a name="bk_CommonIdentifiers"> </a>

Les identificateurs utilisés par EWS pour les dossiers et les éléments sont appelés identificateurs EWS ou EwsIds. Les EwsIds peuvent être trouvés dans de nombreux objets différents dans EWS, mais sont appelés différemment pour différents objets. Étant donné que vous pouvez utiliser ces objets dans votre application, vous devez comprendre la relation entre les identificateurs de ces objets et EwsId. 
  
Les identificateurs dans EWS sont également applicables à l’API managée EWS. Dans l’API managée EWS, les identificateurs sont les propriétés des objets et sont gérés en interne pour être mappés aux éléments EWS.
  
**Tableau 1. Identificateurs d’objets dans EWS**

|**Object**|**Identifiant**|**Comment se rapporte-t-il à EwsId ?**|
|:-----|:-----|:-----|
|[CalendarItem](https://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) <br/> |L’élément enfant [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) contient l’identificateur unique de l’élément de calendrier.  <br/> |L’élément enfant [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) est le même que le EwsId de cet élément.  <br/> |
|[ConversationId](https://msdn.microsoft.com/library/d5f1ddb3-9af3-4677-a6ba-111b304a951e%28Office.15%29.aspx) <br/> |L’attribut **ID** contient l’identificateur de la conversation dont cet élément fait partie.  <br/> |L’attribut **ID** est le même que le EwsId de cet élément.  <br/> |
|[AttachmentId](https://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) <br/> |Fournit l’identificateur unique de la pièce jointe. L’attribut [RootItemId](https://msdn.microsoft.com/library/f613c705-17ce-48ce-aa64-4dc2cea25e31%28Office.15%29.aspx) contient l’identificateur unique de l’élément de magasin racine auquel la pièce jointe est attachée.  <br/> |Les pièces jointes peuvent être des autres éléments de la Banque d’Exchange, auquel cas le [attachmentid](https://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) est le même que le EwsId. Dans tous les cas, [RootItemId](https://msdn.microsoft.com/library/f613c705-17ce-48ce-aa64-4dc2cea25e31%28Office.15%29.aspx) est un EwsId, car il fait référence à un élément dans le magasin.  <br/> |
|[PersonaId](https://msdn.microsoft.com/library/eec3a468-afd5-4d72-a61e-cd1964fb686c%28Office.15%29.aspx) <br/> |L’attribut **ID** renvoie une chaîne qui contient l’identificateur du personnage.  <br/> |L’attribut **ID** est le même que le EwsId pour le personnage.  <br/> |
|[Mettez](https://msdn.microsoft.com/library/86f66275-1e39-48ed-bd89-ac3bffc465a7%28Office.15%29.aspx) <br/> |L’attribut **ID** renvoie une chaîne qui contient l’identificateur du contact.  <br/> |L’attribut **ID** est le même que le EwsId pour le contact.  <br/> |
|[GroupId](https://msdn.microsoft.com/library/656d9b9a-8a65-4a75-8466-5b0d96512dab%28Office.15%29.aspx) <br/> |L’attribut **ID** renvoie une chaîne qui contient l’identificateur du groupe.  <br/> |L’attribut **ID** est le même que le EwsId pour le groupe.  <br/> |
|[AssociatedCalendarItemId](https://msdn.microsoft.com/library/5b29898c-ea59-4e6a-914c-c011ec754032%28Office.15%29.aspx) <br/> |L’attribut **ID** identifie l’élément de calendrier associé à un [MeetingMessage](https://msdn.microsoft.com/library/c95956a8-7505-44b4-bea4-11d1f5182796%28Office.15%29.aspx), [propriété meetingrequest](https://msdn.microsoft.com/library/c44f8804-a355-473d-a837-48cc91617251%28Office.15%29.aspx), [MeetingResponse](https://msdn.microsoft.com/library/9f798e79-dafd-4d4d-9967-95fd8e5c0502%28Office.15%29.aspx)ou [MeetingCancellation](https://msdn.microsoft.com/library/a9c61f7f-2ecd-4b21-9dce-24d9f61aeeea%28Office.15%29.aspx).  <br/> |L’attribut **ID** est le même que le EwsId pour l’élément de calendrier.  <br/> |
|[UserConfigurationProperties](https://msdn.microsoft.com/library/c143a6ec-62ad-4d48-b844-b1ad88054bc1%28Office.15%29.aspx) <br/> |La valeur **ID** de cet élément spécifie la propriété identifier.  <br/> |Cet identificateur ne correspond pas directement au EwsId, car il s’agit d’un identificateur de propriété et non d’un élément.  <br/> |
|[OccurrenceItemId](https://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) <br/> |L’attribut **recurringMasterId** identifie la forme de base d’un élément périodique.  <br/> |La valeur **OccurrenceItemId** ne correspond pas directement à EwsId, mais **recurringMasterId** ne fait pas référence à l’objet de niveau supérieur de l’élément périodique.  <br/> |
|[StoreEntryId](https://msdn.microsoft.com/library/f536e264-8c4d-4cc5-bab8-22a4fa38de39%28Office.15%29.aspx) <br/> |Contient l’identificateur de la banque Exchange d’un élément.  <br/> |La valeur **StoreEntryId** ne correspond pas à EwsId, mais elle donne l’identificateur de la banque où les éléments sont conservés.  <br/> |
   
## <a name="working-with-identifiers"></a>Utilisation des identificateurs
<a name="bk_WorkingWithIdentifiers"> </a>

Le serveur Exchange gère les identificateurs de différentes manières. Tenez compte des éléments suivants lorsque vous développez votre API managée EWS ou votre application EWS :
  
- La valeur de l’élément **ItemId** pour les dossiers et les éléments est sensible à la casse. Si vous examinez l’ID d’élément pour un dossier ou un élément qui est renvoyé par l' [opération FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) (ou la méthode de l’API managée EWS [FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) ), vous pouvez penser qu’il s’agit d’un doublon d’un autre ID d’élément ; Toutefois, un ou plusieurs caractères dans les ID d’élément pour les deux éléments auront un cas différent. 
    
- Si vous envisagez de stocker l’ID d’élément dans une base de données pour le récupérer plus tard, nous vous recommandons d’utiliser une taille de champ de 512 octets, afin qu’elle soit suffisamment élevée pour contenir le GUID.
    
- Ne partez pas du principe que votre ID d’élément sera toujours valide si vous devez récupérer l’élément ultérieurement. Si un élément est déplacé dans le magasin, l’ID peut être modifié en raison de la gestion d’un déplacement. Un élément est en fait copié et un nouvel ID est généré, puis [l’élément d’origine est supprimé](deleting-items-by-using-ews-in-exchange.md). Notez que les ID de dossier sont immuables et ne changent pas lorsqu’ils sont déplacés dans la Banque.
    
- Les identificateurs dans Exchange sont opaques. Par exemple, le EwsId est créé à partir de plusieurs informations qui ne sont pas importantes pour vous en tant que développeur, mais qui sont importantes pour Exchange.
    
- Lorsque vous travaillez avec des éléments dans Exchange, une autre valeur à garder à l’esprit est l’attribut **ChangeKey** . Cette valeur, en plus de l’ID d’élément, est utilisée pour effectuer le suivi de l’état d’un élément. Chaque fois qu’un élément est modifié, une nouvelle clé de modification est générée. Lorsque vous effectuez une [opération UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx), par exemple, vous pouvez utiliser l’attribut **ChangeKey** pour informer le serveur que votre mise à jour est appliquée à la version la plus récente de l’élément. Si une autre application a apporté une modification à l’élément que vous mettez à jour, les clés de modification ne correspondent pas et vous ne pouvez pas effectuer la mise à jour. 
    
## <a name="distinguished-folder-ids"></a>Identificateurs de dossiers uniques
<a name="bk_DistinguishedFolderIds"> </a>

Exchange comprend un certain nombre de dossiers de boîte aux lettres prédéfinis, chacun d’eux étant affecté d’un identificateur, appelé ID de dossier unique. Celles-ci sont définies par l’énumération d’API managée EWS [WellKnownFolderName](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) et l’élément [DistinguishedFolderId](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) EWS. Vous pouvez utiliser ces ID de dossiers uniques pour faire référence plus facilement à l’un des dossiers prédéfinis. Par exemple, pour le dossier boîte de réception, vous pouvez simplement utiliser « boîte de réception » pour l’identificateur, plutôt que de déterminer l’identificateur du dossier. 
  
Les autres dossiers que vous créez pour organiser les éléments de courrier électronique ont également un ID propre à ce dossier. Cet ID ne change pas même si vous modifiez les autres propriétés du dossier.
  
Vous pouvez utiliser des identificateurs de dossiers uniques comme point d’entrée pour l’accès délégué. Lorsque vous lancez l’accès délégué, vous recherchez des éléments ou des dossiers et fournissez l’ID de dossier distinctif pour spécifier l’emplacement de la recherche. Lorsqu’un utilisateur délégué accède au serveur, un élément de [boîte aux lettres](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) qui est un enfant de l’élément **DistinguishedFolderId** est utilisé pour spécifier explicitement la boîte aux lettres pour laquelle le délégué peut accéder. 
  
## <a name="handling-errors"></a>Gestion des erreurs
<a name="bk_DealingWithErrors"> </a>

Chaque programme est lié pour obtenir une erreur toutes les fois, et alors, et les applications EWS ne sont pas des exceptions (PUN). Il se peut que vous receviez des erreurs liées à l’identificateur dans l’élément [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) EWS ou dans le cadre de l’énumération de l’API managée EWS [ServiceError](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.serviceerror%28v=exchg.80%29.aspx) . 
  
Les erreurs suivantes peuvent se produire dans votre API managée EWS ou votre application EWS. Si vous utilisez une application d’API managée EWS, les erreurs sont généralement liées à des valeurs de propriété ; pour les applications EWS, les erreurs sont associées à des opérations ou des valeurs d’éléments XML.
  
**Tableau 2. Erreurs liées à l’identificateur**

|**Error**|**Se produit quand...**|**Description**|
|:-----|:-----|:-----|
|ErrorCalendarCannotUseIdForOccurrenceId  <br/> |La valeur de **OccurenceID** ne correspond pas à un élément de calendrier périodique valide.  <br/> |La valeur du **OccurenceId** qui a été spécifié dans la requête peut être valide dans structure, mais la demande ne peut pas la faire correspondre à une forme de base périodique existante. L’élément périodique peut être supprimé du calendrier. Vérifiez que l’élément existe toujours et que vous utilisez l’identificateur correct.  <br/> |
|ErrorCalendarCannotUseIdForRecurringMasterId  <br/> |L’attribut **recurringMasterId** ne correspond pas à une occurrence valide de l’élément **OccurrenceId** .  <br/> |La valeur du **recurringMasterId** qui a été spécifié dans la requête peut être valide dans structure, mais la requête ne peut pas la faire correspondre à une occurrence existante de l’élément. L’occurrence de l’élément peut être supprimée du calendrier. Vérifiez que l’élément existe toujours et que vous utilisez l’identificateur correct.  <br/> |
|ErrorCannotUseFolderIdForItemId  <br/> |L' **ID** passé représente un dossier au lieu d’un élément.  <br/> |L’identificateur peut être valide dans un format, mais pas avec le serveur attendu pour l’opération. Vérifiez que vous référencez l’identificateur correct pour l’opération.  <br/> |
|ErrorCannotUseItemIdForFolderId  <br/> |L' **ID** passé représente un élément au lieu d’un dossier.  <br/> |L’identificateur peut être valide dans un format, mais pas avec le serveur attendu pour l’opération. Vérifiez que vous référencez l' **ID** correct pour l’opération.  <br/> |
|ErrorChangeKeyRequiredForWriteOperations  <br/> |Une clé de modification valide doit être fournie lorsque vous effectuez certaines opérations de mise à jour.  <br/> |Soit vous avez omis une valeur **ChangeKey** lorsque vous avez demandé une mise à jour, soit la clé de modification était incorrecte. Vérifiez que vous disposez de la clé de modification correcte lorsque vous effectuez des opérations de mise à jour.  <br/> |
|ErrorInvalidAttachmentId  <br/> |La pièce jointe est introuvable dans la collection de pièces jointes de l’élément.  <br/> |Vous pouvez recevoir ce code de réponse si vous avez un **ID** de pièce jointe, puis que la pièce jointe est supprimée et que vous essayez d’appeler l' [opération GETATTACHMENT](https://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx) sur l’ID de pièce jointe. Vérifiez que la pièce jointe existe dans la collection de pièces jointes.  <br/> |
|ErrorInvalidChangeKey  <br/> |Une clé de modification non valide a été transmise.  <br/> |Notez que de nombreuses opérations et méthodes ne nécessitent pas qu’une clé de modification soit passée. Toutefois, si vous fournissez une clé de modification, celle-ci doit être valide, bien qu’elle ne doit pas nécessairement être à jour.  <br/> |
|ErrorInvalidFolderId  <br/> |L' **ID** de dossier est endommagé.  <br/> |Vérifiez que vous disposez d’un identificateur correctement formaté et valide.  <br/> |
|ErrorInvalidId  <br/> |La structure de l' **ID** et/ou de la clé de modification est incohérente en interne.  <br/> |Exchange a rencontré un problème avec l' **ID** après qu’il a été analysé. Une erreur est peut-être survenue lors de la conversion. Cela peut se produire, par exemple, si vous avez un **IdFormatType. HexEntryId** pour un élément dans Outlook, mais que vous le convertissez en EwsId pensant qu’il s’agissait d’un format **IdFormatType. EntryID** . Assurez-vous que vous utilisez le type de conversion approprié.  <br/> |
|ErrorInvalidIdEmpty  <br/> |L’application a spécifié un **ID** qui est vide.  <br/> |Votre application a passé une chaîne vide pour l’identificateur. Vérifiez que vous disposez d’un identificateur correctement formaté et valide.  <br/> |
|ErrorInvalidIdMalformed  <br/> |La structure de l' **ID** est incohérente en interne.  <br/> |Exchange a rencontré un problème avec l' **ID** après qu’il a été analysé. L’ID n’a peut-être pas été converti correctement. Assurez-vous que vous utilisez le type de conversion approprié.  <br/> |
|ErrorInvalidIdMalformedEwsLegacyIdFormat  <br/> |Un dossier ou un **ID** d’élément qui utilise le format Exchange 2007 a été spécifié pour une demande avec une version d’Exchange 2007 SP1 ou version ultérieure.  <br/> |Vous ne pouvez pas utiliser les ID Exchange 2007 dans les requêtes Exchange 2007 SP1 ou version ultérieure. Vous devez utiliser l’opération EWS [ConvertId](https://msdn.microsoft.com/library/47d96cf6-9e2f-4fc0-9682-7258d3fbf918%28Office.15%29.aspx) ou la méthode de l’API managée EWS [ConvertId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.convertid%28v=exchg.80%29.aspx) pour les convertir en premier.  <br/> |
|ErrorInvalidIdNotAnItemAttachmentId  <br/> |La propriété **attachmentid** ne fait pas référence à une pièce jointe d’élément.  <br/> |L’identificateur peut être valide dans un format, mais pas avec le serveur attendu pour l’opération. Vérifiez que vous référencez l’identificateur correct pour l’opération.  <br/> |
|ErrorInvalidIdReturnedByResolveNames  <br/> |Un contact dans votre boîte aux lettres est endommagé.  <br/> |L’opération EWS [ResolveNames](https://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) ou la méthode de l’API managée EWS [ResolveName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) a renvoyé un ou plusieurs identificateurs, mais ils ne sont pas valides. Vous devrez peut-être recréer le contact.  <br/> |
|ErrorInvalidIdStoreObjectIdTooLong  <br/> |La structure de l' **ID** est incohérente en interne.  <br/> |Exchange a rencontré un problème avec l' **ID** après qu’il a été analysé. L' **ID** n’a peut-être pas été converti correctement. Assurez-vous que vous utilisez le type de conversion approprié.  <br/> |
|ErrorInvalidIdTooManyAttachmentLevels  <br/> |Les hiérarchies des pièces jointes dépassent le nombre maximal de 255 niveaux.  <br/> |La valeur de la propriété **attachmentid** qui a été spécifiée dans la requête peut être valide dans structure, mais la pièce jointe demandée est trop imbriquée dans la hiérarchie. Votre code a peut-être essayé d’attacher un élément au-delà de la limite de 255 niveaux.  <br/> |
|ErrorInvalidImContactId  <br/> |Cette erreur peut être renvoyée lorsque le contact est introuvable dans le groupe de messagerie instantanée lorsque vous utilisez l' [opération RemoveImContactFromGroup](https://msdn.microsoft.com/library/a190bbec-c71b-4e6a-880b-55854c724d8c%28Office.15%29.aspx). Cette erreur s’applique aux clients qui ciblent Exchange Online et les versions d’Exchange à partir d’Exchange 2013.  <br/> |La valeur de la propriété **ContactID** qui a été spécifiée dans la requête peut être valide dans structure, mais aucun contact dans la boîte aux lettres ne correspond à cette structure. Le contact a peut-être déjà été supprimé.  <br/> |
|ErrorInvalidImGroupId  <br/> |Cette erreur peut être renvoyée lorsque le groupe est introuvable dans la boîte aux lettres lorsque vous utilisez l' [opération RemoveImGroup](https://msdn.microsoft.com/library/5e788016-68e0-4a3f-9243-03f6b6c6b389%28Office.15%29.aspx). Cette erreur s’applique aux clients qui ciblent Exchange Online et les versions d’Exchange à partir d’Exchange 2013.  <br/> |La valeur de la propriété **GroupID** spécifiée dans la requête peut être valide dans structure, mais aucun groupe de la boîte aux lettres ne correspond à cette structure. Le groupe a peut-être déjà été supprimé.  <br/> |
|ErrorInvalidReferenceItem  <br/> |L’identificateur de l’élément référencé n’est pas un **MessageType** ou **ExchangeWebServices. CalendarItemTypeType**, ou l’un de ses descendants. L’identificateur d’élément de référence est destiné à un objet **CalendarItemType** et l’organisateur essaie de répondre ou ReplyAll.  <br/> |L’identificateur peut être valide dans un format, mais pas avec le serveur attendu pour l’opération. Vérifiez que vous référencez l’identificateur correct pour l’opération.  <br/> |
|ErrorMissingManagedFolderId  <br/> |La propriété ID de stratégie, balise de propriété 0x6732, pour le dossier est manquante.  <br/> |Le dossier est endommagé. Envisagez de le recréer.  <br/> |
   
## <a name="converting-identifiers"></a>Conversion des identificateurs
<a name="bk_ConvertingIdentifiers"> </a>

Vous devrez peut-être convertir un identificateur d’un format à un autre. Par exemple, vous pouvez être amené à convertir un identificateur en dehors d’EWS, comme un identificateur provenant d’une connexion MAPI, vers un format que votre application peut utiliser. Pour ce faire, vous pouvez utiliser l’opération EWS [ConvertId](https://msdn.microsoft.com/library/47d96cf6-9e2f-4fc0-9682-7258d3fbf918%28Office.15%29.aspx) ou la méthode de l’API managée EWS [ConvertId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.convertid%28v=exchg.80%29.aspx) . 
  
Par exemple, un EntryID est un identificateur unique généré par le magasin de messages MAPI qui est affecté par le magasin lors de l’enregistrement de l’élément. Pour utiliser un EntryID dans votre application, vous devez d’abord le convertir en EwsId. 
  
Outlook Web App utilise sa propre version d’identificateurs, appelée OwaId, dans les URL pour accéder aux dossiers et aux éléments. Si votre application a besoin d’accéder aux éléments dans Outlook Web App, vous devez convertir OwaId en EwsId.
  
Vous pouvez utiliser l’opération ou la méthode **ConvertId** pour convertir plusieurs formats d’identificateur. 
  
**Tableau 3. Formats d’identificateur convertible dans Exchange**

|**Format**|**Description**|
|:-----|:-----|
|EwsLegacyId  <br/> |EwsId qui s’applique à Exchange 2007.  <br/> |
|EwsId  <br/> |EwsId qui s’applique à Exchange Online et aux versions d’Exchange à partir d’Exchange 2007 SP1.  <br/> |
|StoreId  <br/> |Identificateur de la banque Exchange où sont stockés les dossiers et les éléments.  <br/> |
|OwaId  <br/> |Identificateur Outlook Web App utilisé avec Outlook Web App dans Exchange 2007 et Exchange 2010. <br/><br/>**Remarque**: Exchange Online et les versions d’Exchange commençant par Exchange 2013 utilisent le EwsId pour Outlook Web App.           |
|Entrée  <br/> |Identificateur MAPI communément appelé la propriété **PR_ENTRYID** d’un message MAPI.  <br/> |
|HexEntryId  <br/> |Une représentation codée en hexadécimal de la propriété **PR_ENTRYID** utilisée pour l’identificateur d’événement de calendrier de disponibilité. Il s’agit également du format d’identificateur utilisé par Outlook.  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)  
- [Opération ConvertId](https://msdn.microsoft.com/library/47d96cf6-9e2f-4fc0-9682-7258d3fbf918%28Office.15%29.aspx)  
- [ServiceError, énumération](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.serviceerror%28v=exchg.80%29.aspx) 
- [Supprimer des éléments à l’aide d’EWS dans Exchange](deleting-items-by-using-ews-in-exchange.md)
    


---
title: Compléments Outlook et EWS dans Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.assetid: 821c8eb9-bb58-42e8-9a3a-61ca635cba59
description: Trouvez des informations sur les compléments Outlook et leur fonctionnement avec EWS dans Exchange.
localization_priority: Priority
ms.openlocfilehash: 2b0cee2017c24d714fa444c094ab1797be1fbe99
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456275"
---
# <a name="outlook-add-ins-and-ews-in-exchange"></a>Compléments Outlook et EWS dans Exchange

Trouvez des informations sur les compléments Outlook et leur fonctionnement avec EWS dans Exchange.

Les compléments Outlook fournissent une interface unique et un modèle de programmation qui utilise des normes Web pour vous permettre de créer une expérience personnalisée pour vos utilisateurs de messagerie. Vous pouvez créer des applications de messagerie qui affichent des informations contextuelles ou utiles dans un cadre HTML5 hébergé dans Outlook ; par exemple, une application de messagerie peut afficher une carte Bing avec une adresse mise en surbrillance lorsqu’un message électronique contient une adresse. Ou lorsqu’un utilisateur compose un message, une application de messagerie peut afficher des informations supplémentaires sur le destinataire et insérer un message d’accueil standard dans le message électronique en appuyant sur un bouton.

> [!NOTE]
> Les références à « Outlook » s’appliquent, dans cet article, au client riche Outlook, à Outlook RT, à Outlook Web App et à OWA pour périphériques

L’interface des applications de messagerie fait partie de l’API JavaScript pour Office. Vous pouvez utiliser l’API pour accéder aux informations dans Exchange afin de permettre à votre application de messagerie de :

- [Reconnaître les entités](https://msdn.microsoft.com/library/a6b0904b-afe9-4882-9136-3d8cfd57fcf8%28Office.15%29.aspx), telles que les adresses, les numéros de téléphone, les suggestions de tâches ou les suggestions de réunion dans un message électronique.

- Ouvrez et affichez les [messages](https://msdn.microsoft.com/library/d0bca550-70c3-457c-85f8-e19b39e3b892%28Office.15%29.aspx) et [rendez-vous](https://msdn.microsoft.com/library/6cfbc29d-8581-474e-9a8b-510471e4bf8b%28Office.15%29.aspx) existants dans un affichage distinct afin que les utilisateurs puissent effectuer des renvois d’informations dans un ou plusieurs messages.

- [Effectuer des demandes EWS](https://msdn.microsoft.com/library/2ec380e0-4a67-4146-92a6-6a39f65dc6f2%28Office.15%29.aspx) auprès du serveur Exchange qui héberge la boîte aux lettres de l’utilisateur. Une application de messagerie peut, par exemple, obtenir une liste de dossiers pour permettre à l’utilisateur de stocker le message, ou afficher tous les éléments d’une conversation, ou marquer un message électronique comme courrier indésirable.

- [Obtenir un jeton](https://msdn.microsoft.com/library/c658518b-6867-41a0-99cf-810303e4c539%28Office.15%29.aspx) pour identifier un compte de messagerie de manière unique afin d’activer l’authentification unique sur un service tiers.

- [Obtenez un jeton](https://msdn.microsoft.com/library/c658518b-6867-41a0-99cf-810303e4c539%28Office.15%29.aspx) qui permet à un service tiers de formuler des demandes EWS au nom de l’utilisateur, par exemple, pour extraire les pièces jointes d’un élément ou pour obtenir un élément à partir du serveur Exchange pour un traitement plus poussé.

Vous pouvez utiliser les applications de messagerie pour personnaliser l’expérience Outlook Web App pour vos utilisateurs ; Toutefois, si vous souhaitez personnaliser l’apparence d’Outlook Web App, consultez les articles suivants sur TechNet :

- [Création d'un thème pour Outlook Web App](https://technet.microsoft.com/library/bb201700%28v=exchg.150%29.aspx)

- [Personnaliser les pages de connexion, de sélection de la langue et d’erreur d’Outlook Web App](https://technet.microsoft.com/library/ee633483%28v=exchg.150%29.aspx)

Votre organisation peut installer des applications de messagerie sur un serveur interne pour limiter l’accès aux utilisateurs autorisés, ou vous et d’autres développeurs d’applications de messagerie peuvent placer des applications de messagerie sur l' [Office Store](https://office.microsoft.com/store/) pour les vendre au grand public. Toute personne qui exécute Outlook peut télécharger, installer et utiliser des applications de messagerie à partir du Marketplace.

Si vous souhaitez en savoir plus sur la création d’applications de messagerie, consultez la documentation sur les [compléments Outlook](/outlook/add-ins) ou l’exemple [créer une requête EWS](https://code.msdn.microsoft.com/exchange/Mail-apps-for-Outlook-Make-770b2528) .

## <a name="ews-and-outlook-add-ins"></a>Compléments EWS et Outlook

Vous pouvez utiliser un sous-ensemble des opérations EWS sur le serveur Exchange qui héberge le compte qui exécute une application de messagerie.

La fonction [Mailbox. makeEwsRequestAsync](https://msdn.microsoft.com/library/2ec380e0-4a67-4146-92a6-6a39f65dc6f2%28Office.15%29.aspx) vous permet d’effectuer des demandes EWS à partir de votre application de messagerie vers le serveur qui héberge la boîte aux lettres de l’utilisateur. Vous créez l’enveloppe SOAP et la requête XML, et la fonction **makeEwsRequestAsync** appelle EWS avec un jeton d’authentification qui identifie la boîte aux lettres et l’application de messagerie qui effectue la demande. Pour sécuriser la boîte aux lettres de l’utilisateur, le serveur Exchange rejette toutes les requêtes qui ne proviennent pas de l’application de messagerie ou d’une boîte aux lettres qui n’est pas hébergée sur le serveur.

Comme toute autre application, une application de messagerie doit disposer d’autorisations pour fonctionner. Votre administrateur doit :

- [Accorder un accès EWS](controlling-client-application-access-to-ews-in-exchange.md) à l’utilisateur des applications de messagerie.

- [Définissez « OAuthAuthentication » sur true](https://technet.microsoft.com/library/aa997233%28v=exchg.150%29.aspx) dans le répertoire EWS du serveur d’accès au client.

Vous devez également vous assurer que votre application demande l’autorisation de lecture/écriture de boîte aux lettres dans le [modèle d’autorisation](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md)applications pour Office.

Une fois ces étapes terminées, un sous-ensemble des opérations EWS de dossier et d’élément est disponible pour l’application de messagerie à utiliser.

**Tableau 1. Opérations de dossier et d’élément EWS que les applications de messagerie peuvent utiliser**

|**Opérations sur les dossiers**|**Opérations d’élément**|
|:-----|:-----|
|[Opération CreateFolder](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> [Opération FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> [Opération GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> [Opération UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |[Opération CopyItem](https://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> [Opération CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> [Opération FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) <br/> [Opération FindConversation](https://msdn.microsoft.com/library/2384908a-c203-45b6-98aa-efd6a4c23aac%28Office.15%29.aspx) <br/> [Opération GetConversationItems](https://msdn.microsoft.com/library/8ae00a99-b37b-4194-829c-fe300db6ab99%28Office.15%29.aspx) <br/> [Opération GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> [Opération MarkAsJunk](https://msdn.microsoft.com/library/1f71f04d-56a9-4fee-a4e7-d1034438329e%28Office.15%29.aspx) <br/> [Opération MoveItem](https://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> [Opération SendItem](https://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) <br/> [Opération UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |

### <a name="service-callback-tokens"></a>Jetons de rappel de service

Les jetons de rappel de service permettent aux applications de messagerie de transmettre un jeton d’accès à un service tiers afin que ce service puisse effectuer des demandes EWS sur le serveur Exchange qui héberge la boîte aux lettres. Par exemple, une application de messagerie peut transmettre un jeton de rappel de service à un service tiers, ainsi qu’une liste d’ID de pièces jointes pour les images jointes à un message électronique. Le service peut ensuite utiliser les ID de pièce jointe et le jeton de rappel pour effectuer une demande EWS auprès du serveur Exchange de l’utilisateur pour obtenir les images jointes. Les applications de messagerie peuvent également utiliser le jeton de rappel de service avec une liste d’ID d’élément pour obtenir des éléments de messagerie et de rendez-vous à partir du serveur Exchange.

Le jeton de rappel de service est un jeton opaque que le service tiers attache à la demande EWS dans un en-tête d’authentification de porteur. Le jeton identifie l’application de messagerie et la boîte aux lettres pour sécuriser la demande EWS. Pour savoir comment utiliser les jetons de rappel de service, consultez la rubrique relative aux [compléments Outlook : obtenir des pièces jointes à partir d’un exemple de serveur Exchange](https://code.msdn.microsoft.com/exchange/Mail-apps-for-Office-Get-38babdc9) .

## <a name="see-also"></a>Voir aussi


- [Contrôle de l'accès aux applications de client pour EWS dans Exchange](controlling-client-application-access-to-ews-in-exchange.md)

- [Méthode Mailbox.makeEwsRequestAsync (interface API JavaScript pour Office)](https://msdn.microsoft.com/library/2ec380e0-4a67-4146-92a6-6a39f65dc6f2%28Office.15%29.aspx)

- [Compléments Outlook](https://docs.microsoft.com/outlook/add-ins)

- [Méthode Mailbox.getUserIdentityTokenAsync (interface API JavaScript pour Office)](https://msdn.microsoft.com/library/c658518b-6867-41a0-99cf-810303e4c539%28Office.15%29.aspx)

- [Authentifier un complément Outlook à l’aide de jetons d’identité Exchange](https://msdn.microsoft.com/library/c0520a1e-d9ba-495a-a99f-6816d7d2a23e%28Office.15%29.aspx)

- [Présentation des autorisations de complément Outlook](https://docs.microsoft.com/outlook/add-ins/understanding-outlook-add-in-permissions)

- [Set-WebServicesVirtualDirectory](https://technet.microsoft.com/library/aa997233%28v=exchg.150%29.aspx)

- [Compléments Outlook : créer une demande EWS](https://code.msdn.microsoft.com/office/Mail-apps-for-Outlook-Make-770b2528)

- [Compléments Outlook : utiliser un jeton d’identité client](https://code.msdn.microsoft.com/Mail-apps-for-Outlook-Use-b20a66b6)

- [Compléments Outlook : obtenir des pièces jointes à partir d’un serveur Exchange](https://code.msdn.microsoft.com/office/Mail-apps-for-Office-Get-38babdc9)

---
title: Compléments Outlook et EWS dans Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 821c8eb9-bb58-42e8-9a3a-61ca635cba59
description: Trouvez des informations sur les compléments Outlook et leur fonctionnement avec EWS dans Exchange.
ms.openlocfilehash: 7eae834fe0bb93e2e94f094e811ab6cf002fc71b
ms.sourcegitcommit: 42eecc78e7aed7e95f73370d6c39ab8f4e96bf68
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/12/2018
ms.locfileid: "25541637"
---
# <a name="outlook-add-ins-and-ews-in-exchange"></a>Compléments Outlook et EWS dans Exchange

Trouvez des informations sur les compléments Outlook et leur fonctionnement avec EWS dans Exchange.

Compléments Outlook fournissent une interface unique et le modèle de programmation qui utilise des normes web pour vous permettent de créer une expérience personnalisée pour vos utilisateurs de messagerie. Vous pouvez créer des applications de messagerie qui fournissent des informations contextuelles ou utiles dans un cadre d’HTML5 hébergé dans Outlook. par exemple, une application de messagerie peut afficher une carte Bing à une adresse mis en surbrillance lorsqu’un message électronique contienne une adresse. Ou lorsqu’un utilisateur compose un message, une application de messagerie peut afficher des informations supplémentaires sur le destinataire, puis insérer un message d’accueil standard dans le courrier électronique à l’aide d’un bouton.

> [!NOTE]
> Les références à « Outlook » s’appliquent, dans cet article, au client riche Outlook, à Outlook RT, à Outlook Web App et à OWA pour périphériques

L’interface d’applications de messagerie fait partie de l’API JavaScript pour Office. Vous pouvez utiliser l’API pour accéder aux informations dans Exchange pour activer votre application de messagerie :

- [Reconnaître les entités](http://msdn.microsoft.com/library/a6b0904b-afe9-4882-9136-3d8cfd57fcf8%28Office.15%29.aspx), telles que les adresses, numéros de téléphone, suggestions de tâche ou des suggestions de réunion dans un message électronique.

- Ouvrir et afficher les [messages](http://msdn.microsoft.com/library/d0bca550-70c3-457c-85f8-e19b39e3b892%28Office.15%29.aspx) existants et des [rendez-vous](http://msdn.microsoft.com/library/6cfbc29d-8581-474e-9a8b-510471e4bf8b%28Office.15%29.aspx) dans un affichage distinct, afin que les utilisateurs peuvent une référence croisée dans un ou plusieurs messages.

- [Demandes EWS effectuer](http://msdn.microsoft.com/library/2ec380e0-4a67-4146-92a6-6a39f65dc6f2%28Office.15%29.aspx) sur le serveur Exchange qui héberge la boîte aux lettres de l’utilisateur. Une application de messagerie peut, par exemple, obtenez une liste de dossiers afin que l’utilisateur peut choisir une pour stocker le message, ou afficher tous les éléments dans une conversation, ou de marquer un message électronique comme courrier indésirable.

- [Obtenir un jeton](http://msdn.microsoft.com/library/c658518b-6867-41a0-99cf-810303e4c539%28Office.15%29.aspx) à identifier de manière unique un compte de messagerie à activer unique de se connecter à un service tiers.

- [Obtenir un jeton](http://msdn.microsoft.com/library/c658518b-6867-41a0-99cf-810303e4c539%28Office.15%29.aspx) qui permet à un service tiers pour les demandes EWS au nom de l’utilisateur, par exemple, pour extraire les pièces jointes d’un élément ou pour obtenir un élément à partir du serveur Exchange pour un traitement supplémentaire.

Vous pouvez utiliser les applications de messagerie pour personnaliser l’expérience Outlook Web App pour vos utilisateurs ; Si, toutefois, vous souhaitez personnaliser la « aspect » d’Outlook Web App, voir les articles suivants sur TechNet :

- [Créer un thème pour Outlook Web App](http://technet.microsoft.com/en-us/library/bb201700%28v=exchg.150%29.aspx)

- [Personnaliser la Outlook Web App connexion, sélection de la langue et les pages d’erreurs](http://technet.microsoft.com/en-us/library/ee633483%28v=exchg.150%29.aspx)

Votre organisation permettre installer des applications de messagerie sur un serveur interne pour limiter l’accès aux utilisateurs autorisés, ou vous et autres développeurs d’application de messagerie peuvent mettre des applications de messagerie sur l' [Office Store](http://office.microsoft.com/store/) pour la vente au grand public. Toute personne exécute Outlook peut télécharger, installer et utiliser les applications de messagerie Marketplace.

Si vous souhaitez en savoir plus sur la création d’applications de messagerie, consultez la [documentation de compléments Outlook](/outlook/add-ins) ou l’exemple [effectuer une demande EWS](http://code.msdn.microsoft.com/exchange/Mail-apps-for-Outlook-Make-770b2528) .

## <a name="ews-and-outlook-add-ins"></a>Compléments EWS et Outlook

Vous pouvez utiliser un sous-ensemble des opérations EWS sur le serveur Exchange qui héberge le compte qui exécute une application de messagerie.

La fonction [mailbox.makeEwsRequestAsync](http://msdn.microsoft.com/library/2ec380e0-4a67-4146-92a6-6a39f65dc6f2%28Office.15%29.aspx) vous permet d’effectuer des demandes EWS à partir de votre application de messagerie sur le serveur qui héberge la boîte aux lettres de l’utilisateur. Créer l’enveloppe SOAP et demande XML et les appels de fonction **makeEwsRequestAsync** EWS avec un jeton d’authentification qui identifie la boîte aux lettres et de l’application qui effectue la demande de messagerie. Pour sécuriser des boîtes aux lettres de l’utilisateur, le serveur Exchange rejette toutes les demandes qui ne proviennent pas à partir de l’application de messagerie ou d’une boîte aux lettres qui n’est pas hébergé sur le serveur.

Comme toute autre application, une application de messagerie a besoin des autorisations pour travailler. Votre administrateur doit :

- [EWS accorder l’accès](controlling-client-application-access-to-ews-in-exchange.md) à l’utilisateur d’applications de messagerie.

- [Définir « OAuthAuthentication » sur true](http://technet.microsoft.com/en-us/library/aa997233%28v=exchg.150%29.aspx) dans le répertoire EWS du serveur Client Access.

Vous devez également vous assurer que votre application demande l’autorisation de boîte aux lettres en lecture/écriture dans les applications pour Office- [modèle d’autorisation](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md).

Une fois ces étapes terminées, un sous-ensemble de dossier et opérations EWS d’élément sont disponibles pour l’application de messagerie à utiliser.

**Le tableau 1. Opérations EWS dossiers et éléments que les applications de messagerie peuvent utiliser**

|**Opérations de dossier**|**Opérations d’élément**|
|:-----|:-----|
|[Opération CreateFolder](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> [Opération FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> [Opération GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> [Opération UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |[Opération CopyItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> [Opération CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> [Opération FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) <br/> [Opération FindConversation](http://msdn.microsoft.com/library/2384908a-c203-45b6-98aa-efd6a4c23aac%28Office.15%29.aspx) <br/> [Opération GetConversationItems](http://msdn.microsoft.com/library/8ae00a99-b37b-4194-829c-fe300db6ab99%28Office.15%29.aspx) <br/> [Opération GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> [Opération MarkAsJunk](http://msdn.microsoft.com/library/1f71f04d-56a9-4fee-a4e7-d1034438329e%28Office.15%29.aspx) <br/> [Opération MoveItem](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> [Opération SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) <br/> [Opération UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |

### <a name="service-callback-tokens"></a>Jetons de rappel de service

Jetons de rappel service activer les applications de messagerie transmettre un jeton d’accès à un service tiers afin que le service peut effectuer des demandes EWS sur le serveur Exchange qui héberge la boîte aux lettres. Par exemple, une application de messagerie peut passer un jeton de rappel de service à un service tiers avec une liste d’ID de pièce jointe pour les images attaché à un message électronique. Le service peut utiliser ensuite l’ID de pièce jointe et le jeton de rappel pour effectuer une demande EWS à Exchange server l’utilisateur pour obtenir les images jointes. Les applications de messagerie peuvent également utiliser le jeton de rappel de service avec une liste d’ID d’élément de pour obtenir des éléments de courrier électronique et rendez-vous à partir du serveur Exchange.

Le jeton de rappel de service est un jeton opaque qui le service tiers joint à la demande EWS dans un en-tête d’authentification illimitées. Le jeton identifie l’application de messagerie et de la boîte aux lettres pour aider à sécuriser la demande EWS. Pour savoir comment utiliser les jetons de rappel de service, voir la [des compléments Outlook : obtenir des pièces jointes à partir d’un serveur Exchange](http://code.msdn.microsoft.com/exchange/Mail-apps-for-Office-Get-38babdc9) exemple.

## <a name="see-also"></a>Voir aussi


- [Contrôler l’accès des applications clientes à EWS dans Exchange](controlling-client-application-access-to-ews-in-exchange.md)

- [Méthode Mailbox.makeEwsRequestAsync (interface API JavaScript pour Office)](http://msdn.microsoft.com/library/2ec380e0-4a67-4146-92a6-6a39f65dc6f2%28Office.15%29.aspx)

- [Compléments Outlook](https://docs.microsoft.com/outlook/add-ins)

- [Méthode Mailbox.getUserIdentityTokenAsync (interface API JavaScript pour Office)](http://msdn.microsoft.com/library/c658518b-6867-41a0-99cf-810303e4c539%28Office.15%29.aspx)

- [Authentifier un complément Outlook à l’aide de jetons d’identité Exchange](http://msdn.microsoft.com/library/c0520a1e-d9ba-495a-a99f-6816d7d2a23e%28Office.15%29.aspx)

- [Spécifier les autorisations pour l'accès du complément Outlook à la boîte aux lettres de l'utilisateur](https://docs.microsoft.com/en-us/outlook/add-ins/understanding-outlook-add-in-permissions)

- [Set-WebServicesVirtualDirectory](http://technet.microsoft.com/en-us/library/aa997233%28v=exchg.150%29.aspx)

- [Compléments Outlook : créer une demande EWS](http://code.msdn.microsoft.com/office/Mail-apps-for-Outlook-Make-770b2528)

- [Compléments Outlook : utiliser un jeton d’identité client](http://code.msdn.microsoft.com/Mail-apps-for-Outlook-Use-b20a66b6)

- [Compléments Outlook : obtenir des pièces jointes à partir d’un serveur Exchange](http://code.msdn.microsoft.com/office/Mail-apps-for-Office-Get-38babdc9)

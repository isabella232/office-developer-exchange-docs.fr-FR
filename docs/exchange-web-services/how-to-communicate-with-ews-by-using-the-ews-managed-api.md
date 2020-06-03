---
title: Communiquer avec EWS à l'aide de l'API managée EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: d1b78293-da02-413a-875c-681e99146af3
description: Trouvez des informations sur l’utilisation de l’API managée EWS pour communiquer avec EWS dans Exchange.
localization_priority: Priority
ms.openlocfilehash: be807f2d936bf79d181476ec8eb12f20fca7950f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528243"
---
# <a name="communicate-with-ews-by-using-the-ews-managed-api"></a>Communiquer avec EWS à l'aide de l'API managée EWS

Trouvez des informations sur l’utilisation de l’API managée EWS pour communiquer avec EWS dans Exchange.
  
La classe [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) de l’API managée EWS contient les méthodes et les propriétés qui permettent de définir les informations d’identification de l’utilisateur, d’identifier le point de terminaison EWS, d’envoyer et de recevoir des messages SOAP et de configurer la liaison pour communiquer avec EWS. Avant de pouvoir utiliser l’API managée EWS pour effectuer une tâche, vous devez créer une instance de la classe **ExchangeService** et la lier à EWS. 
  
Une fois que vous avez configuré un objet [ExchangeService](https://msdn.microsoft.com/library/Microsoft.Exchange.WebServices.Data.ExchangeService.aspx) avec les informations d’identification de l’utilisateur et le point de terminaison EWS, tout objet Mailbox qui fait référence à l’objet [ExchangeService](https://msdn.microsoft.com/library/Microsoft.Exchange.WebServices.Data.ExchangeService.aspx) peut utiliser les types de méthodes suivants pour communiquer avec EWS : 
  
- Méthodes de l’objet ExchangeService : toutes les méthodes sur l’objet **ExchangeService** qui ne sont pas héritées du type d' **objet** de base effectuent des appels vers EWS. 
    
- Éléments de boîte aux lettres Exchange et type de dossier.
    
**Tableau 1. Méthodes de boîte aux lettres et de type de dossier qui communiquent avec EWS**

|Méthode|Fonction|Opérations qu’il appelle|
|:-----|:-----|:-----|
|[Load](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.load%28v=exchg.80%29.aspx) <br/> |Obtient les propriétés d’un élément, d’une pièce jointe ou d’un objet de configuration utilisateur.  <br/> |[Opération GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/><br/> [Opération GetAttachment](https://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx) <br/><br/> [Opération GetUserConfiguration](https://msdn.microsoft.com/library/71d50e3c-92bd-435f-8118-b28bb85f8138%28Office.15%29.aspx) <br/> |
|[Rattach](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) <br/> |Remplit un nouvel élément sur le client avec les informations d’un élément existant sur le serveur.  <br/> |[Opération GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> |
|[Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.save%28v=exchg.80%29.aspx) <br/> |Enregistre la copie de l’élément client sur le serveur.  <br/> |[Opération UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/><br/> [Opération UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/><br/>[Opération CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/><br/>[Opération CreateFolder](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> |
|[Mettre à jour](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.update%28v=exchg.80%29.aspx) <br/> |Met à jour le serveur avec les modifications apportées sur le client.<br/><br/>Pour les éléments et les dossiers, la méthode **Update** utilise l' [opération UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) et l' [opération UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx).  <br/> |[Opération UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/><br/>[Opération UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |
|[Supprimer](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx) <br/> |Supprime un élément sur le serveur.<br/><br/>Pour les éléments et les dossiers, la méthode **Delete** utilise le et l' [opération DeleteFolder](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx).  <br/> |[Opération DeleteItem](https://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/><br/> [Opération DeleteFolder](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |
|[Copy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.copy%28v=exchg.80%29.aspx) <br/> |Crée une copie de l’élément ou des dossiers sur le serveur.  <br/> |[Opération CopyItem](https://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/><br/> [CopyFolder, opération](https://msdn.microsoft.com/library/c7ea0d68-9793-4144-b378-d99536776db9%28Office.15%29.aspx) <br/> |
|[Move](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.move%28v=exchg.80%29.aspx) <br/> |Déplace des éléments ou des dossiers sur le serveur.  <br/> |[Opération MoveItem](https://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/><br/> [Opération MoveFolder](https://msdn.microsoft.com/library/c7233966-6c87-4a14-8156-b1610760176d%28Office.15%29.aspx) <br/> |
   
## <a name="to-use-the-ews-managed-api-to-communicate-with-ews"></a>Pour utiliser l’API managée EWS pour communiquer avec EWS

1. Instanciez la classe **ExchangeService** . 
    
   ```csharp
    ExchangeService service = new ExchangeService();
   ```

   > [!NOTE]
   > L’instanciation de **ExchangeService** avec un constructeur vide crée une instance liée à la dernière version connue d’Exchange. Vous pouvez également cibler une version spécifique d’Exchange en spécifiant version comme paramètre. `ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2007_SP1);`
  
2. Définissez les informations d’identification de l’utilisateur qui envoie des demandes au serveur Exchange. Si vous souhaitez vous connecter à EWS à partir d’un ordinateur connecté au domaine, à l’aide des informations d’identification de l’utilisateur authentifié, définissez la propriété **UseDefaultCredentials** de l’objet **ExchangeService** sur **true**.
    
   ```cs
    // Connect by using the default credentials of the authenticated user.
    service.UseDefaultCredentials = true;
   ```

   Si vous ne souhaitez pas vous connecter à l’aide des informations d’identification par défaut de l’utilisateur, définissez la propriété **Credentials** sur l’objet **ExchangeService** afin de spécifier explicitement les informations d’identification d’un autre utilisateur. Si vous utilisez Exchange Online ou Exchange Online dans le cadre d’Office 365, vous utiliserez l’authentification de base, avec un nom d’utilisateur et un mot de passe. Un nom de domaine est requis pour l’authentification NTLM. 
    
   ```cs
    // Connect by using the credentials of user1 at contoso.com.
    service.Credentials = new WebCredentials("user1@contoso.com", "password");
   ```

   Vous pouvez également spécifier les informations d’identification de l’utilisateur à l’aide du nom de domaine et du mot de passe de l’utilisateur.
    
   ```cs
    // Connect by using the credentials of contoso/user1.
    service.Credentials = new WebCredentials("user1", "password", "contoso");
   ```

   > [!NOTE]
   > Si la propriété **UseDefaultCredentials** est définie sur **true**, la valeur de la propriété **Credentials** est ignorée. 
  
3. Définissez l’URL du point de terminaison EWS. Cette URL localise le fichier Exchange. asmx sur le serveur d’accès au client.
    
   ```cs
    // Use Autodiscover to set the URL endpoint.
    service.AutodiscoverUrl("user1@contoso.com");
   ```

   > [!NOTE]
   >  Bien que vous puissiez définir explicitement la propriété **URL** de **ExchangeService** sur une valeur codée en dur, nous vous recommandons d’utiliser à la place le service de découverte automatique, pour les raisons suivantes : > la découverte automatique détermine le meilleur point de terminaison pour un utilisateur donné (le point de terminaison le plus proche du serveur de boîtes aux lettres de l’utilisateur). > l’URL EWS peut changer si de nouveaux serveurs d’accès au client sont déployés. Dans ce scénario, l’utilisation de la [découverte automatique](autodiscover-for-exchange.md) signifie qu’aucune modification de code n’est nécessaire. > vous devez définir l’URL explicitement ou appeler **AutodiscoverUrl**, mais vous ne devez pas effectuer les deux. 
  
## <a name="see-also"></a>Voir aussi

- [Prise en main des applications clientes d'API managée EWS](get-started-with-ews-managed-api-client-applications.md) 
- [Utilisation de la découverte automatique pour trouver des points de connexion](how-to-use-autodiscover-to-find-connection-points.md)   
- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)
    


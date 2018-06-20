---
title: Communiquer avec EWS à l’aide de l’API managée EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: d1b78293-da02-413a-875c-681e99146af3
description: Trouvez des informations sur l’utilisation de l’API managée EWS pour communiquer avec EWS dans Exchange.
ms.openlocfilehash: 773fcc3f7e95d25effb5a686d4b79ec22610df8c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754821"
---
# <a name="communicate-with-ews-by-using-the-ews-managed-api"></a>Communiquer avec EWS à l’aide de l’API managée EWS

Trouvez des informations sur l’utilisation de l’API managée EWS pour communiquer avec EWS dans Exchange.
  
La classe [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) dans l’API managée EWS contient les méthodes et propriétés que vous utilisez pour définir les informations d’identification utilisateur, identifier le point de terminaison EWS, envoyer et recevoir des messages SOAP et configurer la liaison de communiquer avec EWS. Avant de pouvoir utiliser l’API managée EWS pour accomplir une tâche, vous devez créer une instance de la classe **ExchangeService** et le lier à EWS. 
  
Après avoir configuré un objet [ExchangeService](https://msdn.microsoft.com/library/Microsoft.Exchange.WebServices.Data.ExchangeService.aspx) avec les informations d’identification utilisateur et le point de terminaison EWS, n’importe quel objet boîte aux lettres qui fait référence à l’objet [ExchangeService](https://msdn.microsoft.com/library/Microsoft.Exchange.WebServices.Data.ExchangeService.aspx) peut utiliser les types suivants de la méthode pour communiquer avec EWS : 
  
- Méthodes de l’objet ExchangeService — toutes les méthodes de l’objet **ExchangeService** qui ne sont pas héritées le type **d’objet** base appeler EWS. 
    
- Élément de boîte aux lettres Exchange et dossier type de méthodes.
    
**Le tableau 1. Élément de boîte aux lettres et de dossiers tapez méthodes qui communiquent avec EWS**

|Méthode|Fonction|Opérations qu’elle appelle|
|:-----|:-----|:-----|
|[Load](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.load%28v=exchg.80%29.aspx) <br/> |Obtient les propriétés sur un objet de configuration utilisateur, pièces jointes ou élément.  <br/> |[GetItem Operation](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/><br/> [Opération GetAttachment](http://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx) <br/><br/> [Opération GetUserConfiguration](http://msdn.microsoft.com/library/71d50e3c-92bd-435f-8118-b28bb85f8138%28Office.15%29.aspx) <br/> |
|[Créer une liaison](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) <br/> |Remplit un nouvel élément sur le client avec des informations à partir d’un élément existant sur le serveur.  <br/> |[GetItem Operation](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> |
|[Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.save%28v=exchg.80%29.aspx) <br/> |Enregistre la copie de l’élément client sur le serveur.  <br/> |[UpdateItem Operation](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/><br/> [Opération UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/><br/>[CreateItem Operation](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/><br/>[Opération CreateFolder](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> |
|[Mettre à jour](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.update%28v=exchg.80%29.aspx) <br/> |Met à jour le serveur avec les modifications effectuées sur le client.<br/><br/>Pour les éléments et les dossiers, la méthode de **mise à jour** utilise l' [opération UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) et l' [opération UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx).  <br/> |[UpdateItem Operation](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/><br/>[Opération UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |
|[Supprimer](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx) <br/> |Supprime un élément sur le serveur.<br/><br/>Pour les éléments et les dossiers, la méthode **Delete** utilise l' [opération DeleteFolder](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx).  <br/> |[Opération DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/><br/> [Opération DeleteFolder](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |
|[Copier](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.copy%28v=exchg.80%29.aspx) <br/> |Crée une copie de l’élément ou les dossiers sur le serveur.  <br/> |[Opération CopyItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/><br/> [Opération CopyFolder](http://msdn.microsoft.com/library/c7ea0d68-9793-4144-b378-d99536776db9%28Office.15%29.aspx) <br/> |
|[Déplacer](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.move%28v=exchg.80%29.aspx) <br/> |Déplace les éléments ou des dossiers sur le serveur.  <br/> |[Opération MoveItem](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/><br/> [Opération MoveFolder](http://msdn.microsoft.com/library/c7233966-6c87-4a14-8156-b1610760176d%28Office.15%29.aspx) <br/> |
   
## <a name="to-use-the-ews-managed-api-to-communicate-with-ews"></a>Pour utiliser l’API managée EWS pour communiquer avec EWS

1. Instanciez la classe **ExchangeService** . 
    
   ```csharp
    ExchangeService service = new ExchangeService();
   ```

   > [!NOTE]
   > L’instanciation de **ExchangeService** avec un constructeur vide créera une instance qui est liée à la dernière version connue d’Exchange. Vous pouvez également cibler une version spécifique d’Exchange en spécifiant la version en tant que paramètre. `ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2007_SP1);`
  
2. Définir les informations d’identification de l’utilisateur qui envoie des requêtes sur le serveur Exchange. Si vous souhaitez vous connecter à EWS depuis un ordinateur qui est connecté au domaine, les informations d’identification de l’utilisateur authentifié, définissez la propriété **UseDefaultCredentials** sur l’objet **ExchangeService** sur **true**.
    
   ```cs
    // Connect by using the default credentials of the authenticated user.
    service.UseDefaultCredentials = true;
   ```

   Si vous ne souhaitez pas vous connecter en utilisant les informations d’identification des utilisateurs par défaut, définissez la propriété **d’informations d’identification** sur l’objet **ExchangeService** spécifier de manière explicite les informations d’identification d’un autre utilisateur. Si vous utilisez Exchange Online ou Exchange Online dans le cadre d’Office 365, vous allez utiliser l’authentification de base, avec uniquement un nom d’utilisateur et un mot de passe. Un nom de domaine est requis pour l’authentification NTLM. 
    
   ```cs
    // Connect by using the credentials of user1 at contoso.com.
    service.Credentials = new WebCredentials("user1@contoso.com", "password");
   ```

   Vous pouvez également spécifier les informations d’identification de l’utilisateur à l’aide de nom de domaine de l’utilisateur et le mot de passe.
    
   ```cs
    // Connect by using the credentials of contoso/user1.
    service.Credentials = new WebCredentials("user1", "password", "contoso");
   ```

   > [!NOTE]
   > Si la propriété **UseDefaultCredentials** est définie sur **true**, la valeur de la propriété **Credentials** est ignorée. 
  
3. Définir l’URL du point de terminaison EWS. Cette URL localise le fichier exchange.asmx sur le serveur d’accès au Client.
    
   ```cs
    // Use Autodiscover to set the URL endpoint.
    service.AutodiscoverUrl("user1@contoso.com");
   ```

   > [!NOTE]
   >  Vous pouvez définir explicitement la propriété **Url** de **ExchangeService** sur une valeur codée en dur, nous vous recommandons d’utiliser le service de découverte automatique au lieu de cela, pour les raisons suivantes : > découverte automatique détermine le point de terminaison meilleures pour un utilisateur donné (le point de terminaison le plus proche de serveur de boîtes aux lettres de l’utilisateur). > L’URL EWS peut changer si les nouveaux serveurs d’accès au Client sont déployés. Dans ce scénario, l’utilisation [d’Autodiscover](autodiscover-for-exchange.md) signifie qu'aucune modification de code n’est nécessaires. > Vous devez définir l’URL de manière explicite ou appel **AutodiscoverUrl**, mais vous ne devez pas effectuer les deux. 
  
## <a name="see-also"></a>Voir aussi

- [Prise en main des applications clientes d'API managée EWS](get-started-with-ews-managed-api-client-applications.md) 
- [Utiliser la découverte automatique pour rechercher les points de connexion](how-to-use-autodiscover-to-find-connection-points.md)   
- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)
    


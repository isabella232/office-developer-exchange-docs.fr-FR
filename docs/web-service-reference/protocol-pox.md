---
title: Protocole (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: f77e4d66-6fdd-4999-9339-f7d7f9c86f44
description: L’élément de protocole contient les spécifications pour connecter un client à l’ordinateur qui exécute le serveur Exchange qui a le rôle de serveur d’accès au Client est installé.
ms.openlocfilehash: e58ae82ea5ec9d39db0f9219f6019df7da24a343
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828926"
---
# <a name="protocol-pox"></a>Protocole (POX)

L’élément de **protocole** contient les spécifications pour connecter un client à l’ordinateur qui exécute le serveur Exchange qui a le rôle de serveur d’accès au Client est installé. 
  
[Découverte automatique (POX)](autodiscover-pox.md)
  
[Réponse (POX)](response-pox.md)
  
[Compte (POX)](account-pox.md)
  
[Protocole (POX)](protocol-pox.md)
  
```xml
<Protocol>
   <Type/>
   <Internal/>
   <External/>
   <TTL/>
   <Server/>
   <ServerDN/>
   <ServerVersion/>
   <MdbDN/>
   <PublicFolderServer/>
   <Port/>
   <DirectoryPort/>
   <ReferralPort/>
   <ASUrl/>
   <EwsUrl/>
   <EmwsUrl/>
   <SharingUrl/>
   <EcpUrl/>
   <EcpUrl-um/>
   <EcpUrl-aggr/>
   <EcpUrl-mt/>
   <EcpUrl-ret/>
   <EcpUrl-sms/>
   <EcpUrl-publish/>
   <EcpUrl-photo/>
   <EcpUrl-tm/>
   <EcpUrl-tmCreating/>
   <EcpUrl-tmHiding/>
   <EcpUrl-tmEditing/>
   <EcpUrl-extinstall/>
   <OOFUrl/>
   <OABUrl/>
   <UMUrl/>
   <EwsPartnerUrl/>
   <LoginName/>
   <DomainRequired/>
   <DomainName/>
   <SPA/>
   <AuthPackage/>
   <CertPrincipalName/>
   <SSL/>
   <AuthRequired/>
   <UsePOPAuth/>
   <SMTPLast/>
   <NetworkRequirements/>
   <AddressBook/>
   <MailStore/>
</Protocol>
```

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|Type  <br/> |Indique le type de protocole décrit par cet élément de **protocole** . La seule valeur valide pour cet attribut est « mapiHttp ». Cet attribut est présent uniquement si la demande de la découverte automatique qui correspond à cette réponse [inclus un en-tête X-MapiHttpCapability](pox-autodiscover-request-for-exchange.md). Cet attribut s’applique aux clients qui implémentent le protocole MAPI/HTTP et cible Exchange Online, Exchange Online dans le cadre d’Office 365, ou créer des versions locales d’Exchange commençant par 15.00.0847.032 (Exchange Server 2013 SP1).  <br/> |
|Version  <br/> |Indique la version du protocole décrit par cet élément de **protocole** . La seule valeur valide pour cet attribut est « 1 ». Cet attribut est présent uniquement si la demande de découverte automatique qui correspond à cette réponse inclut un en-tête **X-MapiHttpCapability** . Cet attribut s’applique aux clients qui implémentent le protocole MAPI/HTTP et cible Exchange Online, Exchange Online dans le cadre d’Office 365, ou créer des versions locales d’Exchange commençant par 15.00.0847.032 (Exchange Server 2013 SP1).  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Type (POX)](type-pox.md) <br/> |Identifie le type du compte de messagerie configuré.  <br/> |
|[Interne (POX)](internal-pox.md) <br/> |Contient une collection d’URL qu’un client peut utiliser pour se connecter à Exchange à partir de l’intérieur du réseau de l’organisation.  <br/> |
|[Externe (POX)](external-pox.md) <br/> |Contient une collection d’URL qu’un client peut utiliser pour se connecter à Exchange à partir d’en dehors du réseau de l’organisation.  <br/> |
|[TTL (POX)](ttl-pox.md) <br/> |Spécifie la durée de vie, en heures, pendant laquelle les paramètres restent valides.  <br/> |
|[Serveur (POX)](server-pox.md) <br/> |Spécifie le nom du serveur de messagerie.  <br/> |
|[ServerDN (POX)](serverdn-pox.md) <br/> |Spécifie le nom unique du serveur Exchange.  <br/> |
|[ServerVersion (POX)](serverversion-pox.md) <br/> |Représente le numéro de version d’Exchange Server.  <br/> |
|[MdbDN (POX)](mdbdn-pox.md) <br/> |Représente le nom unique de la base de données de boîtes aux lettres.  <br/> |
|[PublicFolderServer (POX)](publicfolderserver-pox.md) <br/> |Contient le nom de domaine complet (FQDN) du serveur de dossiers publics de l’utilisateur.  <br/> |
|[Port (POX)](port-pox.md) <br/> |Spécifie le port utilisé pour se connecter à la banque.  <br/> |
|[DirectoryPort (POX)](directoryport-pox.md) <br/> |Spécifie le port utilisé pour se connecter au répertoire lorsque le protocole fournisseur Interface NSPI (Name Service) est utilisé.  <br/> |
|[ReferralPort (POX)](referralport-pox.md) <br/> |Spécifie le port qui est utilisé pour obtenir une référence à un répertoire.  <br/> |
|[ASUrl (POX)](asurl-pox.md) <br/> |Spécifie l’URL de l’instance des Services Web Exchange pour un utilisateur à extension messagerie meilleures.  <br/> |
|[EwsUrl (POX)](ewsurl-pox.md) <br/> |Spécifie l’URL de l’instance de point de terminaison meilleures pour Exchange Web Services (EWS) pour un utilisateur à extension messagerie.  <br/> |
|[EmwsUrl (POX)](emwsurl-pox.md) <br/> |Spécifie l’URL de l’instance de point de terminaison meilleures pour Exchange Web Services (EWS) pour un utilisateur à extension messagerie.  <br/> |
|[SharingUrl (POX)](sharingurl-pox.md) <br/> |Contient l’URL du serveur de partage utilisé pour le partage des calendriers et des contacts d’échelle de l’organisation.  <br/> |
|[EcpUrl (POX)](ecpurl-pox.md) <br/> |Spécifie l’URL du Panneau de commande Exchange pour un utilisateur à extension messagerie.  <br/> |
|[EcpUrl-MU POX)](ecpurl-um-pox.md) <br/> |Spécifie une URL partielle peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour accéder aux paramètres de messagerie vocale d’un utilisateur à extension messagerie.  <br/> |
|[EcpUrl-aggr (POX)](ecpurl-aggr-pox.md) <br/> |Spécifie une URL partielle peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour accéder aux paramètres d’agrégation de messagerie pour un utilisateur à extension messagerie.  <br/> |
|[EcpUrl-mt (POX)](ecpurl-mt-pox.md) <br/> |Spécifie une URL partielle peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour accéder aux paramètres d’un utilisateur à extension messagerie de suivi des messages électroniques.  <br/> |
|[EcpUrl-ret (POX)](ecpurl-ret-pox.md) <br/> |Spécifie une URL partielle peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour accéder aux paramètres de balises de rétention pour un utilisateur à extension messagerie.  <br/> |
|[EcpUrl-sms (POX)](ecpurl-sms-pox.md) <br/> |Spécifie une URL partielle peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour accéder aux paramètres du Service SMS (Short Message) pour un utilisateur à extension messagerie.  <br/> |
|[Publication EcpUrl (POX)](ecpurl-publish-pox.md) <br/> |Spécifie une URL partielle peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour accéder aux paramètres de publication de calendrier pour un utilisateur à extension messagerie.  <br/> |
|[EcpUrl-photo (POX)](ecpurl-photo-pox.md) <br/> |Spécifie une URL partielle peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour afficher ou modifier la photo actuelle d’un utilisateur à extension messagerie.  <br/> |
|[EcpUrl-tm (POX)](ecpurl-tm-pox.md) <br/> |Spécifie une URL partielle peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut servir à accéder à une liste de toutes les boîtes aux lettres de site dont un utilisateur à extension messagerie est un membre.  <br/> |
|[EcpUrl-tmCreating (POX)](ecpurl-tmcreating-pox.md) <br/> |Spécifie une URL partielle peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour créer une nouvelle boîte aux lettres du site.  <br/> |
|[EcpUrl-tmHiding (POX)](ecpurl-tmhiding-pox.md) <br/> |Spécifie une URL partielle peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour annuler l’abonnement de l’utilisateur à partir d’une boîte aux lettres du site.  <br/> |
|[EcpUrl-tmEditing (POX)](ecpurl-tmediting-pox.md) <br/> |Spécifie une URL partielle peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour modifier une boîte aux lettres de site existante.  <br/> |
|[EcpUrl-extinstall (POX)](ecpurl-extinstall-pox.md) <br/> |Spécifie une URL partielle peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour afficher ou modifier les applications de messagerie actuellement installées dans la boîte aux lettres de l’utilisateur.  <br/> |
|[OOFUrl (POX)](oofurl-pox.md) <br/> |Spécifie l’URL de l’instance du service de disponibilité pour un utilisateur à extension messagerie meilleures.  <br/> |
|[OABUrl (POX)](oaburl-pox.md) <br/> |Spécifie l’URL du serveur de configuration du carnet d’adresses en mode hors connexion pour une topologie Exchange.  <br/> |
|[UMUrl (POX)](umurl-pox.md) <br/> |Spécifie l’URL de l’instance du service Web de messagerie unifiée pour un utilisateur à extension messagerie meilleures.  <br/> |
|[EwsPartnerUrl (POX)](ewspartnerurl-pox.md) <br/> |Spécifie l’URL de l’instance de point de terminaison meilleures pour Exchange Web Services (EWS) pour un utilisateur à extension messagerie.  <br/> |
|[LoginName (POX)](loginname-pox.md) <br/> |Spécifie le nom d’ouverture de session.  <br/> |
|[DomainRequired (POX)](domainrequired-pox.md) <br/> |Indique si le domaine est requis pour l’authentification.  <br/> |
|[DomainName (POX)](domainname-pox.md) <br/> |Spécifie le domaine de l’utilisateur.  <br/> |
|[SPA (POX)](spa-pox.md) <br/> |Indique si l’authentification du mot de passe sécurisé est nécessaire.  <br/> |
|[AuthPackage (POX)](authpackage-pox.md) <br/> |Spécifie le schéma d’authentification utilisé lors de l’authentification par rapport à l’ordinateur Exchange 2007 ayant le rôle de serveur de boîtes aux lettres est installé.  <br/> |
|[CertPrincipalName (POX)](certprincipalname-pox.md) <br/> |Spécifie le nom principal du certificat Secure Sockets Layer (SSL) qui est nécessaire pour se connecter à l’organisation Microsoft Exchange à l’aide de SSL.  <br/> |
|[SSL (POX)](ssl-pox.md) <br/> |Indique si une connexion sécurisée est nécessaire.  <br/> |
|[AuthRequired (POX)](authrequired-pox.md) <br/> |Spécifie si l’authentification est requise.  <br/> |
|[UsePOPAuth (POX)](usepopauth-pox.md) <br/> |Indique si les informations d’authentification qui sont fournies pour un type de POP3 de compte sont également utilisées pour SMTP Simple Mail Transfer Protocol ().  <br/> |
|[SMTPLast (POX)](smtplast-pox.md) <br/> |Indique si le serveur SMTP nécessite que courrier électronique doit être téléchargée avant qu’il envoie un message électronique à l’aide du serveur SMTP.  <br/> |
|[NetworkRequirements (POX)](networkrequirements-pox.md) <br/> |Contient les critères utilisés pour déterminer si l’ordinateur client est sur un réseau qui répond aux exigences du fournisseur de services Internet pour se connecter au serveur.  <br/> |
|[Carnet d’adresses (POX)](addressbook-pox.md) <br/> |Contient les spécifications pour la connexion d’un client pour le serveur de carnet d’adresses à l’aide du protocole MAPI/HTTP. Cet élément est présent uniquement si l’attribut **Type** de l’élément de **protocole** est présente et définie sur « mapiHttp ». L’élément de **Carnet d’adresses** est applicable aux clients qui implémentent le protocole MAPI/HTTP et cible Exchange Online et les versions d’Exchange commençant par 15.00.0847.032.  <br/> |
|[Magasin de courrier électronique (POX)](mailstore-pox.md) <br/> |Contient les spécifications pour connecter un client à la boîte aux lettres de l’utilisateur à l’aide du protocole MAPI/HTTP. Cet élément est présent uniquement si l’attribut **Type** de l’élément de **protocole** est présente et définie sur « mapiHttp ». L’élément de **magasin de courrier électronique** est applicable aux clients qui implémentent le protocole MAPI/HTTP et cible Exchange Online et les versions d’Exchange commençant par 15.00.0847.032.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Compte (POX)](account-pox.md) <br/> |Spécifie les paramètres de compte pour l’utilisateur.  <br/> |
   
## <a name="remarks"></a>Remarques

L’élément de **protocole** est présente dans une réponse qui comporte une valeur [d’Action (POX)](action-pox.md) est égale aux **paramètres**.
  
## <a name="see-also"></a>Voir aussi



[Éléments du fichier XML Autodiscover variole pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)


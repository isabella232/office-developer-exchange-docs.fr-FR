---
title: Protocol (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: f77e4d66-6fdd-4999-9339-f7d7f9c86f44
description: L’élément Protocol contient les spécifications de connexion d’un client à l’ordinateur qui exécute Exchange Server et sur lequel le rôle de serveur d’accès au client est installé.
ms.openlocfilehash: 6fca347f49e27958ecb16cce345387b6a2146979
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467759"
---
# <a name="protocol-pox"></a>Protocol (POX)

L’élément **Protocol** contient les spécifications de connexion d’un client à l’ordinateur qui exécute Exchange Server et sur lequel le rôle de serveur d’accès au client est installé. 
  
[Découverte automatique (POX)](autodiscover-pox.md)
  
[Réponse (POX)](response-pox.md)
  
[Compte (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
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

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|Type  <br/> |Indique le type de protocole décrit par cet élément de **protocole** . La seule valeur valide pour cet attribut est « MAPI ». Cet attribut est présent uniquement si la demande de découverte automatique correspondant à cette réponse [inclut un en-tête X-MapiHttpCapability](pox-autodiscover-request-for-exchange.md). Cet attribut est applicable aux clients qui implémentent le protocole MAPI/HTTP et ciblent Exchange Online, Exchange Online dans le cadre d’Office 365 ou les versions locales d’Exchange à partir de Build 15.00.0847.032 (Exchange Server 2013 SP1).  <br/> |
|Version  <br/> |Indique la version du protocole décrit par cet élément de **protocole** . La seule valeur valide pour cet attribut est « 1 ». Cet attribut est présent uniquement si la demande de découverte automatique correspondant à cette réponse inclut un en-tête **X-MapiHttpCapability** . Cet attribut est applicable aux clients qui implémentent le protocole MAPI/HTTP et ciblent Exchange Online, Exchange Online dans le cadre d’Office 365 ou les versions locales d’Exchange à partir de Build 15.00.0847.032 (Exchange Server 2013 SP1).  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Type (POX)](type-pox.md) <br/> |Identifie le type de compte de messagerie configuré.  <br/> |
|[Interne (POX)](internal-pox.md) <br/> |Contient une collection d’URL qu’un client peut utiliser pour se connecter à Exchange à l’intérieur du réseau de l’organisation.  <br/> |
|[Externe (POX)](external-pox.md) <br/> |Contient une collection d’URL qu’un client peut utiliser pour se connecter à Exchange depuis l’extérieur du réseau de l’organisation.  <br/> |
|[TTL (POX)](ttl-pox.md) <br/> |Spécifie la durée de vie, en heures, pendant laquelle les paramètres restent valides.  <br/> |
|[Serveur (POX)](server-pox.md) <br/> |Spécifie le nom du serveur de messagerie.  <br/> |
|[ServerDN (POX)](serverdn-pox.md) <br/> |Spécifie le nom unique du serveur Exchange.  <br/> |
|[ServerVersion (POX)](serverversion-pox.md) <br/> |Représente le numéro de version d’Exchange Server.  <br/> |
|[MdbDN (POX)](mdbdn-pox.md) <br/> |Représente le nom unique de la base de données de boîtes aux lettres.  <br/> |
|[PublicFolderServer (POX)](publicfolderserver-pox.md) <br/> |Contient le nom de domaine complet (FQDN) du serveur de dossiers publics de l’utilisateur.  <br/> |
|[Port (POX)](port-pox.md) <br/> |Spécifie le port utilisé pour se connecter à la Banque.  <br/> |
|[DirectoryPort (POX)](directoryport-pox.md) <br/> |Spécifie le port utilisé pour se connecter à l’annuaire lorsque le protocole NSPI (Name Service Provider Interface) est utilisé.  <br/> |
|[ReferralPort (POX)](referralport-pox.md) <br/> |Spécifie le port utilisé pour obtenir une référence à un annuaire.  <br/> |
|[ASUrl (POX)](asurl-pox.md) <br/> |Spécifie l’URL de la meilleure instance des services Web Exchange pour un utilisateur à extension messagerie.  <br/> |
|[EwsUrl (POX)](ewsurl-pox.md) <br/> |Spécifie l’URL de la meilleure instance de point de terminaison pour les services Web Exchange (EWS) pour un utilisateur à extension messagerie.  <br/> |
|[EmwsUrl (POX)](emwsurl-pox.md) <br/> |Spécifie l’URL de la meilleure instance de point de terminaison pour les services Web Exchange (EWS) pour un utilisateur à extension messagerie.  <br/> |
|[SharingUrl (POX)](sharingurl-pox.md) <br/> |Contient l’URL du serveur de partage utilisé pour le partage entre les organisations des calendriers et des contacts.  <br/> |
|[EcpUrl (POX)](ecpurl-pox.md) <br/> |Spécifie l’URL du panneau de configuration Exchange pour un utilisateur à extension messagerie.  <br/> |
|[EcpUrl-messagerie unifiée (POX)](ecpurl-um-pox.md) <br/> |Spécifie une URL partielle pouvant être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour accéder aux paramètres de messagerie vocale d’un utilisateur à extension messagerie.  <br/> |
|[EcpUrl-aggr (POX)](ecpurl-aggr-pox.md) <br/> |Spécifie une URL partielle pouvant être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour accéder aux paramètres d’agrégation de courrier électronique pour un utilisateur à extension messagerie.  <br/> |
|[EcpUrl-MT (POX)](ecpurl-mt-pox.md) <br/> |Spécifie une URL partielle pouvant être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour accéder aux paramètres de suivi des messages électroniques pour un utilisateur à extension messagerie.  <br/> |
|[EcpUrl-RET (POX)](ecpurl-ret-pox.md) <br/> |Spécifie une URL partielle pouvant être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour accéder aux paramètres des balises de rétention pour un utilisateur à extension messagerie.  <br/> |
|[EcpUrl-SMS (POX)](ecpurl-sms-pox.md) <br/> |Spécifie une URL partielle pouvant être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour accéder aux paramètres SMS (Short Message Service) pour un utilisateur à extension messagerie.  <br/> |
|[EcpUrl-Publish (POX)](ecpurl-publish-pox.md) <br/> |Spécifie une URL partielle pouvant être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour accéder aux paramètres de publication de calendrier pour un utilisateur à extension messagerie.  <br/> |
|[EcpUrl-photo (POX)](ecpurl-photo-pox.md) <br/> |Spécifie une URL partielle pouvant être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour afficher ou modifier la photo actuelle d’un utilisateur à extension messagerie.  <br/> |
|[EcpUrl-TM (POX)](ecpurl-tm-pox.md) <br/> |Spécifie une URL partielle qui peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour accéder à une liste de toutes les boîtes aux lettres de site dont un utilisateur à extension messagerie est actuellement membre.  <br/> |
|[EcpUrl-tmCreating (POX)](ecpurl-tmcreating-pox.md) <br/> |Spécifie une URL partielle pouvant être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour créer une nouvelle boîte aux lettres de site.  <br/> |
|[EcpUrl-tmHiding (POX)](ecpurl-tmhiding-pox.md) <br/> |Spécifie une URL partielle pouvant être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour annuler l’abonnement de l’utilisateur à partir d’une boîte aux lettres de site.  <br/> |
|[EcpUrl-tmEditing (POX)](ecpurl-tmediting-pox.md) <br/> |Spécifie une URL partielle pouvant être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour modifier une boîte aux lettres de site existante.  <br/> |
|[EcpUrl-extinstall (POX)](ecpurl-extinstall-pox.md) <br/> |Spécifie une URL partielle qui peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour afficher ou modifier les applications de messagerie actuellement installées dans la boîte aux lettres de l’utilisateur.  <br/> |
|[OOFUrl (POX)](oofurl-pox.md) <br/> |Spécifie l’URL de la meilleure instance du service de disponibilité pour un utilisateur à extension messagerie.  <br/> |
|[OABUrl (POX)](oaburl-pox.md) <br/> |Spécifie l’URL du serveur de configuration du carnet d’adresses en mode hors connexion pour une topologie Exchange.  <br/> |
|[UMUrl (POX)](umurl-pox.md) <br/> |Spécifie l’URL de la meilleure instance du service Web de messagerie unifiée pour un utilisateur à extension messagerie.  <br/> |
|[EwsPartnerUrl (POX)](ewspartnerurl-pox.md) <br/> |Spécifie l’URL de la meilleure instance de point de terminaison pour les services Web Exchange (EWS) pour un utilisateur à extension messagerie.  <br/> |
|[LoginName (POX)](loginname-pox.md) <br/> |Spécifie le nom de connexion de l’utilisateur.  <br/> |
|[DomainRequired (POX)](domainrequired-pox.md) <br/> |Indique si le domaine est requis pour l’authentification.  <br/> |
|[Nom_domaine (POX)](domainname-pox.md) <br/> |Spécifie le domaine de l’utilisateur.  <br/> |
|[SPA (POX)](spa-pox.md) <br/> |Indique si l’authentification par mot de passe sécurisé est requise.  <br/> |
|[Package (POX)](authpackage-pox.md) <br/> |Spécifie le modèle d’authentification utilisé lors de l’authentification auprès de l’ordinateur Exchange 2007 sur lequel le rôle serveur de boîtes aux lettres est installé.  <br/> |
|[CertPrincipalName (POX)](certprincipalname-pox.md) <br/> |Spécifie le nom de principal du certificat SSL (Secure Sockets Layer) qui est requis pour se connecter à l’organisation Microsoft Exchange à l’aide de SSL.  <br/> |
|[SSL (POX)](ssl-pox.md) <br/> |Indique si la connexion sécurisée est nécessaire.  <br/> |
|[AuthRequired (POX)](authrequired-pox.md) <br/> |Indique si l’authentification est requise.  <br/> |
|[UsePOPAuth (POX)](usepopauth-pox.md) <br/> |Indique si les informations d’authentification fournies pour un type de compte POP3 sont également utilisées pour le protocole SMTP (Simple Mail Transfer Protocol).  <br/> |
|[SMTPLast (POX)](smtplast-pox.md) <br/> |Indique si le serveur SMTP requiert le téléchargement du courrier électronique avant qu’il envoie des messages électroniques à l’aide du serveur SMTP.  <br/> |
|[NetworkRequirements (POX)](networkrequirements-pox.md) <br/> |Contient les critères utilisés pour déterminer si l’ordinateur client est sur un réseau qui répond aux exigences du fournisseur de services Internet pour se connecter au serveur.  <br/> |
|[AddressBook (POX)](addressbook-pox.md) <br/> |Contient les spécifications relatives à la connexion d’un client au serveur de carnet d’adresses à l’aide du protocole MAPI/HTTP. Cet élément est présent uniquement si l’attribut **type** de l’élément **Protocol** est présent et défini sur « MAPI ». L’élément **AddressBook** est applicable aux clients qui implémentent le protocole MAPI/http et qui ciblent Exchange Online et les versions d’Exchange à partir de 15.00.0847.032.  <br/> |
|[MailStore (POX)](mailstore-pox.md) <br/> |Contient les spécifications relatives à la connexion d’un client à la boîte aux lettres de l’utilisateur à l’aide du protocole MAPI/HTTP. Cet élément est présent uniquement si l’attribut **type** de l’élément **Protocol** est présent et défini sur « MAPI ». L’élément **mailstore** est applicable aux clients qui implémentent le protocole MAPI/http et qui ciblent Exchange Online et les versions d’Exchange à partir de 15.00.0847.032.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Compte (POX)](account-pox.md) <br/> |Spécifie les paramètres de compte de l’utilisateur.  <br/> |
   
## <a name="remarks"></a>Remarques

L’élément **Protocol** est présent dans une réponse dont la valeur [action (POX)](action-pox.md) est égale aux **paramètres**.
  
## <a name="see-also"></a>Voir aussi



[Éléments XML de découverte automatique de la VARIOle pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)


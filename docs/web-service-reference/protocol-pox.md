---
title: Protocol (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: f77e4d66-6fdd-4999-9339-f7d7f9c86f44
description: L’élément Protocol contient les spécifications de connexion d’un client à l’ordinateur qui exécute Exchange Server sur qui le rôle serveur d’accès au client est installé.
ms.openlocfilehash: 4f308951c74612936755e6d4c16620e38277aecb
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516397"
---
# <a name="protocol-pox"></a>Protocol (POX)

**L’élément Protocol** contient les spécifications de connexion d’un client à l’ordinateur qui exécute Exchange Server sur le rôle serveur d’accès au client installé. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
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
|Type  <br/> |Indique le type de protocole décrit par cet **élément Protocol.** La seule valeur valide pour cet attribut est « mapiHttp ». Cet attribut est uniquement présent si la demande de découverte automatique qui correspond à cette réponse incluait un [en-tête X-MapiHttpCapability](pox-autodiscover-request-for-exchange.md). Cet attribut s’applique aux clients qui implémentent le protocole MAPI/HTTP et les Exchange Online, Exchange Online cibles dans le cadre de Office 365 ou des versions sur site de Exchange à partir de la build 15.00.0847.032 (Exchange Server 2013 SP1).  <br/> |
|Version  <br/> |Indique la version du protocole décrite par cet **élément Protocol.** La seule valeur valide pour cet attribut est « 1 ». Cet attribut n’est présent que si la demande de découverte automatique qui correspond à cette réponse incluait un **en-tête X-MapiHttpCapability.** Cet attribut s’applique aux clients qui implémentent le protocole MAPI/HTTP et les Exchange Online, Exchange Online cibles dans le cadre de Office 365 ou des versions sur site de Exchange à partir de la build 15.00.0847.032 (Exchange Server 2013 SP1).  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Type (POX)](type-pox.md) <br/> |Identifie le type du compte de messagerie configuré.  <br/> |
|[Internal (POX)](internal-pox.md) <br/> |Contient une collection d’URL qu’un client peut utiliser pour se connecter à Exchange à partir de l’intérieur du réseau de l’organisation.  <br/> |
|[External (POX)](external-pox.md) <br/> |Contient une collection d’URL qu’un client peut utiliser pour se connecter à Exchange en dehors du réseau de l’organisation.  <br/> |
|[TTL (POX)](ttl-pox.md) <br/> |Spécifie l’heure de vie, en heures, pendant laquelle les paramètres restent valides.  <br/> |
|[Server (POX)](server-pox.md) <br/> |Spécifie le nom du serveur de messagerie.  <br/> |
|[ServerDN (POX)](serverdn-pox.md) <br/> |Spécifie le nom Exchange Server nom.  <br/> |
|[ServerVersion (POX)](serverversion-pox.md) <br/> |Représente le numéro Exchange Server version.  <br/> |
|[MdbDN (POX)](mdbdn-pox.md) <br/> |Représente le nom unique de la base de données de boîtes aux lettres.  <br/> |
|[PublicFolderServer (POX)](publicfolderserver-pox.md) <br/> |Contient le nom de domaine complet (FQDN) du serveur de dossiers publics pour l’utilisateur.  <br/> |
|[Port (POX)](port-pox.md) <br/> |Spécifie le port utilisé pour se connecter au magasin.  <br/> |
|[DirectoryPort (POX)](directoryport-pox.md) <br/> |Spécifie le port utilisé pour se connecter à l’annuaire lorsque le protocole NSPI (Name Service Provider Interface) est utilisé.  <br/> |
|[ReferralPort (POX)](referralport-pox.md) <br/> |Spécifie le port utilisé pour obtenir une référence à un répertoire.  <br/> |
|[ASUrl (POX)](asurl-pox.md) <br/> |Spécifie l’URL de la meilleure instance des services web Exchange pour un utilisateur à messagerie.  <br/> |
|[EwsUrl (POX)](ewsurl-pox.md) <br/> |Spécifie l’URL de la meilleure instance de point de terminaison pour Exchange Web Services (EWS) pour un utilisateur à messagerie.  <br/> |
|[EmwsUrl (POX)](emwsurl-pox.md) <br/> |Spécifie l’URL de la meilleure instance de point de terminaison pour Exchange Web Services (EWS) pour un utilisateur à messagerie.  <br/> |
|[SharingUrl (POX)](sharingurl-pox.md) <br/> |Contient l’URL du serveur de partage utilisé pour le partage entre les organisations des calendriers et des contacts.  <br/> |
|[EcpUrl (POX)](ecpurl-pox.md) <br/> |Spécifie l’URL du Panneau de Exchange pour un utilisateur à messagerie.  <br/> |
|[EcpUrl-um (POX)](ecpurl-um-pox.md) <br/> |Spécifie une URL partielle qui peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour accéder aux paramètres de messagerie vocale d’un utilisateur à extension messagerie.  <br/> |
|[EcpUrl-aggr (POX)](ecpurl-aggr-pox.md) <br/> |Spécifie une URL partielle qui peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour accéder aux paramètres d’agrégation de courrier électronique pour un utilisateur à extension messagerie.  <br/> |
|[EcpUrl-mt (POX)](ecpurl-mt-pox.md) <br/> |Spécifie une URL partielle qui peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour accéder aux paramètres de suivi des messages électroniques pour un utilisateur à extension messagerie.  <br/> |
|[EcpUrl-ret (POX)](ecpurl-ret-pox.md) <br/> |Spécifie une URL partielle qui peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour accéder aux paramètres de balise de rétention d’un utilisateur à extension messagerie.  <br/> |
|[EcpUrl-sms (POX)](ecpurl-sms-pox.md) <br/> |Spécifie une URL partielle qui peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour accéder aux paramètres SMS (Short Message Service) d’un utilisateur à extension messagerie.  <br/> |
|[EcpUrl-publish (POX)](ecpurl-publish-pox.md) <br/> |Spécifie une URL partielle qui peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour accéder aux paramètres de publication de calendrier pour un utilisateur à extension messagerie.  <br/> |
|[EcpUrl-photo (POX)](ecpurl-photo-pox.md) <br/> |Spécifie une URL partielle qui peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour afficher ou modifier la photo actuelle d’un utilisateur à extension messagerie.  <br/> |
|[EcpUrl-tm (POX)](ecpurl-tm-pox.md) <br/> |Spécifie une URL partielle qui peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour accéder à la liste de toutes les boîtes aux lettres de site dont un utilisateur à extension messagerie est actuellement membre.  <br/> |
|[EcpUrl-tmCreating (POX)](ecpurl-tmcreating-pox.md) <br/> |Spécifie une URL partielle qui peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour créer une boîte aux lettres de site.  <br/> |
|[EcpUrl-tmHiding (POX)](ecpurl-tmhiding-pox.md) <br/> |Spécifie une URL partielle qui peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour désabonner l’utilisateur d’une boîte aux lettres de site.  <br/> |
|[EcpUrl-tmEditing (POX)](ecpurl-tmediting-pox.md) <br/> |Spécifie une URL partielle qui peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour modifier une boîte aux lettres de site existante.  <br/> |
|[EcpUrl-extinstall (POX)](ecpurl-extinstall-pox.md) <br/> |Spécifie une URL partielle qui peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour afficher ou modifier les applications de messagerie actuellement installées dans la boîte aux lettres de l’utilisateur.  <br/> |
|[OOFUrl (POX)](oofurl-pox.md) <br/> |Spécifie l’URL de la meilleure instance du service de disponibilité pour un utilisateur à messagerie.  <br/> |
|[OABUrl (POX)](oaburl-pox.md) <br/> |Spécifie l’URL du serveur de configuration du carnet d’adresses en mode hors connexion pour Exchange topologie.  <br/> |
|[UMUrl (POX)](umurl-pox.md) <br/> |Spécifie l’URL de la meilleure instance du service Web de messagerie unifiée pour un utilisateur à messagerie.  <br/> |
|[EwsPartnerUrl (POX)](ewspartnerurl-pox.md) <br/> |Spécifie l’URL de la meilleure instance de point de terminaison pour Exchange Web Services (EWS) pour un utilisateur à messagerie.  <br/> |
|[LoginName (POX)](loginname-pox.md) <br/> |Spécifie le nom de la logon de l’utilisateur.  <br/> |
|[DomainRequired (POX)](domainrequired-pox.md) <br/> |Indique si le domaine est requis pour l’authentification.  <br/> |
|[DomainName (POX)](domainname-pox.md) <br/> |Spécifie le domaine de l’utilisateur.  <br/> |
|[SPA (POX)](spa-pox.md) <br/> |Indique si l’authentification par mot de passe sécurisé est requise.  <br/> |
|[AuthPackage (POX)](authpackage-pox.md) <br/> |Spécifie le schéma d’authentification utilisé lors de l’authentification sur l Exchange 2007 sur l’ordinateur sur qui le rôle serveur de boîtes aux lettres est installé.  <br/> |
|[CertPrincipalName (POX)](certprincipalname-pox.md) <br/> |Spécifie le nom principal du certificat SSL (Secure Sockets Layer) requis pour se connecter à l’organisation Microsoft Exchange à l’aide de SSL.  <br/> |
|[SSL (POX)](ssl-pox.md) <br/> |Spécifie si une logonisation sécurisée est nécessaire.  <br/> |
|[AuthRequired (POX)](authrequired-pox.md) <br/> |Spécifie si l’authentification est requise.  <br/> |
|[UsePOPAuth (POX)](usepopauth-pox.md) <br/> |Indique si les informations d’authentification fournies pour un type de compte POP3 sont également utilisées pour SMTP (Simple Mail Transfer Protocol).  <br/> |
|[SMTPLast (POX)](smtplast-pox.md) <br/> |Spécifie si le serveur SMTP requiert que le courrier électronique soit téléchargé avant d’envoyer des messages électroniques à l’aide du serveur SMTP.  <br/> |
|[NetworkRequirements (POX)](networkrequirements-pox.md) <br/> |Contient les critères utilisés pour déterminer si l’ordinateur client se trouve sur un réseau qui répond aux exigences du fournisseur de services Internet pour se connecter au serveur.  <br/> |
|[AddressBook (POX)](addressbook-pox.md) <br/> |Contient les spécifications de connexion d’un client au serveur de carnet d’adresses à l’aide du protocole MAPI/HTTP. Cet élément n’est présent que si l’attribut **Type** de l’élément **Protocol** est présent et a la valeur « mapiHttp ». L’élément **AddressBook** s’applique aux clients qui implémentent le protocole MAPI/HTTP et aux Exchange Online cibles et aux versions de Exchange à partir de 15.00.0847.032.  <br/> |
|[MailStore (POX)](mailstore-pox.md) <br/> |Contient les spécifications de connexion d’un client à la boîte aux lettres de l’utilisateur à l’aide du protocole MAPI/HTTP. Cet élément n’est présent que si l’attribut **Type** de l’élément **Protocol** est présent et a la valeur « mapiHttp ». L’élément **MailStore** s’applique aux clients qui implémentent le protocole MAPI/HTTP et aux Exchange Online cibles et aux versions de Exchange à partir de 15.00.0847.032.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Account (POX)](account-pox.md) <br/> |Spécifie les paramètres de compte de l’utilisateur.  <br/> |
   
## <a name="remarks"></a>Remarques

**L’élément Protocol** est présent dans une réponse qui a une valeur [Action (POX)](action-pox.md) égale aux **paramètres.**
  
## <a name="see-also"></a>Voir aussi



[Éléments XML de découverte automatique POX pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)


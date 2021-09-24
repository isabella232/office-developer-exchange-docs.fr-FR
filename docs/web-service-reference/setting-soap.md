---
title: Setting (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 43db26e1-f7be-49fd-b26b-fc1b10bd3458
description: L’élément Setting représente un paramètre de configuration à retourner.
ms.openlocfilehash: 2e03bfacaf36676ee4687c148f3b08732a9f17b1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539142"
---
# <a name="setting-soap"></a>Setting (SOAP)

**L’élément Setting** représente un paramètre de configuration à retourner. 
  
```XML
<Setting/>
```

 **chaîne**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[RequestedSettings (SOAP)](requestedsettings-soap.md) <br/> |Contient les noms des paramètres de configuration demandés.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte de cet élément est le paramètre de configuration. Le tableau suivant répertorie les paramètres de configuration possibles.
  
|**Paramètre de configuration**|**Description**|
|:-----|:-----|
|UserDisplayName  <br/> |Nom d’affichage de l’utilisateur.  <br/> |
|UserDN  <br/> |Nom hérité de l’utilisateur.  <br/> |
|UserDeploymentId  <br/> |Identificateur de déploiement de l’utilisateur.  <br/> |
|InternalMailboxServer  <br/> |Nom de domaine complet (FQDN) du serveur de boîtes aux lettres.  <br/> |
|InternalRpcClientServer  <br/> |Nom de domaine complet du serveur client RPC.  <br/> |
|InternalMailboxServerDN  <br/> |Nom hérité du serveur de boîtes aux lettres.  <br/> |
|InternalEcpUrl  <br/> |URL interne du Panneau de Exchange de contrôle.  <br/> |
|InternalEcpVoicemailUrl  <br/> |URL interne du Panneau de Exchange pour la personnalisation de la messagerie vocale.  <br/> |
|InternalEcpEmailSubscriptionsUrl  <br/> |URL interne du Panneau de Exchange pour les abonnements de messagerie.  <br/> |
|InternalEcpTextMessagingUrl  <br/> |URL interne du Panneau de Exchange pour la messagerie texte.  <br/> |
|InternalEcpDeliveryReportUrl  <br/> |URL interne du Panneau de Exchange pour les rapports de remise.  <br/> |
|InternalEcpRetentionPolicyTagsUrl  <br/> |URL interne du Panneau de Exchange pour les balises RetentionPolicy.  <br/> |
|InternalEcpPublishingUrl  <br/> |URL interne du Panneau de Exchange pour la publication.  <br/> |
|InternalEwsUrl  <br/> |URL interne des services web Exchange web.  <br/> |
|InternalOABUrl  <br/> |URL interne du carnet d’adresses en mode hors connexion.  <br/> |
|InternalUMUrl  <br/> |URL interne des services de messagerie unifiée.  <br/> |
|InternalWebClientUrls  <br/> |URL internes du client Exchange Web.  <br/> |
|MailboxDN  <br/> |Nom unique de la base de données de boîtes aux lettres de la boîte aux lettres de l’utilisateur.  <br/> |
|PublicFolderServer  <br/> |Nom du serveur de dossiers publics.  <br/> |
|ActiveDirectoryServer  <br/> |Nom du serveur Active Directory.  <br/> |
|ExternalMailboxServer  <br/> |Nom du serveur RPC sur HTTP.  <br/> |
|ExternalMailboxServerRequiresSSL  <br/> |Indicateur qui permet de déterminer si le serveur RPC sur HTTP requiert SSL.  <br/> |
|ExternalMailboxServerAuthenticationMethods  <br/> |Méthodes d’authentification qui sont pris en charge par le serveur RPC sur HTTP.  <br/> |
|EcpVoicemailUrlFragment,  <br/> |Fragment d’URL du Panneau de Exchange pour la personnalisation de la messagerie vocale.  <br/> |
|EcpEmailSubscriptionsUrlFragment  <br/> |Fragment d’URL du Panneau de Exchange pour les abonnements de messagerie.  <br/> |
|EcpTextMessagingUrlFragment  <br/> |Fragment d’URL du Panneau de Exchange pour la messagerie texte.  <br/> |
|EcpDeliveryReportUrlFragment  <br/> |Fragment d’URL du Panneau de Exchange pour les rapports de remise.  <br/> |
|EcpRetentionPolicyTagsUrlFragment  <br/> |Fragment d’URL du Panneau de Exchange de rétention pour les balises RetentionPolicy.  <br/> |
|EcpPublishingUrlFragment  <br/> |Fragment d’URL du Panneau de Exchange pour la publication.  <br/> |
|ExternalEcpUrl  <br/> |URL externe du Panneau de Exchange de contrôle.  <br/> |
|ExternalEcpVoicemailUrl  <br/> |URL externe du Panneau de Exchange pour la personnalisation de la messagerie vocale.  <br/> |
|ExternalEcpEmailSubscriptionsUrl  <br/> |URL externe du Panneau de Exchange pour les abonnements de messagerie.  <br/> |
|ExternalEcpTextMessagingUrl  <br/> |URL externe du Panneau de Exchange pour la messagerie texte.  <br/> |
|ExternalEcpDeliveryReportUrl  <br/> |URL externe du Panneau de Exchange pour les rapports de remise.  <br/> |
|ExternalEcpRetentionPolicyTagsUrl  <br/> |URL externe du Panneau de Exchange pour les balises RetentionPolicy.  <br/> |
|ExternalEcpPublishingUrl  <br/> |URL externe du Panneau de Exchange pour la publication.  <br/> |
|ExternalEwsUrl  <br/> |URL externe des services Exchange Web.  <br/> |
|ExternalOABUrl  <br/> |URL externe du OAB.  <br/> |
|ExternalUMUrl  <br/> |URL externe des services de messagerie unifiée.  <br/> |
|ExternalWebClientUrls  <br/> |URL externes du client Exchange Web.  <br/> |
|CrossOrganizationSharingEnabled  <br/> |Indique que le partage entre les organisations est activé.  <br/> |
|AlternateMailboxes  <br/> |Collection de boîtes aux lettres de remplacement.  <br/> |
|CasVersion  <br/> |Version du serveur d’accès au client qui sert la demande (par exemple, 14.XX.YYYY. ZZZ)  <br/> |
|EwsSupportedSchemas  <br/> |Liste de versions de schémas séparées par des virgules, prise en charge par Exchange Web Services. Les valeurs de version du schéma seront identiques aux valeurs de l’éumération **ExchangeServerVersion.**  <br/> |
|InternalPop3Connections  <br/> |Liste des paramètres de connexion interne pour les connexions au protocole POP3.  <br/> |
|ExternalPop3Connections  <br/> |Liste des paramètres de connexion externe pour les connexions au protocole POP3.  <br/> |
|InternalImap4Connections  <br/> |Liste des paramètres de connexion interne pour les connexions au protocole IMAP4.  <br/> |
|ExternalImap4Connections  <br/> |Liste des paramètres de connexion externe pour les connexions au protocole IMAP4.  <br/> |
|InternalSmtpConnections  <br/> |Liste des paramètres de connexion interne pour les connexions SMTP.  <br/> |
|ExternalSmtpConnections  <br/> |Liste des paramètres de connexion externe pour les connexions SMTP.  <br/> |
|InternalServerExclusiveConnect  <br/> |Indicateur de connexion exclusive du serveur interne. Si ce protocole est « Off », les clients ne doivent pas se connecter via ce protocole.  <br/> |
|ExternalServerExclusiveConnect  <br/> |Indicateur de connexion exclusive du serveur externe. Si ce protocole est « On », les clients doivent se connecter via ce protocole.  <br/> |
|ExchangeRpcUrl  <br/> |URL utilisée pour les appels de procédure distante. Cette URL est interne au serveur et ne doit pas être utilisée par les clients.  <br/> |
|ShowGalAsDefaultView  <br/> |Spécifie une valeur de booléen qui indique si la LAL doit être affichée en tant que carnet d’adresses. Une valeur de texte « true » indique que la LAL doit être affichée par défaut. La valeur « false » indique que la liste des contacts doit être affichée.  <br/> |
|AutoDiscoverSMTPAddress  <br/> |Adresse SMTP principale de découverte automatique pour l’utilisateur. Il s’agit de l’adresse proxy au lieu de l’adresse de messagerie de l’utilisateur, si une adresse proxy existe.  <br/> |
|InteropExternalEwsUrl  <br/> |URL externe du point de terminaison du service Web du serveur. Il s’agit de l’URL d’un serveur qui peut servir des boîtes aux lettres hébergées sur un serveur qui n’a pas les services Web.  <br/> |
|ExternalEwsVersion  <br/> |Version du serveur de services Web qui fournit la demande spécifiée.  <br/> |
|InteropExternalEwsVersion  <br/> |La version du serveur InteropExternalEwsUrl pointe vers.  <br/> |
|MobileMailboxPolicyInterop  <br/> |Paramètres de stratégie de boîte aux lettres mobile.  <br/> |
|GroupingInformation  <br/> |Valeur utilisée conjointement avec le paramètre ExternalEwsUrl pour [](https://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx) grouper plusieurs boîtes aux lettres afin de conserver l’affinité lors de l’abonnement aux notifications.  <br/> |
|UserMSOnline  <br/> |Valeur Boolean qui indique si la boîte aux lettres de l’utilisateur est hébergée dans Exchange Online ou Exchange Online dans le cadre de Office 365.  <br/> |
|MapiHttpEnabled  <br/> |Valeur Boolean qui indique si la boîte aux lettres de l’utilisateur est accessible via le protocole MAPI/HTTP.  <br/> |
   
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetUserSettings (SOAP)](getusersettings-operation-soap.md)
  
[Opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)


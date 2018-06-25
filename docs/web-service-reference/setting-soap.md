---
title: Paramètre (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 43db26e1-f7be-49fd-b26b-fc1b10bd3458
description: L’élément de paramètre représente un paramètre de configuration à renvoyer.
ms.openlocfilehash: cb5b1d6ab2109b48810b96221b76c6b8fc9803ac
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829472"
---
# <a name="setting-soap"></a>Paramètre (SOAP)

L’élément de **paramètre** représente un paramètre de configuration à renvoyer. 
  
```XML
<Setting/>
```

 **string**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[RequestedSettings (SOAP)](requestedsettings-soap.md) <br/> |Contient les noms des paramètres de configuration demandé.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de texte pour cet élément est le paramètre de configuration. Le tableau suivant répertorie les paramètres de configuration possibles.
  
|**Paramètre de configuration**|**Description**|
|:-----|:-----|
|UserDisplayName  <br/> |Le nom complet de l’utilisateur.  <br/> |
|NUUtilisateur  <br/> |Le nom unique hérité de l’utilisateur.  <br/> |
|UserDeploymentId  <br/> |L’identificateur de déploiement de l’utilisateur.  <br/> |
|InternalMailboxServer  <br/> |Le nom de domaine complet (FQDN) du serveur de boîtes aux lettres.  <br/> |
|InternalRpcClientServer  <br/> |Le nom de domaine complet du serveur client RPC.  <br/> |
|InternalMailboxServerDN  <br/> |Le nom unique hérité du serveur de boîtes aux lettres.  <br/> |
|InternalEcpUrl  <br/> |L’URL interne du Panneau de configuration Exchange.  <br/> |
|InternalEcpVoicemailUrl  <br/> |L’URL interne du Panneau de configuration Exchange pour la personnalisation de la messagerie vocale.  <br/> |
|InternalEcpEmailSubscriptionsUrl  <br/> |L’URL interne du Panneau de configuration Exchange pour les abonnements de messagerie.  <br/> |
|InternalEcpTextMessagingUrl  <br/> |L’URL interne du Panneau de configuration Exchange pour la messagerie texte.  <br/> |
|InternalEcpDeliveryReportUrl  <br/> |L’URL interne du Panneau de configuration Exchange pour les rapports de remise.  <br/> |
|InternalEcpRetentionPolicyTagsUrl  <br/> |L’URL interne du Panneau de configuration Exchange pour les balises RetentionPolicy.  <br/> |
|InternalEcpPublishingUrl  <br/> |L’URL interne du Panneau de configuration Exchange pour la publication.  <br/> |
|InternalEwsUrl  <br/> |L’URL de Exchange Web Services internes.  <br/> |
|InternalOABUrl  <br/> |L’URL interne du carnet d’adresses en mode hors connexion (OAB).  <br/> |
|InternalUMUrl  <br/> |L’URL interne de services de messagerie unifiée.  <br/> |
|InternalWebClientUrls  <br/> |Les URL internes du client Web Exchange.  <br/> |
|MailboxDN  <br/> |Le nom unique de la base de données de boîtes aux lettres de boîte aux lettres de l’utilisateur.  <br/> |
|PublicFolderServer  <br/> |Le nom du serveur de dossiers publics.  <br/> |
|ActiveDirectoryServer  <br/> |Le nom du serveur Active Directory.  <br/> |
|ExternalMailboxServer  <br/> |Nom de la RPC sur le serveur HTTP.  <br/> |
|ExternalMailboxServerRequiresSSL  <br/> |L’indicateur pour que RPC sur le serveur HTTP requiert une connexion SSL.  <br/> |
|ExternalMailboxServerAuthenticationMethods  <br/> |Les méthodes d’authentification prises en charge par le RPC sur le serveur HTTP.  <br/> |
|EcpVoicemailUrlFragment,  <br/> |Le fragment d’URL du Panneau de commande Exchange pour la personnalisation de la messagerie vocale.  <br/> |
|EcpEmailSubscriptionsUrlFragment  <br/> |Le fragment d’URL du Panneau de commande pour les abonnements de messagerie Exchange.  <br/> |
|EcpTextMessagingUrlFragment  <br/> |Le fragment d’URL du Panneau de commande Exchange pour la messagerie texte.  <br/> |
|EcpDeliveryReportUrlFragment  <br/> |Le fragment d’URL du Panneau de commande Exchange pour les rapports de remise.  <br/> |
|EcpRetentionPolicyTagsUrlFragment  <br/> |Le fragment d’URL du Panneau de commande Exchange pour les balises RetentionPolicy.  <br/> |
|EcpPublishingUrlFragment  <br/> |Le fragment d’URL du Panneau de commande Exchange pour la publication.  <br/> |
|ExternalEcpUrl  <br/> |L’URL externe du Panneau de configuration Exchange.  <br/> |
|ExternalEcpVoicemailUrl  <br/> |L’URL externe du Panneau de configuration Exchange pour la personnalisation de la messagerie vocale.  <br/> |
|ExternalEcpEmailSubscriptionsUrl  <br/> |L’URL externe du Panneau de configuration Exchange pour les abonnements de messagerie.  <br/> |
|ExternalEcpTextMessagingUrl  <br/> |L’URL externe du Panneau de configuration Exchange pour la messagerie texte.  <br/> |
|ExternalEcpDeliveryReportUrl  <br/> |L’URL externe du Panneau de configuration Exchange pour les rapports de remise.  <br/> |
|ExternalEcpRetentionPolicyTagsUrl  <br/> |L’URL externe du Panneau de configuration Exchange pour les balises RetentionPolicy.  <br/> |
|ExternalEcpPublishingUrl  <br/> |L’URL externe du Panneau de configuration Exchange pour la publication.  <br/> |
|ExternalEwsUrl  <br/> |L’URL externe des Services Web Exchange.  <br/> |
|ExternalOABUrl  <br/> |L’URL externe du carnet d’adresses.  <br/> |
|ExternalUMUrl  <br/> |L’URL externe des services de messagerie unifiée.  <br/> |
|ExternalWebClientUrls  <br/> |L’URL externes du client Web Exchange.  <br/> |
|CrossOrganizationSharingEnabled  <br/> |Indique que le partage de l’échelle de l’organisation est activé.  <br/> |
|AlternateMailboxes  <br/> |Collection d’autres boîtes aux lettres.  <br/> |
|CasVersion  <br/> |La version du serveur d’accès Client qui sert à la demande (par exemple, 14.XX. AAAA. ZZZ)  <br/> |
|EwsSupportedSchemas  <br/> |Une liste séparée par des virgules des versions de schéma pris en charge par les Services Web Exchange. Les valeurs de version de schéma sera la même que les valeurs de l’énumération **ExchangeServerVersion** .  <br/> |
|InternalPop3Connections  <br/> |La liste de paramètres de connexion interne pour les connexions de protocole POP3.  <br/> |
|ExternalPop3Connections  <br/> |La liste de paramètres de connexion externe pour les connexions de protocole POP3.  <br/> |
|InternalImap4Connections  <br/> |La liste de paramètres de connexion interne pour les connexions de protocole IMAP4.  <br/> |
|ExternalImap4Connections  <br/> |La liste de paramètres de connexion externe pour les connexions de protocole IMAP4.  <br/> |
|InternalSmtpConnections  <br/> |La liste de paramètres de connexion interne pour les connexions SMTP.  <br/> |
|ExternalSmtpConnections  <br/> |La liste de paramètres de connexion externe pour les connexions SMTP.  <br/> |
|InternalServerExclusiveConnect  <br/> |Le serveur interne exclusif se connecter indicateur. Si la valeur « Désactivé » dans clients puis ne doit pas se connecter via ce protocole.  <br/> |
|ExternalServerExclusiveConnect  <br/> |Le serveur externe exclusif se connecter indicateur. Si la valeur « Sur » puis clients doit se connecter via ce protocole.  <br/> |
|ExchangeRpcUrl  <br/> |L’URL utilisée pour les appels de procédure distante. Cette URL est interne au serveur et ne doit ne pas être utilisé par les clients.  <br/> |
|ShowGalAsDefaultView  <br/> |Spécifie une valeur de type Boolean qui indique si la liste d’adresses globale doit être affichée en tant que le carnet d’adresses. Une valeur de texte « True » indique que la liste d’adresses globale doit être affiché par défaut. Une valeur de texte « False » indique que la liste des contacts est à afficher.  <br/> |
|AutoDiscoverSMTPAddress  <br/> |L’adresse principale SMTP découverte automatique de l’utilisateur. Il s’agit de l’adresse proxy à la place de l’adresse de messagerie de l’utilisateur, si une adresse proxy existe.  <br/> |
|InteropExternalEwsUrl  <br/> |L’URL externe du point de terminaison de service du serveur Web. Il s’agit de l’URL vers un serveur qui peut servir des boîtes aux lettres hébergées sur un serveur qui n’a pas les services Web.  <br/> |
|ExternalEwsVersion  <br/> |La version du serveur de services Web qui fournit la requête spécifiée.  <br/> |
|InteropExternalEwsVersion  <br/> |Pointe vers la version du serveur InteropExternalEwsUrl.  <br/> |
|MobileMailboxPolicyInterop  <br/> |Les paramètres de stratégie de boîte aux lettres mobile.  <br/> |
|GroupingInformation  <br/> |Une valeur utilisée conjointement avec le paramètre ExternalEwsUrl pour regrouper plusieurs boîtes aux lettres afin de [mettre à jour l’affinité](http://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx) lors de l’abonnement aux notifications.  <br/> |
|UserMSOnline  <br/> |Une valeur de type Boolean qui indique si la boîte aux lettres de l’utilisateur est hébergée dans Exchange Online ou Exchange Online dans le cadre d’Office 365.  <br/> |
|MapiHttpEnabled  <br/> |Une valeur de type Boolean qui indique si la boîte aux lettres de l’utilisateur est accessible par le biais du protocole MAPI/HTTP.  <br/> |
   
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetUserSettings (SOAP)](getusersettings-operation-soap.md)
  
[Opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)


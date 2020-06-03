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
description: L’élément Setting représente un paramètre de configuration à renvoyer.
ms.openlocfilehash: df3b55fe7ba2c5ae92f8c31ec0643dbe100fa072
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466744"
---
# <a name="setting-soap"></a>Paramètre (SOAP)

L’élément **Setting** représente un paramètre de configuration à renvoyer. 
  
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
|UserDN  <br/> |Nom unique hérité de l’utilisateur.  <br/> |
|UserDeploymentId  <br/> |Identificateur de déploiement de l’utilisateur.  <br/> |
|InternalMailboxServer  <br/> |Nom de domaine complet (FQDN) du serveur de boîtes aux lettres.  <br/> |
|InternalRpcClientServer  <br/> |Nom de domaine complet du serveur client RPC.  <br/> |
|InternalMailboxServerDN  <br/> |Nom unique hérité du serveur de boîtes aux lettres.  <br/> |
|InternalEcpUrl  <br/> |URL interne du panneau de configuration Exchange.  <br/> |
|InternalEcpVoicemailUrl  <br/> |URL interne du panneau de configuration Exchange pour la personnalisation de la messagerie vocale.  <br/> |
|InternalEcpEmailSubscriptionsUrl  <br/> |URL interne du panneau de configuration Exchange pour les abonnements de messagerie.  <br/> |
|InternalEcpTextMessagingUrl  <br/> |URL interne du panneau de configuration Exchange pour la messagerie texte.  <br/> |
|InternalEcpDeliveryReportUrl  <br/> |URL interne du panneau de configuration Exchange pour les rapports de remise.  <br/> |
|InternalEcpRetentionPolicyTagsUrl  <br/> |URL interne du panneau de configuration Exchange pour les balises RetentionPolicy.  <br/> |
|InternalEcpPublishingUrl  <br/> |URL interne du panneau de configuration Exchange pour la publication.  <br/> |
|InternalEwsUrl  <br/> |URL interne des services Web Exchange.  <br/> |
|InternalOABUrl  <br/> |URL interne du carnet d’adresses en mode hors connexion.  <br/> |
|InternalUMUrl  <br/> |URL interne des services de messagerie unifiée.  <br/> |
|InternalWebClientUrls  <br/> |URL internes du client Web Exchange.  <br/> |
|MailboxDN  <br/> |Nom unique de la base de données de boîtes aux lettres de la boîte aux lettres de l’utilisateur.  <br/> |
|PublicFolderServer  <br/> |Nom du serveur de dossiers publics.  <br/> |
|ActiveDirectoryServer  <br/> |Nom du serveur Active Directory.  <br/> |
|ExternalMailboxServer  <br/> |Nom du serveur RPC sur HTTP.  <br/> |
|ExternalMailboxServerRequiresSSL  <br/> |Indicateur indiquant si le serveur RPC sur HTTP requiert le protocole SSL.  <br/> |
|ExternalMailboxServerAuthenticationMethods  <br/> |Les méthodes d’authentification prises en charge par le serveur RPC sur HTTP.  <br/> |
|EcpVoicemailUrlFragment,  <br/> |Le fragment d’URL du panneau de configuration Exchange pour la personnalisation de la messagerie vocale.  <br/> |
|EcpEmailSubscriptionsUrlFragment  <br/> |Le fragment d’URL du panneau de configuration Exchange pour les abonnements de messagerie.  <br/> |
|EcpTextMessagingUrlFragment  <br/> |Le fragment d’URL du panneau de configuration Exchange pour la messagerie texte.  <br/> |
|EcpDeliveryReportUrlFragment  <br/> |Le fragment d’URL du panneau de configuration Exchange pour les rapports de remise.  <br/> |
|EcpRetentionPolicyTagsUrlFragment  <br/> |Le fragment d’URL du panneau de configuration Exchange pour les balises RetentionPolicy.  <br/> |
|EcpPublishingUrlFragment  <br/> |Le fragment d’URL du panneau de configuration Exchange pour la publication.  <br/> |
|ExternalEcpUrl  <br/> |URL externe du panneau de configuration Exchange.  <br/> |
|ExternalEcpVoicemailUrl  <br/> |URL externe du panneau de configuration Exchange pour la personnalisation de la messagerie vocale.  <br/> |
|ExternalEcpEmailSubscriptionsUrl  <br/> |URL externe du panneau de configuration Exchange pour les abonnements de messagerie.  <br/> |
|ExternalEcpTextMessagingUrl  <br/> |URL externe du panneau de configuration Exchange pour la messagerie texte.  <br/> |
|ExternalEcpDeliveryReportUrl  <br/> |URL externe du panneau de configuration Exchange pour les rapports de remise.  <br/> |
|ExternalEcpRetentionPolicyTagsUrl  <br/> |URL externe du panneau de configuration Exchange pour les balises RetentionPolicy.  <br/> |
|ExternalEcpPublishingUrl  <br/> |URL externe du panneau de configuration Exchange pour la publication.  <br/> |
|ExternalEwsUrl  <br/> |URL externe des services Web Exchange.  <br/> |
|ExternalOABUrl  <br/> |URL externe du carnet d’adresses en mode hors connexion.  <br/> |
|ExternalUMUrl  <br/> |L’URL externe des services de messagerie unifiée.  <br/> |
|ExternalWebClientUrls  <br/> |URL externes du client Web Exchange.  <br/> |
|CrossOrganizationSharingEnabled  <br/> |Indique que le partage entre organisations est activé.  <br/> |
|AlternateMailboxes  <br/> |Collection de boîtes aux lettres de substitution.  <br/> |
|CasVersion  <br/> |Version du serveur d’accès au client qui traite la demande (par exemple, 14. XX. Aaaa. ZZZ  <br/> |
|EwsSupportedSchemas  <br/> |Liste de versions de schéma séparées par des virgules prises en charge par les services Web Exchange. Les valeurs de version de schéma seront identiques aux valeurs de l’énumération **ExchangeServerVersion** .  <br/> |
|InternalPop3Connections  <br/> |Liste des paramètres de connexion interne pour les connexions de protocole POP3.  <br/> |
|ExternalPop3Connections  <br/> |Liste des paramètres de connexion externe pour les connexions de protocole POP3.  <br/> |
|InternalImap4Connections  <br/> |Liste des paramètres de connexion internes pour les connexions de protocole IMAP4.  <br/> |
|ExternalImap4Connections  <br/> |Liste des paramètres de connexion externe pour les connexions de protocole IMAP4.  <br/> |
|InternalSmtpConnections  <br/> |Liste des paramètres de connexion internes pour les connexions SMTP.  <br/> |
|ExternalSmtpConnections  <br/> |Liste des paramètres de connexion externe pour les connexions SMTP.  <br/> |
|InternalServerExclusiveConnect  <br/> |Indicateur de connexion exclusive au serveur interne. Si la valeur est définie sur "OFF", les clients ne doivent pas se connecter via ce protocole.  <br/> |
|ExternalServerExclusiveConnect  <br/> |Indicateur de connexion exclusive de serveur externe. Si la valeur est définie sur « on », les clients doivent se connecter via ce protocole.  <br/> |
|ExchangeRpcUrl  <br/> |URL utilisée pour les appels de procédure distante. Cette URL est interne au serveur et ne doit pas être utilisée par les clients.  <br/> |
|ShowGalAsDefaultView  <br/> |Spécifie une valeur de type Boolean qui indique si la liste d’adresses globale doit être affichée comme carnet d’adresses. La valeur « true » indique que la liste d’adresses globale doit être affichée par défaut. La valeur « false » indique que la liste des contacts doit être affichée.  <br/> |
|AutoDiscoverSMTPAddress  <br/> |Adresse SMTP principale de découverte automatique pour l’utilisateur. Il s’agit de l’adresse proxy à la place de l’adresse de messagerie de l’utilisateur, si une adresse proxy existe.  <br/> |
|InteropExternalEwsUrl  <br/> |URL externe du point de terminaison du service Web du serveur. Il s’agit de l’URL d’un serveur qui peut servir des boîtes aux lettres hébergées sur un serveur qui ne dispose pas des services Web.  <br/> |
|ExternalEwsVersion  <br/> |Version du serveur de services Web qui fournit la requête spécifiée.  <br/> |
|InteropExternalEwsVersion  <br/> |La version du serveur InteropExternalEwsUrl pointe vers.  <br/> |
|MobileMailboxPolicyInterop  <br/> |Les paramètres de stratégie de boîte aux lettres mobile.  <br/> |
|GroupingInformation  <br/> |Valeur utilisée conjointement avec le paramètre ExternalEwsUrl pour regrouper plusieurs boîtes aux lettres afin de [préserver l’affinité](https://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx) lors de l’abonnement aux notifications.  <br/> |
|UserMSOnline  <br/> |Valeur booléenne indiquant si la boîte aux lettres de l’utilisateur est hébergée dans Exchange Online ou Exchange Online dans le cadre d’Office 365.  <br/> |
|MapiHttpEnabled  <br/> |Une valeur de type Boolean qui indique si la boîte aux lettres de l’utilisateur est accessible via le protocole MAPI/HTTP.  <br/> |
   
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetUserSettings (SOAP)](getusersettings-operation-soap.md)
  
[Opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)


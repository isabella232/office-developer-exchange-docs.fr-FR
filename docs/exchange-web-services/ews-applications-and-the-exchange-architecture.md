---
title: Applications EWS et architecture Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: c10f308a-65bb-4a0b-8fdd-b4a61503f0fd
description: Découvrez le fonctionnement d'EWS au sein de l'architecture Exchange, et les protocoles sur lesquels EWS s'appuie.
ms.openlocfilehash: 1fbc1e68edbca829555fbbf1b9f0bc4723da9524
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754785"
---
# <a name="ews-applications-and-the-exchange-architecture"></a><span data-ttu-id="24c45-103">Applications EWS et architecture Exchange</span><span class="sxs-lookup"><span data-stu-id="24c45-103">EWS applications and the Exchange architecture</span></span>

<span data-ttu-id="24c45-104">Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. Découvrez le fonctionnement d'EWS au sein de l'architecture Exchange, et les protocoles sur lesquels EWS s'appuie.</span><span class="sxs-lookup"><span data-stu-id="24c45-104">Learn about how EWS works within the Exchange architecture, and find out which protocols EWS relies on.</span></span>
  
<span data-ttu-id="24c45-p101">Exchange Web Services (EWS) est une API multiplateformes qui permet aux applications d'accéder à des éléments de boîte aux lettres tels que des messages électroniques, des réunions et des contacts à partir d'Exchange Online, Exchange Online dans le cadre d'Office 365 ou des versions locales d'Exchange à partir d'Exchange Server 2007. [Les applications EWS](ews-application-types.md) peuvent accéder aux éléments de boîte aux lettres localement ou à distance en envoyant une requête dans un message XML basé sur SOAP. Le message SOAP est incorporé dans un message HTTP lorsqu'il est envoyé entre l'application et le serveur, ce qui signifie que tant que votre application peut publier des éléments XML via HTTP, elle peut utiliser EWS pour accéder à Exchange.</span><span class="sxs-lookup"><span data-stu-id="24c45-p101">Exchange Web Services (EWS) is a cross-platform API that enables applications to access mailbox items such as email messages, meetings, and contacts from Exchange Online, Exchange Online as part of Office 365, or on-premises versions of Exchange starting with Exchange Server 2007. [EWS applications](ews-application-types.md) can access mailbox items locally or remotely by sending a request in a SOAP-based XML message. The SOAP message is embedded in an HTTP message when sent between the application and the server, which means that as long as your application can post XML through HTTP, it can use EWS to access Exchange.</span></span> 
  
## <a name="exchange-architecture-overview"></a><span data-ttu-id="24c45-108">Vue d'ensemble de l'architecture Exchange</span><span class="sxs-lookup"><span data-stu-id="24c45-108">Exchange architecture overview</span></span>
<span data-ttu-id="24c45-109"><a name="bk_techarch"> </a></span><span class="sxs-lookup"><span data-stu-id="24c45-109"></span></span>

<span data-ttu-id="24c45-p102">Les diagrammes suivants montrent les méthodes d'authentification et les chemins de communication utilisés par les applications EWS pour communiquer avec Exchange 2013 et Exchange Online. Du point de vue de l'application EWS, les chemins de communication sont identiques et les méthodes d'authentification varient légèrement. La principale différence réside dans la visibilité que vous avez du serveur principal Exchange.</span><span class="sxs-lookup"><span data-stu-id="24c45-p102">The following diagrams show the authentication methods and communication paths used by EWS applications when communicating with Exchange 2013 and Exchange Online. From the EWS application perspective, the communication paths are identical and the authentication methods only vary slightly; the main difference is the visibility you have into the Exchange backend.</span></span>
  
<span data-ttu-id="24c45-112">**Figure 1. Application EWS et architecture locale Exchange**</span><span class="sxs-lookup"><span data-stu-id="24c45-112">**Figure 1. EWS application and the Exchange on-premises architecture**</span></span>

![Illustration présentant une application EWS dans le cadre d'une architecture Exchange sur site. Pour obtenir une description des composants dans ce diagramme, voir les éléments 1 à 8 dans le texte suivant et l'image suivante.](media/Ex2013_ArchitecturesOverview.png)
  
<span data-ttu-id="24c45-115">La figure 2 illustre les mêmes chemins de communication présentés dans la figure 1, utilisés par les applications EWS pour communiquer avec Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="24c45-115">Figure 2 shows the same communication paths shown in Figure 1, as used by EWS applications when communicating with Exchange Online.</span></span>
  
<span data-ttu-id="24c45-116">**Figure 2. Application EWS et architecture Exchange Online**</span><span class="sxs-lookup"><span data-stu-id="24c45-116">**Figure 2. EWS application and the Exchange Online architecture**</span></span>

![Illustration présentant une application EWS dans le cadre d'une architecture Exchange Online pour une application EWS. Pour obtenir une description des composants dans ce diagramme, voir les éléments 1, 2, 3, 6 et 9 dans le texte suivant cette image.](media/Ex2013_Architectures_Online.png)
  
<span data-ttu-id="24c45-119">Les éléments suivants sont les composants affichés dans les diagrammes :</span><span class="sxs-lookup"><span data-stu-id="24c45-119">The following are the components that are shown in the diagrams:</span></span>
  
1. <span data-ttu-id="24c45-p105">Application EWS : il peut s'agir d'un [client, un portail ou une application de service](ews-application-types.md) et elle peut être installée sur un client ou sur un serveur d'accès au client Exchange local. Si vous utilisez l'API managée EWS pour développer l'application EWS, les assemblies de l'API managée EWS doivent être installés sur le client et [redistribués par votre application](redistribution-requirements-for-the-ews-managed-api.md).</span><span class="sxs-lookup"><span data-stu-id="24c45-p105">EWS application — This can be a [client, portal, or service application](ews-application-types.md) and it can be installed on a client or on an Exchange on-premises Client Access server. If you use the EWS Managed API to develop the EWS application, the EWS Managed API assemblies have to be installed on the client and [redistributed by your application](redistribution-requirements-for-the-ews-managed-api.md).</span></span>
    
2. <span data-ttu-id="24c45-p106">Message XML SOAP : message XML, dans une enveloppe SOAP, incorporé dans un message HTTP/S conforme au fichier Services.wsdl sur le serveur d'accès au client. HTTPS est recommandé pour Exchange en local et est obligatoire pour Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="24c45-p106">The SOAP XML message — An XML message, in a SOAP envelope, embedded in an HTTP/S message that conforms to the Services.wsdl file on the Client Access server. HTTPS is recommended for Exchange on-premises and is required for Exchange Online.</span></span> 
    
3. <span data-ttu-id="24c45-124">Méthodes d'authentification : les messages EWS comprennent des informations d'authentification de base, NTLM (authentification intégrée de Windows) ou OAuth dans le cadre de la charge utile HTTP.</span><span class="sxs-lookup"><span data-stu-id="24c45-124">Authentication methods — EWS messages include basic, NTLM (Windows Integrated authentication), or OAuth authentication information as part of the HTTP payload.</span></span> 
    
4. <span data-ttu-id="24c45-p107">Équilibreur de charge : l'équilibreur de charge distribue le message à un serveur d'accès au client dans le groupe de serveurs d'accès au client. Ce composant n'est visible que dans l'architecture Exchange locale.</span><span class="sxs-lookup"><span data-stu-id="24c45-p107">Load balancer — The load balancer distributes the message to a Client Access server in the Client Access server array. This component is only visible in the Exchange on-premises architecture.</span></span>
    
5. <span data-ttu-id="24c45-p108">Groupe de serveurs d'accès au client : les serveurs d'accès au client sont organisés en un groupe à charge équilibrée, appelé groupe de serveurs d'accès au client. Les serveurs d'accès au client individuels fournissent une authentification, une redirection limitée et des services proxy. Les serveurs d'accès au client n'effectuent aucun rendu des données et aucune donnée n'est mise en file d'attente ou stockée sur un serveur d'accès au client, car il est fin et sans état. Il authentifie simplement la demande, effectue une recherche de découverte automatique, puis transmet via un proxy la demande au serveur de boîtes aux lettres. Le serveur d'accès au client conserve une relation 1:1 avec le serveur de boîtes aux lettres qui héberge les données de l'utilisateur. Le protocole HTTP (sécurisé via SSL à l'aide d'un certificat auto-signé) est utilisé entre le serveur d'accès au client et le serveur de boîtes aux lettres. Ce composant n'est visible que dans l'architecture Exchange locale.</span><span class="sxs-lookup"><span data-stu-id="24c45-p108">Client Access server array — Client Access servers are organized into a load-balanced group called a Client Access server array. Individual Client Access servers provide authentication, limited redirection, and proxy services. The Client Access servers themselves don't do any data rendering, and no data is queued or stored on a Client Access server - it is thin and stateless; it simply authenticates the request, performs an Autodiscover lookup, and then proxies the request to the Mailbox server. The Client Access server does maintain a 1:1 relationship with the Mailbox server that hosts the user's data. The HTTP protocol (secured via SSL using a self-signed certificate) is used between the Client Access server and Mailbox server. This component is only visible in the Exchange on-premises architecture.</span></span>
    
6. <span data-ttu-id="24c45-133">Service de découverte automatique : le service de découverte automatique effectue une découverte des services en accédant aux services de domaine Active Directory (AD DS) pour récupérer la version de boîte aux lettres et l'emplacement du serveur de boîtes aux lettres qui héberge la copie active des données de l'utilisateur.</span><span class="sxs-lookup"><span data-stu-id="24c45-133">Autodiscover service — The Autodiscover service performs a service discovery by accessing Active Directory Domain Services (AD DS) to retrieve the mailbox version and the location of the Mailbox server that is hosting the active copy of the user's data.</span></span>
    
7. <span data-ttu-id="24c45-p109">Service EWS : le service EWS est décrit par trois fichiers : Services.wsdl, Messages.xsd et Types.xsd, ainsi que par les assemblies de l'API managée EWS. Services.wsdl décrit le contrat entre le client et le serveur, Messages.xsd définit les messages SOAP de requête et de réponse, et Types.xsd définit les éléments utilisés dans les messages SOAP. Messages.xsd et Types.xsd contiennent toujours les dernières versions du schéma, bien qu'il existe des versions antérieures du schéma. Notez que Services.wsdl, Messages.xsd et Types.xsd sont disponibles sur le serveur d'accès au client, mais ne sont pas utilisés pour la validation du schéma : ils sont fournis à titre de référence uniquement. Les assemblies de l'API managée EWS sont fournis pour les applications clientes EWS côté serveur et sont déployés sur tous les rôles d'Exchange Server, pas seulement les serveurs d'accès au client. Ce composant n'est visible que dans l'architecture Exchange locale.</span><span class="sxs-lookup"><span data-stu-id="24c45-p109">EWS service —The EWS service is described by three files: Services.wsdl, Messages.xsd, and Types.xsd, as well as the EWS Managed API assemblies. Services.wsdl describes the contract between the client and server, Messages.xsd defines the request and response SOAP messages, and Types.xsd defines the elements used in the SOAP messages. Messages.xsd and Types.xsd always contain the latest versions of the schema, although earlier versions of the schema exist. Note that Services.wsdl, Messages.xsd, and Types.xsd are made available on the Client Access server, but are not actually used for schema validation — they are provided for reference only. The EWS Managed API assemblies are provided for server-side EWS client applications and are deployed on all Exchange Server roles, not just the Client Access servers. This component is only visible in the Exchange on-premises architecture.</span></span>
    
    <span data-ttu-id="24c45-p110">La disponibilité des fonctionnalités est basée sur la version du schéma EWS ciblée par votre application. Étant donné que les schémas EWS sont compatibles en amont et en aval, si vous créez une application qui cible une version antérieure du schéma, comme Exchange 2007 SP1, votre application fonctionnera également sur une version ultérieure du schéma, comme le service Exchange 2010 SP2, ainsi que sur Exchange Online. Étant donné que les fonctionnalités et les mises à jour de fonctionnalité sont pilotées par le schéma, nous vous recommandons d'utiliser la base de code commun la plus récente ciblant les fonctionnalités EWS que vous souhaitez mettre en œuvre dans votre application cliente. De nombreuses applications peuvent cibler la version Exchange2007_SP1, car le schéma Exchange 2007 SP1 contient presque toutes les principales fonctionnalités Exchange pour travailler avec des éléments et des dossiers dans la banque d'informations Exchange. Pour plus d'informations, voir [Fonctionnalités clientes EWS](ews-client-design-overview-for-exchange.md#EWSFeatures).</span><span class="sxs-lookup"><span data-stu-id="24c45-p110">Feature availability is based on the EWS schema version that your application targets. Because EWS schemas are backward- and forward-compatible, if you create an application that targets an earlier schema version, such as Exchange 2007 SP1, your application will also work against a later schema version, such as the Exchange 2010 SP2 service, as well as Exchange Online. Because features and feature updates are driven by the schema, we recommend that you use the earliest common code base that targets the EWS features that you want to implement in your client application. Many applications can target the Exchange2007_SP1 version, because the Exchange 2007 SP1 schema contains almost all the core Exchange functionality for working with items and folders in the Exchange store. For more information, see [EWS client features](ews-client-design-overview-for-exchange.md#EWSFeatures).</span></span>
    
8. <span data-ttu-id="24c45-p111">Groupe de disponibilité de base de données (DAG) : les serveurs de boîtes aux lettres sont organisés en un groupe de disponibilité de base de données hautement disponible, qui peut être déployé sur un ou plusieurs centres de données. Le serveur de boîtes aux lettres contient la base de données de boîtes aux lettres et gère toutes les activités pour les boîtes aux lettres actives sur ce serveur. Tous les composants qui traitent, rendent et stockent des données sont sur le serveur de boîtes aux lettres. Les clients ne se connectent pas directement au serveur de boîtes aux lettres, toutes les connexions sont gérées par le serveur d'accès au client. Ce composant n'est visible que dans l'architecture Exchange locale.</span><span class="sxs-lookup"><span data-stu-id="24c45-p111">Database Availability Group (DAG) — Mailbox servers are organized into a highly available DAG, which can be deployed in one or more datacenters. The Mailbox server contains the mailbox database and handles all activity for the active mailboxes on that server. All components that process, render, and store data are on the Mailbox server. Clients do not connect directly to the Mailbox server; all connections are handled by the Client Access server. This component is only visible in the Exchange on-premises architecture.</span></span>
    
9. <span data-ttu-id="24c45-150">Exchange Online et Exchange Online dans le cadre d'Office 365 : solution de messagerie hébergée qui fournit des fonctionnalités Exchange comme un service basé sur un nuage.</span><span class="sxs-lookup"><span data-stu-id="24c45-150">Exchange Online and Exchange Online as part of Office 365 — The hosted messaging solution that delivers Exchange features as a cloud-based service.</span></span>
    
<span data-ttu-id="24c45-p112">Lorsqu'une application EWS demande des informations à la banque d'informations Exchange, un message de requête XML conforme à la norme SOAP est créé et envoyé au serveur Exchange. Lorsque le serveur Exchange reçoit la requête, il vérifie les informations d'identification fournies par le client et analyse automatiquement les données XML pour trouver les données demandées. Le serveur crée alors une réponse SOAP contenant les données XML qui représentent les objets fortement typés demandés et leurs propriétés. Les données XML sont renvoyées à l'application dans une réponse HTTP. L'application désérialise ensuite les données XML et les utilise pour reformer les objets fortement typés.</span><span class="sxs-lookup"><span data-stu-id="24c45-p112">When an EWS application requests information from the Exchange store, an XML request message that complies with the SOAP standard is created and sent to the Exchange server. When the Exchange server receives the request, it verifies the credentials that are provided by the client and automatically parses the XML for the requested data. The server then builds a SOAP response that contains XML data that represents the requested strongly typed objects and their properties. The XML data is sent back to the application in an HTTP response. The application then deserializes the XML and uses the data to reform the strongly typed objects.</span></span>
  
## <a name="protocols-and-standards-that-ews-applications-must-support"></a><span data-ttu-id="24c45-156">Protocoles et normes que les applications EWS doivent prendre en charge</span><span class="sxs-lookup"><span data-stu-id="24c45-156">Protocols and standards that EWS applications must support</span></span>
<span data-ttu-id="24c45-157"><a name="bk_standards"> </a></span><span class="sxs-lookup"><span data-stu-id="24c45-157"></span></span>

<span data-ttu-id="24c45-158">Pour communiquer avec un serveur Exchange, les applications EWS doivent prendre en charge les protocoles et normes suivants.</span><span class="sxs-lookup"><span data-stu-id="24c45-158">To communicate with an Exchange server, EWS applications must support the following protocols and standards.</span></span>
  
<span data-ttu-id="24c45-159">**Tableau 1. Protocoles**</span><span class="sxs-lookup"><span data-stu-id="24c45-159">**Table 1. Protocols**</span></span>

|<span data-ttu-id="24c45-160">**Protocole**</span><span class="sxs-lookup"><span data-stu-id="24c45-160">**Protocol**</span></span>|<span data-ttu-id="24c45-161">**Utilisation**</span><span class="sxs-lookup"><span data-stu-id="24c45-161">**How it's used**</span></span>|
|:-----|:-----|
|<span data-ttu-id="24c45-162">HTTP/S</span><span class="sxs-lookup"><span data-stu-id="24c45-162">HTTP/S</span></span>  <br/> |<span data-ttu-id="24c45-163">Permet aux applications EWS d'accéder aux données de base de données Exchange sur le réseau, que le client se trouve sur Internet ou l'intranet.</span><span class="sxs-lookup"><span data-stu-id="24c45-163">Enables EWS applications to access Exchange database data over the network, regardless of whether the client is on the Internet or intranet.</span></span>  <br/> |
|<span data-ttu-id="24c45-164">SOAP 1.0</span><span class="sxs-lookup"><span data-stu-id="24c45-164">SOAP 1.0</span></span>  <br/> |<span data-ttu-id="24c45-p113">Permet de former une enveloppe autour de la charge de messagerie. EWS implémente le protocole SOAP à l'aide de différentes parties de l'enveloppe SOAP pour activer plusieurs fonctionnalités. L'en-tête SOAP est utilisé pour l'emprunt d'identité et pour fournir des données de contrôle des versions. Le corps SOAP fournit des informations sur l'opération à exécuter et les données soumises à l'opération. SOAP s'appuie sur WSDL pour décrire les opérations à appeler.</span><span class="sxs-lookup"><span data-stu-id="24c45-p113">Forms an envelope around the messaging payload. EWS implements the SOAP protocol by using different parts of the SOAP envelope to enable different functionality. The SOAP header is used for impersonation and to provide versioning data. The SOAP body provides information about the operation to run and the data that is submitted to the operation. SOAP relies on WSDL to describe the operations to call.</span></span>  <br/> |
|<span data-ttu-id="24c45-170">WSDL 1.0</span><span class="sxs-lookup"><span data-stu-id="24c45-170">WSDL 1.0</span></span>  <br/> |<span data-ttu-id="24c45-p114">Décrit les liaisons, les opérations et les propriétés utilisées pour appeler les opérations EWS, dans le fichier Services.wsdl. Ce fichier, ainsi que les fichiers de schéma référencés, comprennent le contrat entre une application EWS et le serveur Exchange, et sont souvent utilisés avec les outils propres au fournisseur pour créer des applications propres à la plateforme. Le fichier WSDL se trouve dans le répertoire virtuel EWS, qui se trouve à la racine du site web.</span><span class="sxs-lookup"><span data-stu-id="24c45-p114">Describes the bindings, the operations, and the properties that are used to call EWS operations, in the Services.wsdl file. This file, along with the referenced schema files, comprises the contract between an EWS application and the Exchange server, and is often used along with vendor-specific tools to create platform-specific applications. The WSDL file is located in the EWS virtual directory, which is at the root of the website.</span></span>  <br/> |
|<span data-ttu-id="24c45-174">Transport Layer Security (TLS)/SSL</span><span class="sxs-lookup"><span data-stu-id="24c45-174">Transport Layer Security (TLS)/SSL</span></span>  <br/> |<span data-ttu-id="24c45-p115">Fournit des communications web sécurisées sur Internet ou l'intranet. TLS permet aux applications d'authentifier les serveurs ou, éventuellement, permet aux serveurs d'authentifier les applications EWS. Il fournit également un canal de sécurité en chiffrant les communications. TLS est la version la plus récente du protocole Secure Sockets Layer (SSL).</span><span class="sxs-lookup"><span data-stu-id="24c45-p115">Provides secure web communications on the Internet or on intranet. TLS enables applications to authenticate servers or, optionally, servers to authenticate EWS applications. It also provides a security channel by encrypting communications. TLS is the latest version of the Secure Sockets Layer (SSL) protocol.</span></span>  <br/> |
|<span data-ttu-id="24c45-179">XML/XSD</span><span class="sxs-lookup"><span data-stu-id="24c45-179">XML/XSD</span></span>  <br/> |<span data-ttu-id="24c45-p116">Fournit un format de message universel pour l'échange d'informations entre le client et le serveur Exchange. XML fournit des données de base de données Exchange complexes aux applications clientes, mais dans une structure définie. L'avantage du XML réside dans le fait qu'il permet l'échange de données, même lorsqu'une application EWS et un serveur ne partagent pas de plateforme commune.</span><span class="sxs-lookup"><span data-stu-id="24c45-p116">Provides a universal message format for the exchange of information between the Exchange server and the client. XML provides complex Exchange database data to client applications, but in a defined structure. The beauty of XML is that it allows for the exchange of data even when an EWS application and server do not share a common platform.</span></span>  <br/> |
   
<span data-ttu-id="24c45-183">En outre, les applications EWS doivent prendre en charge les normes d'authentification suivantes :</span><span class="sxs-lookup"><span data-stu-id="24c45-183">In addition, EWS applications must support the following authentication standards:</span></span>
  
- <span data-ttu-id="24c45-184">Authentification de base sur SSL, pour les applications qui ciblent Exchange Online ou Exchange local.</span><span class="sxs-lookup"><span data-stu-id="24c45-184">Basic authentication over SSL, for applications that target Exchange Online or Exchange on-premises.</span></span>
    
- <span data-ttu-id="24c45-185">Authentification NTLM sur SSL, pour les applications qui prennent en charge Exchange local.</span><span class="sxs-lookup"><span data-stu-id="24c45-185">NTLM authentication over SSL, for applications that support Exchange on-premises.</span></span>
    
- <span data-ttu-id="24c45-186">Authentification de jeton OAuth 2.0, pour les applications partenaires approuvées et l'interopérabilité avec Lync Server 2013 et SharePoint Server 2013.</span><span class="sxs-lookup"><span data-stu-id="24c45-186">OAuth 2.0 token authentication, for trusted partner applications and interoperability with Lync Server 2013 and SharePoint Server 2013.</span></span>
    
## <a name="see-also"></a><span data-ttu-id="24c45-187">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="24c45-187">See also</span></span>


- [<span data-ttu-id="24c45-188">Commencer à utiliser les services web dans Exchange</span><span class="sxs-lookup"><span data-stu-id="24c45-188">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)
    
- [<span data-ttu-id="24c45-189">Types d'applications EWS</span><span class="sxs-lookup"><span data-stu-id="24c45-189">EWS application types</span></span>](ews-application-types.md)
    
- [<span data-ttu-id="24c45-190">Vue d'ensemble de la conception client EWS pour Exchange</span><span class="sxs-lookup"><span data-stu-id="24c45-190">EWS client design overview for Exchange</span></span>](ews-client-design-overview-for-exchange.md)
    

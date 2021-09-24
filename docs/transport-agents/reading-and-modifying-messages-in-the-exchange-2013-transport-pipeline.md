---
title: Lecture et modification de messages dans le pipeline de transport Exchange 2013
manager: sethgros
ms.date: 09/17/2021
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: b53ed47a-3d01-4c4e-ad32-fb0532872aad
description: Découvrez les classes .NET Framework que vous pouvez utiliser dans vos agents de transport Exchange 2013 pour lire, écrire et modifier des messages.
ms.openlocfilehash: 5bf4406f7ca82512bb55388e0865e0d343cae66e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59537235"
---
# <a name="reading-and-modifying-messages-in-the-exchange-2013-transport-pipeline"></a>Lecture et modification de messages dans le pipeline de transport Exchange 2013

Découvrez les classes .NET Framework que vous pouvez utiliser dans vos agents de transport Exchange 2013 pour lire, écrire et modifier des messages.
  
**S’applique à :** Exchange Server 2013
  
- Classes utilisées pour lire, écrire ou modifier des messages
- Espace de noms Encoders
- Espace de noms iCalendar
- Espace de noms MIME
- Espace de noms TextConverters
- Espace de noms Tnef
- Espace de noms vCard
  
À mesure que les messages passent par le pipeline de transport, votre agent de transport peut lire, écrire et convertir le contenu des messages entre différents formats de données. Par exemple, vous pouvez lire et écrire des données MIME, identifier les messages entrants au format Uuencoded ou Quoted-printable (qp), puis les convertir en une norme utilisée par votre organisation, ou lire et enregistrer les informations de calendrier ou de contact associées aux messages entrants. 
  
Vous pouvez également identifier le contenu qui représente une menace pour la sécurité et déplacer ou supprimer le contenu ou les messages qui le contiennent . par exemple, en supprimant des liens dans un message HTML.
  
Cet article fournit des informations sur .NET Framework classes que vous pouvez utiliser pour lire, écrire et modifier des messages.
  
> [!CAUTION]
> La plupart des propriétés et des paramètres des API de conversion de contenu autorisent des valeurs suffisamment grandes pour entraîner des problèmes de performances, y compris le refus de service. Lorsque vous utilisez les API de conversion de contenu dans un agent de transport, vous devez implémenter des limites sur les tailles de propriétés et de valeurs de paramètres que vous prendrez en charge lors de la lecture ou de l’écriture afin de limiter la consommation de ressources par votre agent. 

<a name="Namespaces"> </a>

## <a name="classes-used-to-read-write-or-modify-messages"></a>Classes utilisées pour lire, écrire ou modifier des messages

Le tableau suivant répertorie .NET Framework classes que vous pouvez utiliser pour lire, écrire et modifier des messages électroniques.
  
**.NET Framework de noms de traitement des messages**

|**.NET Framework de noms**|**Classes**|
|:-----|:-----|
|[Microsoft. Exchange. Data.Mime.Encoders](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.aspx) <br/> |Contient des classes pour le codage et le décodage en mémoire, une classe de flux encodeur qui accepte l’une des classes d’encodeur ou de décodeur contenues dans une éumération associée, ainsi que la classe de base [ByteEncoder](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.ByteEncoder.aspx) et la classe [d’exception ByteEncoderException](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.ByteEncoderException.aspx) pour les encodeurs et décodeurs.  <br/> |
|[Microsoft. Exchange. Data.ContentTypes.iCalendar](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.aspx) <br/> |Contient des types qui vous permettent de lire et d’écrire des flux de données qui contiennent des informations de calendrier. Inclut un lecteur de calendrier et un rédacteur, un objet d’exception, un objet de récurrence, ainsi que des structures et des éumérations qui vous aident à renvoyer des informations de propriété sur les éléments de calendrier.  <br/> |
|[Microsoft. Exchange. Data.Mime](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.aspx) <br/> |Contient des classes, des structures, des éumérations et des délégués que vous pouvez utiliser pour créer, lire, écrire, parcourir, coder et décoder des données MIME. Inclut un lecteur et un rédacteur basés sur un flux qui vous donne un accès en lecture et en écriture en lecture et en écriture avant uniquement aux flux de données MIME, ainsi que des méthodes et des classes DOM que vous pouvez utiliser sur les documents MIME.  <br/> |
|[Microsoft. Exchange. Data.TextConverters](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.aspx) <br/> |Contient des classes, des structures, des éumérations et des délégués qui vous permettent de lire et d’écrire un flux de données et d’effectuer des conversions entre des types de données spécifiques ; par exemple, html au format RTF (Rich Text Format). Les convertisseurs de texte vous permettent de modifier le format d’un flux de document d’un formulaire à un autre et de supprimer de manière sélective les éléments d’un document qui peuvent poser un risque de sécurité.  <br/> |
|[Microsoft. Exchange. Data.ContentTypes.Tnef](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.aspx) <br/> |Contient un lecteur et un rédacteur de flux avant uniquement, une classe d’exception, ainsi que des structures et des éumérations qui facilitent la lecture et l’écriture de données TNEF (Transport Neutral Encapsulation Format).  <br/> |
|[Microsoft. Exchange. Data.ContentTypes.vCard](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.vCard.aspx) <br/> |Contient un lecteur et un rédacteur de flux avant uniquement, une classe d’exception, ainsi que des structures et des éumérations qui facilitent la lecture et l’écriture de données de contact au format vCard.  <br/> |
   
## <a name="encoders-namespace"></a>Espace de noms Encoders
<a name="Encoders"> </a>

L’espace de noms Encoders contient des classes pour le codage et le décodage en mémoire. Ceux-ci héritent de la classe de base [ByteEncoder.](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.ByteEncoder.aspx) Classes encodent et décodent pour base64, BinHex, Quoted-printable (qp) et Unix-to-Unix (Uu). Les classes suivantes sont utilisées pour le codage et le décodage en mémoire : 
  
- [Base64Encoder](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.Base64Encoder.aspx)
    
- [Base64Decoder](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.Base64Decoder.aspx)
    
- [BinHexEncoder](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.BinHexEncoder.aspx)
    
- [BinHexDecoder](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.BinHexDecoder.aspx)
    
- [QPEncoder](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.QPEncoder.aspx)
    
- [QPDecoder](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.QPDecoder.aspx)
    
- [UUEncoder](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.UUEncoder.aspx)
    
- [UUDecoder](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.UUDecoder.aspx)
    
Les encodeurs et décodeurs héritent de la classe de base [ByteEncoder](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.ByteEncoder.aspx) et utilisent la classe [d’exception ByteEncoderException](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.ByteEncoderException.aspx) pour la gestion des erreurs. 
  
En outre, l’espace de noms contient la classe [MacBinaryHeader,](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.MacBinaryHeader.aspx) qui identifie les fichiers codés MacBinary et lit leur en-tête de fichier associé. 
  
Enfin, la [classe EncoderStream](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.EncoderStream.aspx) effectue une conversion sur un flux de données au lieu d’un objet en mémoire. Cette classe accepte l’une des classes d’encodeur ou de décodeur et lit ou écrit en fonction de l’éumération [EncoderStreamAccess](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.EncoderStreamAccess.aspx) associée. 
  
## <a name="icalendar-namespace"></a>Espace de noms iCalendar
<a name="iCalendar"> </a>

L’espace de noms iCalendar fournit un lecteur et un rédacteur avant uniquement pour les données iCalendar, en plus de la prise en charge des structures et des classes pour la création, l’accès et la modification de flux iCalendar.
  
Les classes [CalendarReader](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.CalendarReader.aspx) et [CalendarWriter](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.CalendarWriter.aspx) sont utilisées pour lire et écrire des données de flux iCalendar. 
  
CalendarReader prend un flux [lisible](https://msdn.microsoft.com/library/System.IO.Stream.aspx) comme argument pour ses constructeurs. Vous pouvez ensuite utiliser les méthodes [ReadFirstChildComponent,](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.CalendarReader.ReadFirstChildComponent.aspx) [ReadNextSiblingComponent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.CalendarReader.ReadNextSiblingComponent.aspx)et [ReadNextComponent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.CalendarReader.ReadNextComponent.aspx) pour accéder de manière séquentielle aux composants iCalendar dans le flux de données. En fonction de la valeur que vous avez définie pour la propriété [ComplianceMode,](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.CalendarReader.ComplianceMode.aspx) les erreurs dans le flux iCalendar entraînent la création d’une exception ou la propriété [ComplianceStatus](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.CalendarReader.ComplianceStatus.aspx) est définie sur une valeur autre que [Compliant](https://msdn.microsoft.com/library/microsoft.exchange.data.contenttypes.icalendar.calendarcompliancestatus.aspx). Vous pouvez vérifier cette propriété pour découvrir les problèmes avec les données iCalendar entrantes. 
  
La [classe CalendarWriter](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.CalendarWriter.aspx) prend un [flux](https://msdn.microsoft.com/library/System.IO.Stream.aspx) accessible en ligne comme argument pour ses constructeurs. 
  
## <a name="mime-namespace"></a>Espace de noms MIME
<a name="MIME"> </a>

L’espace de noms MIME fournit des classes qui vous permettent de créer, d’accéder et de modifier des documents MIME. Vous pouvez utiliser des documents MIME à l’aide d’une méthode basée sur un flux ou doM.
  
### <a name="mimedocument-class-and-the-mime-dom"></a>Classe MimeDocument et DOM MIME

La [classe MimeDocument](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeDocument.aspx) permet à DOM d’accéder à un document MIME. Utilisez des objets de ce type lorsque vous disposez de la mémoire disponible pour charger un DOM entier et que vous devez avoir un accès aléatoire aux en-têtes et au contenu du message. 
  
Vous chargez des données dans [un objet MimeDocument](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeDocument.aspx) à l’aide des méthodes [GetLoadStream](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeDocument.GetLoadStream.aspx) ou [Load.](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeDocument.Load.aspx) Vous pouvez ensuite parcourir la hiérarchie DOM et créer, modifier ou supprimer des données MIME. Après avoir modifié les données MIME, vous pouvez les écrire dans un flux à l’aide de l’une des méthodes [WriteTo.](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeNode.WriteTo.aspx) 
  
La figure suivante illustre la structure des données dans un [objet MimeDocument.](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeDocument.aspx) 
  
**Figure 1. Structure des objets MimeDocument**

![Architecture DOM MIME](media/MimeDomArchitecture.gif)
  
### <a name="mimereader-and-mimewriter-classes-and-stream-based-mime-parsing"></a>Classes MimeReader et MimeWriter et l’doncur MIME basé sur un flux

Les classes [MimeReader](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeReader.aspx) et [MimeWriter](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeWriter.aspx) permettent un accès avant uniquement aux flux MIME. Utilisez ces classes lorsque vous n’avez pas besoin de modifier les données MIME qui nécessitent des données qui ont déjà été lues ou écrites. Par exemple, si vous souhaitez imprimer des messages qui correspondent à un format prédéféré, la classe [MimeWriter](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeWriter.aspx) peut être idéale. 
  
La [classe MimeDocument](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeDocument.aspx) encapsule un DOM. Les classes [MimeReader](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeReader.aspx) et [MimeWriter représentent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeWriter.aspx) des ordinateurs d’état. Leurs états changent en fonction de l’entrée reçue et des méthodes appelées. Les figures 2 à 5 sont des diagrammes de transition d’état simplifiés qui indiquent, pour l’objet [MimeReader,](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeReader.aspx) quelles méthodes sont valides pour appeler à partir de chaque état et l’état qui en résulte. 
  
Pour utiliser ces diagrammes, suivez les flèches d’un état à l’autre, en notant les appels de méthode ou les valeurs de retour qui entraînent le changement d’état. Par exemple, dans le premier diagramme, supposons que vous êtes au début du flux qui appartient à MimeReader que vous avez créé. Pour obtenir l’état Des en-têtes de partie, appelez l’un des membres [ReadNextPart](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeReader.ReadNextPart.aspx) ou [ReadFirstChildPart,](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeReader.ReadFirstChildPart.aspx)dans cet ordre. S’il existe des en-têtes (c’est-à-dire, si l’élément MIME est bien formé), vous entrez dans l’état En-têtes de partie. Dans le cas contraire, une exception sera lancée. 
  
**Figure 2. Diagramme de transition d’état simplifié pour les objets MimeReader**

![Diagramme d’état MimeReader](media/MimeReader_StateDiagram_01.gif)
  
> [!NOTE]
> Les figures 3, 4 et 5 s' expandent sur les états affichés dans chacun des diagrammes précédents. 
  
**Figure 3. Développement de l’état des en-têtes de partie à partir de la figure 2**

![Développement de l’état « En-têtes de composant ».](media/MimeReader_StateDiagram_02.gif)
  
**Figure 4. Développement de l’état d’en-tête à partir de la figure 3 lorsqu’un paramètre a été rencontré dans un en-tête**

![Développement de l’état « En-têtes de partie » lorsqu’un paramètre a été rencontré dans un en-tête](media/MimeReader_StateDiagram_03.gif)
  
> [!NOTE]
> L’état représenté par la figure 5 est récursif en ce que, si un groupe d’adresses est rencontré, vous pouvez utiliser la propriété [GroupRecipientReader](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeAddressReader.GroupRecipientReader.aspx) pour lire les adresses du groupe. 
  
**Figure 5. Développement de l’état d’en-tête à partir de la figure 3 lorsqu’une adresse ou un groupe d’adresses est rencontré**

![Développement de l’état « En-tête » pour l’adresse ou le groupe](media/MimeReader_StateDiagram_04.gif)
  
Les figures 6 et 7 illustrent des diagrammes de transition d’état simplifiés pour [l’objet MimeWriter.](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeWriter.aspx) 
  
> [!NOTE]
> La figure 7 se développe sur l’état Des en-têtes de partie illustré dans la figure 6. 
  
**Figure 6. Diagramme de transition d’état simplifié pour les objets MimeWriter**

![Diagramme de transition d’état pour MimeWriter](media/MimeWriter_TopLevel.gif)
  
**Figure 7. Développement de l’état des en-têtes de partie à partir de la figure 6**

![Développement du diagramme de transition d’état pour MimeWriter](media/MimeWriter_Diagram_Expansion.gif)
  
## <a name="textconverters-namespace"></a>Espace de noms TextConverters
<a name="TextConverters"> </a>

L’espace de noms TextConverters contient des types qui prisent en charge la conversion du contenu des messages électroniques. Ces types peuvent effectuer une conversion de page de code, supprimer du code HTML qui n’est pas sécurisé et effectuer d’autres transformations sur les corps des messages électroniques. [Microsoft.Exchange. L’espace de noms Data.TextConverters](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.aspx) inclut les classes suivantes qui dérivent de la classe abstraite [TextConverter](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.TextConverter.aspx) : 
  
- [EnrichedToHtml](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.EnrichedToHtml.aspx)
    
- [EnrichedToText](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.EnrichedToText.aspx)
    
- [HtmlToEnriched](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.HtmlToEnriched.aspx)
    
- [HtmlToHtml](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.HtmlToHtml.aspx)
    
- [HtmlToRtf](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.HtmlToRtf.aspx)
    
- [HtmlToText](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.HtmlToText.aspx)
    
- [RtfCompressedToRtf](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.RtfCompressedToRtf.aspx)
    
- [RtfToHtml](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.RtfToHtml.aspx)
    
- [RtfToRtf](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.RtfToRtf.aspx)
    
- [RtfToRtfCompressed](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.RtfToRtfCompressed.aspx)
    
- [RtfToText](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.RtfToText.aspx)
    
- [TextToHtml](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.TextToHtml.aspx)
    
- [TextToRtf](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.TextToRtf.aspx)
    
- [TextToText](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.TextToText.aspx)
    
Ces convertisseurs de texte vous permettent de modifier le format d’un flux de document ou de supprimer des éléments qui ne sont pas sécurisés d’un document HTML. Ces classes peuvent être utilisées par elles-mêmes pour effectuer une conversion à l’aide d’un seul appel à l’une des méthodes Convert de la classe de base [TextConverter,](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.TextConverter.aspx) ou elles peuvent être transmises à un constructeur du convertisseur, qui l’utilise pour effectuer des lectures ou des écritures converties. 
  
La fonctionnalité héritée de la classe de base est utile pour effectuer des conversions lorsque vous avez suffisamment d’espace pour stocker le document d’origine et sa sortie convertie, ou lorsque vous souhaitez stocker les résultats de la conversion. La **méthode Convert** prend les flux d’entrée et de sortie, les lecteurs de texte ou les rédacteurs de texte, et convertit le contenu de l’entrée vers la sortie associée. 
  
Les classes de lecture de texte, d’auteur et de flux suivantes sont également incluses dans l’espace de noms :
  
- [ConverterReader](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.ConverterReader.aspx) — Dérivé de **System.IO.TextReader**. 
    
- [ConverterWriter](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.ConverterWriter.aspx) — Dérivé de **System.IO.TextWriter**. 
    
- [ConverterStream](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.ConverterStream.aspx) — Dérivé de **System.IO.Stream**. 
    
Ces conversions sont utilisées pour effectuer des conversions lorsque vous n’avez pas de place pour stocker l’original ou sa sortie convertie, lorsque vous recevez l’entrée ou envoyez la sortie vers un flux, ou lorsque vous souhaitez que la sortie soit uniquement à des fins d’indexation ou de recherche et que, par conséquent, vous ne voulez pas stocker le résultat d’une conversion.
  
## <a name="tnef-namespace"></a>Espace de noms Tnef
<a name="TNEF"> </a>

L’espace de noms Tnef contient des classes et des types qui permettent la lecture et l’écriture de données TNEF en continu uniquement. Le format TNEF est un format de données utilisé pour encapsuler les propriétés MAPI pour les clients qui ne peuvent pas interpréter MAPI.
  
Les classes [TnefReader](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.TnefReader.aspx) et [TnefWriter](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.TnefWriter.aspx) fournissent les fonctionnalités de base dans [Microsoft.Exchange. Espace de noms Data.ContentTypes.Tnef.](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.aspx) 
  
La [classe TnefReader prend](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.TnefReader.aspx) un flux lisible comme argument pour ses constructeurs. Vous utilisez ensuite la [méthode ReadNextAttribute](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.TnefReader.ReadNextAttribute.aspx) pour lire séquentiellement les attributs dans le flux TNEF. Une fois que vous avez lu un attribut, vous pouvez accéder à des informations sur l’attribut à l’aide de l’une des propriétés en lecture seule sur l’objet [TnefReader,](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.TnefReader.aspx) en plus d’obtenir un [TnefPropertyReader](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.TnefPropertyReader.aspx) pour lire la propriété actuelle. Vous pouvez également accéder directement à l’attribut actuel à l’aide de la [méthode ReadAttributeRawValue.](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.TnefReader.ReadAttributeRawValue.aspx) 
  
La [classe TnefWriter](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.TnefWriter.aspx) prend un [stream](https://msdn.microsoft.com/library/System.IO.Stream.aspx) accessible en ligne comme argument pour ses constructeurs. La [classe TnefWriter fournit](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.TnefWriter.aspx) plusieurs façons d’écrire des données dans ce flux. 
  
## <a name="vcard-namespace"></a>Espace de noms vCard
<a name="vCard"> </a>

L’espace de noms vCard contient des classes, des structures et des listes utilisées pour lire et écrire les informations de contact contenues dans un message électronique au format de données vCard. L’espace de noms contient un lecteur de contacts et un rédacteur, une classe d’exception, un lecteur de propriétés, un lecteur de paramètres et des listes de prise en charge qui vous permettent de lire les données vCard associées à un message électronique.
  
## <a name="see-also"></a>Voir aussi

- [Agents de transport dans Exchange](transport-agents-in-exchange-2013.md)  
- [Concepts sur les agents de transport dans Exchange 2013](transport-agent-concepts-in-exchange-2013.md) 
- [Référence de l’agent de transport Exchange 2013](transport-agent-reference-for-exchange-2013.md)
- [Types de médias MIME](http://www.iana.org/assignments/media-types)
    


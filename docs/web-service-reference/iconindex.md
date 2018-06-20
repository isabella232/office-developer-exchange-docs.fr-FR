---
title: IconIndex
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 92020822-2a86-4dfc-aee1-3067af4d4edf
description: L’élément IconIndex identifie l’index de l’icône d’un élément ou d’une conversation.
ms.openlocfilehash: 8ada9da2df1cf128009c9b153736b434925f1a3f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19827848"
---
# <a name="iconindex"></a>IconIndex

L’élément **IconIndex** identifie l’index de l’icône d’un élément ou d’une conversation. 
  
```XML
<IconIndex>Default | PostItem | MailRead | MailUnread | MailReplied | MailForwarded | MailEncrypted | MailSmimeSigned | MailEncrytedReplied | MailSmimeSignedReplied | MailEncryptedForwarded | MailSmimeSignedForwarded | MailEncryptedRead | MailSmimeSignedRead | MailIrm | MailIrmForwarded | MailIrmReplied | SmsSubmitted | SmsRoutedToDeliveryPoint | SmsRoutedToExternalMessagingSystem | SmsDelivered | OutlookDefaultForContacts | AppointmentItem | AppointmentRecur | AppointmentMeet | AppointmentMeetRecur | AppointmentMeetNY | AppointmentMeetYes | AppointmentMeetNo | AppointmentMeetMaybe | AppointmentMeetCancel | AppointmentMeetInfo | TaskItem | TaskRecur | TaskOwned | TaskDelegated</IconIndex>
```

 **IconIndexType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[Conversation (ConversationType)](conversation-conversationtype.md) | [élément](item.md) | [Contact](contact.md) | [DistributionList](distributionlist.md) | [Message](message-ex15websvcsotherref.md) | [CalendarItem](calendaritem.md) | [PostItem](postitem.md) | [tâche ](task.md)
  
## <a name="text-value"></a>Valeur de texte

Le tableau suivant contient les valeurs de texte possibles pour l’élément **IconIndex** . 
  
|**Valeur**|**Description**|
|:-----|:-----|
|||
|Default (Défaut)  <br/> |Spécifie l’icône par défaut.  <br/> |
|Objet postItem  <br/> |Spécifie l’icône pour un élément de publication.  <br/> |
|MailRead  <br/> |Spécifie que le message lu icône.  <br/> |
|MailUnread  <br/> |Spécifie l’icône Courrier non lu.  <br/> |
|MailReplied  <br/> |Spécifie la réponse à l’icône Courrier.  <br/> |
|MailForwarded  <br/> |Spécifie l’icône Courrier transféré.  <br/> |
|MailEncrypted  <br/> |Spécifie l’icône message chiffré.  <br/> |
|MailSmimeSigned  <br/> |Spécifie l’icône de messages électroniques signés Secure/Multipurpose Internet Mail Extensions (S/MIME).  <br/> |
|MailEncryptedReplied  <br/> |Spécifie qu'une réponse chiffrés à l’icône Courrier.  <br/> |
|MailSmimeSignedReplied  <br/> |Spécifie que le S/MIME signés répondu à l’icône Courrier.  <br/> |
|MailEncryptedForwarded  <br/> |Spécifie l’icône Courrier transféré chiffré.  <br/> |
|MailSmimeSignedForwarded  <br/> |Spécifie le S/MIME signé transféré icône Courrier.  <br/> |
|MailEncryptedRead  <br/> |Spécifie l’icône message lecture chiffré.  <br/> |
|MailSmimeSignedRead  <br/> |Spécifie le S/MIME signé lire l’icône Courrier.  <br/> |
|MailIrm  <br/> |Spécifie l’icône Courrier protégés par IRM Information Rights Management.  <br/> |
|MailIrmForwarded  <br/> |Spécifie le-protégé par IRM transféré icône Courrier.  <br/> |
|MailIrmReplied  <br/> |Spécifie que le-protégé par IRM a répondu à l’icône Courrier.  <br/> |
|SmsSubmitted  <br/> |Spécifie la messagerie icône envoyée pour le routage du Service SMS (Short Message).  <br/> |
|SmsRoutedToDeliveryPoint  <br/> |Spécifie l’icône pour le routage de SMS vers un point de remise externe.  <br/> |
|SmsRoutedToExternalMessagingSystem  <br/> |Spécifie l’icône pour le routage de SMS vers un système de messagerie externe.  <br/> |
|SmsDelivered  <br/> |Spécifie l’icône de courrier remis SMS.  <br/> |
|OutlookDefaultForContacts  <br/> |Spécifie l’icône par défaut pour les contacts.  <br/> |
|Objet AppointmentItem  <br/> |Spécifie l’icône de l’élément de rendez-vous.  <br/> |
|AppointmentRecur  <br/> |Spécifie l’icône de rendez-vous périodiques.  <br/> |
|AppointmentMeet  <br/> |Spécifie l’icône de réunion.  <br/> |
|AppointmentMeetRecur  <br/> |Spécifie l’icône réunion périodique.  <br/> |
|AppointmentMeetNY  <br/> |Spécifie l’icône d’une réponse provisoire à la réunion.  <br/> |
|AppointmentMeetYes  <br/> |Spécifie la réunion icône acceptation.  <br/> |
|AppointmentMeetNo  <br/> |Spécifie l’icône de réunion refusée.  <br/> |
|AppointmentMeetMaybe  <br/> |Spécifie l’icône d’une réponse peut-être à la réunion.  <br/> |
|AppointmentMeetCancel  <br/> |Spécifie la réunion annuler l’icône.  <br/> |
|AppointmentMeetInfo  <br/> |Spécifie la réunion icône d’information.  <br/> |
|Objet TaskItem  <br/> |Spécifie l’icône de l’élément de tâche.  <br/> |
|TaskRecur  <br/> |Spécifie l’icône de la tâche périodique.  <br/> |
|TaskOwned  <br/> |Spécifie la tâche propriétée d’icône.  <br/> |
|TaskDelegated  <br/> |Spécifie l’icône déléguées à ces tâches.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |false  <br/> |
   


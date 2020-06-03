---
title: IconIndex
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 92020822-2a86-4dfc-aee1-3067af4d4edf
description: L’élément IndexIcône identifie l’index d’icône d’un élément ou d’une conversation.
ms.openlocfilehash: 0f932f5632422a8786e74500bf83cb1337f780c3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460784"
---
# <a name="iconindex"></a>IconIndex

L’élément **IndexIcône** identifie l’index d’icône d’un élément ou d’une conversation. 
  
```XML
<IconIndex>Default | PostItem | MailRead | MailUnread | MailReplied | MailForwarded | MailEncrypted | MailSmimeSigned | MailEncrytedReplied | MailSmimeSignedReplied | MailEncryptedForwarded | MailSmimeSignedForwarded | MailEncryptedRead | MailSmimeSignedRead | MailIrm | MailIrmForwarded | MailIrmReplied | SmsSubmitted | SmsRoutedToDeliveryPoint | SmsRoutedToExternalMessagingSystem | SmsDelivered | OutlookDefaultForContacts | AppointmentItem | AppointmentRecur | AppointmentMeet | AppointmentMeetRecur | AppointmentMeetNY | AppointmentMeetYes | AppointmentMeetNo | AppointmentMeetMaybe | AppointmentMeetCancel | AppointmentMeetInfo | TaskItem | TaskRecur | TaskOwned | TaskDelegated</IconIndex>
```

 **IconIndexType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[Conversation (ConversationType)](conversation-conversationtype.md)  |  [Élément](item.md)  |  [Contact](contact.md)  |  [DistributionList](distributionlist.md)  |  [Message](message-ex15websvcsotherref.md)  |  [CalendarItem](calendaritem.md)  |  [PostItem](postitem.md)  |  [Tâche](task.md)
  
## <a name="text-value"></a>Valeur texte

Le tableau suivant contient les valeurs de texte possibles pour l’élément **IndexIcône** . 
  
|**Valeur**|**Description**|
|:-----|:-----|
|||
|Par défaut  <br/> |Spécifie l’icône par défaut.  <br/> |
|PostItem  <br/> |Spécifie l’icône d’un élément de publication.  <br/> |
|MailRead  <br/> |Spécifie l’icône de lecture du courrier.  <br/> |
|MailUnread  <br/> |Spécifie l’icône courrier non lu.  <br/> |
|MailReplied  <br/> |Spécifie l’icône réponse à un message.  <br/> |
|MailForwarded  <br/> |Spécifie l’icône de courrier transféré.  <br/> |
|MailEncrypted  <br/> |Spécifie l’icône de messagerie chiffrée.  <br/> |
|MailSmimeSigned  <br/> |Spécifie l’icône de courrier signé S/MIME (Secure/Multipurpose Internet Mail Extensions).  <br/> |
|MailEncryptedReplied  <br/> |Spécifie l’icône réponse chiffrée à un message.  <br/> |
|MailSmimeSignedReplied  <br/> |Indique que la signature S/MIME a répondu à l’icône courrier.  <br/> |
|MailEncryptedForwarded  <br/> |Spécifie l’icône du message transféré chiffré.  <br/> |
|MailSmimeSignedForwarded  <br/> |Spécifie l’icône du message signé S/MIME.  <br/> |
|MailEncryptedRead  <br/> |Spécifie l’icône de lecture de message chiffrée.  <br/> |
|MailSmimeSignedRead  <br/> |Spécifie l’icône de courrier lu signé S/MIME.  <br/> |
|MailIrm  <br/> |Spécifie l’icône de messagerie protégée par la gestion des droits relatifs à l’information (IRM).  <br/> |
|MailIrmForwarded  <br/> |Spécifie l’icône de courrier transféré par IRM.  <br/> |
|MailIrmReplied  <br/> |Spécifie l’icône réponse protégée par IRM au courrier.  <br/> |
|SmsSubmitted  <br/> |Spécifie l’icône courrier électronique envoyé pour le routage SMS (Short Message Service).  <br/> |
|SmsRoutedToDeliveryPoint  <br/> |Spécifie l’icône du routage SMS vers un point de remise externe.  <br/> |
|SmsRoutedToExternalMessagingSystem  <br/> |Spécifie l’icône du routage SMS vers un système de messagerie externe.  <br/> |
|SmsDelivered  <br/> |Spécifie l’icône courrier SMS remis.  <br/> |
|OutlookDefaultForContacts  <br/> |Spécifie l’icône par défaut des contacts.  <br/> |
|AppointmentItem  <br/> |Spécifie l’icône de l’élément de rendez-vous.  <br/> |
|AppointmentRecur  <br/> |Spécifie l’icône de rendez-vous périodique.  <br/> |
|AppointmentMeet  <br/> |Spécifie l’icône de la réunion.  <br/> |
|AppointmentMeetRecur  <br/> |Spécifie l’icône de réunion périodique.  <br/> |
|AppointmentMeetNY  <br/> |Spécifie l’icône d’une réponse provisoire à la réunion.  <br/> |
|AppointmentMeetYes  <br/> |Spécifie l’icône d’acceptation de la réunion.  <br/> |
|AppointmentMeetNo  <br/> |Spécifie l’icône de réunion refusée.  <br/> |
|AppointmentMeetMaybe  <br/> |Spécifie l’icône d’une réponse possible à la réunion.  <br/> |
|AppointmentMeetCancel  <br/> |Spécifie l’icône d’annulation de réunion.  <br/> |
|AppointmentMeetInfo  <br/> |Spécifie l’icône des informations sur la réunion.  <br/> |
|TaskItem  <br/> |Spécifie l’icône de l’élément de tâche.  <br/> |
|TaskRecur  <br/> |Spécifie l’icône de tâche périodique.  <br/> |
|TaskOwned  <br/> |Spécifie l’icône de la tâche.  <br/> |
|TaskDelegated  <br/> |Spécifie l’icône de la tâche déléguée.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |false  <br/> |
   


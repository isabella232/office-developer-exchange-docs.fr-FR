---
title: IconIndex
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 92020822-2a86-4dfc-aee1-3067af4d4edf
description: L’élément IconIndex identifie l’index d’icône d’un élément ou d’une conversation.
ms.openlocfilehash: f0c024eeedcbda9aa5ad8afdea09a68f2499798e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541160"
---
# <a name="iconindex"></a>IconIndex

**L’élément IconIndex** identifie l’index d’icône d’un élément ou d’une conversation. 
  
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

Le tableau suivant contient les valeurs de texte possibles pour **l’élément IconIndex.** 
  
|**Valeur**|**Description**|
|:-----|:-----|
|||
|Par défaut  <br/> |Spécifie l’icône par défaut.  <br/> |
|PostItem  <br/> |Spécifie l’icône d’un élément de publication.  <br/> |
|MailRead  <br/> |Spécifie l’icône de lecture du courrier électronique.  <br/> |
|MailUnread  <br/> |Spécifie l’icône de courrier non lu.  <br/> |
|MailReplied  <br/> |Spécifie l’icône de réponse à un message électronique.  <br/> |
|MailForwarded  <br/> |Spécifie l’icône de courrier transmis.  <br/> |
|MailEncrypted  <br/> |Spécifie l’icône de messagerie chiffrée.  <br/> |
|MailSmimeSigned  <br/> |Spécifie l’icône de messagerie signée S/MIME (Secure/Multipurpose Internet Mail Extensions).  <br/> |
|MailEncryptedReplied  <br/> |Spécifie l’icône de message chiffrée à réponse.  <br/> |
|MailSmimeSignedReplied  <br/> |Spécifie le S/MIME signé répondu à l’icône de courrier.  <br/> |
|MailEncryptedForwarded  <br/> |Spécifie l’icône de courrier transmis chiffré.  <br/> |
|MailSmimeSignedForwarded  <br/> |Spécifie l’icône de courrier transmis signé S/MIME.  <br/> |
|MailEncryptedRead  <br/> |Spécifie l’icône de lecture chiffrée du courrier électronique.  <br/> |
|MailSmimeSignedRead  <br/> |Spécifie l’icône de lecture de courrier signé S/MIME.  <br/> |
|MailIrm  <br/> |Spécifie l’icône de messagerie protégée par la Gestion des droits de l’information (IRM).  <br/> |
|MailIrmForwarded  <br/> |Spécifie l’icône de courrier transmis protégé par IRM.  <br/> |
|MailIrmReplied  <br/> |Spécifie l’icône de courrier électronique protégée par IRM.  <br/> |
|SmsSubmitted  <br/> |Spécifie le message d’icône envoyé pour le routage SMS (Short Message Service).  <br/> |
|SmsRoutedToDeliveryPoint  <br/> |Spécifie l’icône pour le routage sms vers un point de remise externe.  <br/> |
|SmsRoutedToExternalMessagingSystem  <br/> |Spécifie l’icône pour le routage des SMS vers un système de messagerie externe.  <br/> |
|SmsDelivered  <br/> |Spécifie l’icône de courrier remis par SMS.  <br/> |
|OutlookDefaultForContacts  <br/> |Spécifie l’icône par défaut pour les contacts.  <br/> |
|AppointmentItem  <br/> |Spécifie l’icône de l’élément de rendez-vous.  <br/> |
|AppointmentRecur  <br/> |Spécifie l’icône de rendez-vous périodique.  <br/> |
|AppointmentMeet  <br/> |Spécifie l’icône de réunion.  <br/> |
|AppointmentMeetRecur  <br/> |Spécifie l’icône de réunion périodique.  <br/> |
|AppointmentMeetNY  <br/> |Spécifie l’icône d’une réponse provisoire à la réunion.  <br/> |
|AppointmentMeetYes  <br/> |Spécifie l’icône d’acceptation de réunion.  <br/> |
|AppointmentMeetNo  <br/> |Spécifie l’icône de réunion refusée.  <br/> |
|AppointmentMeetMaybe  <br/> |Spécifie l’icône d’une réponse à la réunion.  <br/> |
|AppointmentMeetCancel  <br/> |Spécifie l’icône d’annulation de réunion.  <br/> |
|AppointmentMeetInfo  <br/> |Spécifie l’icône d’informations de réunion.  <br/> |
|TaskItem  <br/> |Spécifie l’icône de l’élément de tâche.  <br/> |
|TaskRecur  <br/> |Spécifie l’icône de tâche périodique.  <br/> |
|TaskOwned  <br/> |Spécifie l’icône de la tâche.  <br/> |
|TaskDelegated  <br/> |Spécifie l’icône déléguée de tâche.  <br/> |
   
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
   


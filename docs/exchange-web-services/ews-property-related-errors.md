---
title: Erreurs liées à la propriété EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 1c4c5969-7bdd-4021-be0e-cae99e86cf2c
description: Découvrez comment gérer les erreurs liées à la propriété dans votre application EWS.
ms.openlocfilehash: 5863ab4e06bd968aa38b6fdec471e09c5e23f54a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455407"
---
# <a name="ews-property-related-errors"></a>Erreurs liées à la propriété EWS

Découvrez comment gérer les erreurs liées à la propriété dans votre application EWS.
  
La plupart des applications de client EWS utiliseront les propriétés, ce qui signifie que vous devez gérer les erreurs liées à la propriété. Vous pouvez gérer ces erreurs en cours d'exécution, ou lorsque vous développez votre application EWS.
  
**Tableau 1: Erreurs liées à la propriété et comment gérer ces**

|**Erreur**|**Dû à une tentative de...**|**Traiter par...**|
|:-----|:-----|:-----|
|ErrorDataSizeLimitExceeded  <br/> |Définir une propriété avec une valeur qui dépasse la taille maximale de la propriété ou la propriété ne gère pas la diffusion en continu, telles que les propriétés de dossier.  <br/> |Limiter la taille des données que vous définissez sur la propriété.  <br/> |
|ErrorFolderPropertRequestFailed  <br/> |Obtenir une propriété qui ne peut pas être récupérée.  <br/> |Indiquant que la propriété ne peut pas être récupérée.  <br/> |
|ErrorInvalidExtendedProperty  <br/> |Définir une combinaison des valeurs de propriété étendue ou de résultats non valide dans un argument non valide, la propriété identificateur URI (Uniform Resource) étendu.  <br/> |Vérification de la valeur de la propriété étendue.  <br/> |
|ErrorInvalidExtendedPropertyValue  <br/> |Définir une valeur de la propriété étendue qui ne correspond pas au type spécifié  <br/> |Mise à jour de votre code pour vérifier les types correspondants.  <br/> |
|ErrorInvalidFolderId  <br/> |Définir la structure d'un identificateur de dossier à un formulaire non valide.  <br/> |En utilisant uniquement des identificateurs renvoyés par EWS.  <br/> |
|ErrorInvalidId  <br/> |La structure d'un identificateur de définir la clé à un formulaire non valide.  <br/> |En utilisant uniquement des identificateurs renvoyés par EWS.  <br/> |
|ErrorInvalidIdEmpty  <br/> |Un identificateur de jeu est vide.  <br/> |La définition de l'identificateur avec un identificateur d'élément ou de dossier valide.  <br/> |
|ErrorInvalidIdMalformed  <br/> |La structure d'un identificateur de définir la clé à un formulaire non valide.  <br/> |En utilisant uniquement des identificateurs renvoyés par EWS.  <br/> |
|ErrorInvalidPropertyAppend  <br/> |Ajouter une propriété qui ne prend pas en charge l'ajout.  <br/> |Mise à jour de votre code afin qu'il essaie uniquement à ajouter les valeurs pour les propriétés de la collection de destinataires (à, Cc, Cci), propriétés de collection Attendee (obligatoire, facultatif, ressources), Body, propriété et la propriété ReplyTo.  <br/> |
|ErrorInvalidPropertyDelete  <br/> |Supprimer une propriété qui ne prend pas en charge la suppression.  <br/> |Mise à jour de votre code pour ne pas essayer de supprimer la propriété. Par exemple, le dossier et les identificateurs d'élément ne peut pas être supprimés.  <br/> |
|ErrorInvalidPropertyForExists  <br/> |Définir une restriction existentielle, espérons-le recherche basé sur une propriété basée sur l'indicateur.  <br/> |Mise à jour de votre code pour ne pas utiliser les propriétés basées sur un indicateur dans une restriction de recherche en fonction d'existentielle, espérons-le. Propriétés basées sur l'indicateur sont IsDraft, IsSubmitted, IsUnmodified, IsResend et IsFromMe.  <br/> |
|ErrorInvalidPropertyForOperation  <br/> |Agir sur une propriété d'un élément ou d'un dossier qui n'est pas pris en charge par l'opération.  <br/> |Mise à jour de votre code pour ne pas accéder à la propriété avec l'opération qui a provoqué l'erreur.  <br/> |
|ErrorInvalidPropertyRequest  <br/> |Spécifiez une propriété dans la demande n'est pas pris en charge pour le type d'élément.  <br/> |Mise à jour de votre code pour ne pas essayer d'accéder à la propriété avec l'opération.  <br/> |
|ErrorInvalidPropertySet  <br/> |Définir une propriété en lecture seule.  <br/> |Mise à jour de votre code pour ne pas essayer de définir la propriété.  <br/> |
|ErrorInvalidValueForProperty  <br/> |Comparer une valeur de propriété dans une restriction de recherche dans laquelle la valeur de comparaison ne correspond pas au type de propriété.  <br/> |Mise à jour de votre code pour vérifier incompatibilité de type de propriété.  <br/> |
|ErrorItemSavePropertyError  <br/> |Enregistrer un élément ou un dossier avec des valeurs de propriété non valide.  <br/> |Les valeurs des propriétés et les types de vérification avant de les envoyer dans une demande.  <br/> |
|ErrorNoFolderClassOverride  <br/> |Définissez la classe d'un dossier sur un nouveau dossier qui n'est pas le type de dossier de base.  <br/> |À l'aide d'un type de dossier générique pour définir la classe d'un dossier.  <br/> |
|ErrorNoPropertyTagForCustomProperties  <br/> |Faire référence à une propriété étendue personnalisée par sa balise de propriété.  <br/> |Mise à jour de votre code pour faire référence à la personnalisé étendu identificateur de propriété à la propriété est définie et la propriété nom ou identificateur de propriété de répartition.  <br/> |
|ErrorObjectTypeChanged  <br/> |Définir ou mettre à jour la classe de l'élément sur un élément qui ne correspond pas à son type de schéma.  <br/> |Mise à jour de votre code afin que la classe de l'élément établit une correspondance avec le type d'élément de schéma.  <br/> |
|ErrorPropertyUpdate  <br/> |Mettre à jour une propriété avec une valeur de propriété non valide.  <br/> |Vérification de la valeur de la propriété avant de les envoyer dans une demande de [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) .  <br/> |
|ErrorRequiredPropertyMissing  <br/> |Envoyer une demande CreateAttachment auquel il manque une propriété obligatoire.  <br/> |Mise à jour de votre code pour définir la propriété manquante comme spécifié par le chemin d'accès de la propriété retourné dans la réponse.  <br/> |
|ErrorUnsupportedMapiPropertyType  <br/> |Utilisez des types de propriété étendue de l'objet de type, tableau d'objets, erreur ou null.  <br/> |Mise à jour de votre code pour ne pas utiliser les types de propriété étendue restreints.  <br/> |
|ErrorUnsupportedPathForQuery  <br/> |Utiliser un chemin de propriété non pris en charge dans une restriction de recherche.  <br/> |Modification de la restriction de recherche pour exclure le chemin d'accès de propriété non pris en charge.  <br/> |
|ErrorUnsupportedPathForSortGroup  <br/> |Utiliser un chemin de propriété non pris en charge dans une requête de recherche triées ou regroupées.  <br/> |Modification de la restriction de recherche pour exclure le chemin d'accès de propriété non pris en charge.  <br/> |
|ErrorUnsupportedTypeForConversion  <br/> |Demander un type de propriété qui ne peuvent pas être converti au format XML pour EWS retourner une réponse.  <br/> |Mise à jour de votre code pour ne demander pas la propriété non pris en charge.  <br/> |
|ErrorUpdatePropertyMismatch  <br/> |Mettre à jour un élément ou un dossier pour lequel la description de modification ne correspond pas à la propriété spécifiée à mettre à jour.  <br/> |Modification de votre code afin que la description de la modification établit une correspondance avec le type d'élément ou un dossier est en cours de mise à jour.  <br/> |
   
## <a name="see-also"></a>Voir aussi


- [Les propriétés et les propriétés étendues dans EWS dans Exchange](properties-and-extended-properties-in-ews-in-exchange.md)
    
- [Commencer à utiliser les services web dans Exchange](start-using-web-services-in-exchange.md)
    
- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)
    


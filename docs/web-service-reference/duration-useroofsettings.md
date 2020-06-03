---
title: Durée (UserOofSettings)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Duration
api_type:
- schema
ms.assetid: 01d67af3-658e-4acd-93e3-441ae827fdd3
description: L’élément Duration spécifie la durée pendant laquelle l’État absent (absent du bureau) est activé si l’élément OofState est défini sur planifié.
ms.openlocfilehash: 0ba0f1ea7498781c0cccb072c7ea0fa05414764c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457297"
---
# <a name="duration-useroofsettings"></a>Durée (UserOofSettings)

L’élément **Duration** spécifie la durée pendant laquelle l’État absent (absent du bureau) est activé si l’élément [OofState](oofstate.md) est défini sur **planifié**.
  
```XML
<Duration>
   <StartTime/>
   <EndTime/> 
</Duration>
```

 **Duration**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[StartTime](starttime.md) <br/> |Représente le début de l’intervalle de temps défini avec un statut OOF. Cet élément est obligatoire.  <br/> |
|[EndTime](endtime.md) <br/> |Représente la fin de l’intervalle de temps défini avec un statut OOF. Cet élément est obligatoire.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[UserOofSettings](useroofsettings.md) <br/> |Spécifie les paramètres OOF.  <br/><br/>Voici l’expression XPath de cet élément :<br/><br/>`/SetUserOofSettingsRequest/UserOofSettings` <br/> |
|[OofSettings](oofsettings.md) <br/> |Contient les paramètres OOF.<br/><br/>Voici l’expression XPath de cet élément :<br/><br/>`/GetUserOofSettingsResponse/OofSettings` <br/> |
|[OutOfOffice](outofoffice.md) <br/> |Définit le message de réponse d’absence du bureau et une durée d’envoi du message de réponse pour une boîte aux lettres.  <br/> |
   
## <a name="remarks"></a>Remarques

Le type de **durée** est également le type des éléments [DetailedSuggestionsWindow](detailedsuggestionswindow.md), [TimeWindow](timewindow.md)et [OutOfOffice](outofoffice.md) . 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="example"></a>Exemple

L’exemple suivant de demande d' [opération SetUserOofSettings](setuseroofsettings-operation.md) définit le [OofState](oofstate.md) sur **Enabled**, les messages OOF internes et externes, et définit la durée du OOF pendant 10 jours.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetUserOofSettingsRequest xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <Mailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
        <Name>David Alexander</Name>
        <Address>someone@example.com</Address>
        <RoutingType>SMTP</RoutingType>
      </Mailbox>
      <UserOofSettings xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
        <OofState>Enabled</OofState>
        <ExternalAudience>All</ExternalAudience>
        <Duration>
          <StartTime>2005-10-05T00:00:00</StartTime>
          <EndTime>2005-10-25T00:00:00</EndTime>
        </Duration>
        <InternalReply>
          <Message>I am out of office.  This is my internal reply.</Message>
        </InternalReply>
        <ExternalReply>
          <Message>I am out of office. This is my external reply.</Message>
        </ExternalReply>
        <SetByLegacyClient>false</SetByLegacyClient>
      </UserOofSettings>
    </SetUserOofSettingsRequest>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération GetUserOofSettings](getuseroofsettings-operation.md)  
- [Opération SetUserOofSettings](setuseroofsettings-operation.md)


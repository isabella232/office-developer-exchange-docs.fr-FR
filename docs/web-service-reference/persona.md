---
title: Persona
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: b115c990-3a2d-4536-9af3-ac1fd06d00dc
description: L’élément Persona spécifie un ensemble de données de personnage renvoyées par une demande GetPersona.
ms.openlocfilehash: 0bbab94b7767b19a3b27bd240151c2abd42f3e6f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519239"
---
# <a name="persona"></a>Persona

**L’élément Persona** spécifie un ensemble de données de personnage renvoyées par une **demande GetPersona.** 
  
```XML
<Persona>
   <PersonaId/>
   <PersonaType/>
   <PersonaObjectStatus/>
   <CreationTime/>
   <Bodies/>
   <DisplayNameFirstLastSortKey/>
   <DisplayNameLastFirstSortKey/>
   <CompanyNameSortKey/>
   <HomeCitySortKey/>
   <WorkCitySortKey/>
   <DisplayNameFirstLastHeader/>
   <DisplayNameLastFirstHeader/>
   <FileAsHeader/>
   <DisplayName/>
   <DisplayNameFirstLast/>
   <DisplayNameLastFirst/>
   <FileAs/>
   <FileAsId/>
   <DisplayNamePrefix/>
   <GivenName/>
   <MiddleName/>
   <Surname/>
   <Generation/>
   <Nickname/>
   <YomiCompanyName/>
   <YomiFirstName/>
   <YomiLastName/>
   <Title/>
   <Department/>
   <CompanyName/>
   <Location/>
   <EmailAddress/>
   <EmailAddresses/>
   <PhoneNumber/>
   <ImAddress/>
   <HomeCity/>
   <WorkCity/>
   <RelevanceScore/>
   <FolderIds/>
   <Attributions/>
   <DisplayNames/>
   <FileAses/>
   <FileAsIds/>
   <DisplayNamePrefixes/>
   <GivenNames/>
   <MiddleNames/>
   <Surnames/>
   <Generations/>
   <Nicknames/>
   <Initials/>
   <YomiCompanyNames/>
   <YomiFirstNames/>
   <YomiLastNames/>
   <BusinessPhoneNumbers/>
   <BusinessPhoneNumbers2/>
   <HomePhones/>
   <HomePhones2/>
   <MobilePhones/>
   <MobilePhones2/>
   <AssistantPhoneNumbers/>
   <CallbackPhones/>
   <CarPhones/>
   <HomeFaxes/>
   <OrganizationMainPhones/>
   <OtherFaxes/>
   <OtherTelephones/>
   <OtherPhones2/>
   <Pagers/>
   <RadioPhones/>
   <TelexNumbers/>
   <TTYTDDPhoneNumbers/>
   <WorkFaxes/>
   <Emails1/>
   <Emails2/>
   <Emails3/>
   <BusinessHomePages/>
   <PersonalHomePages/>
   <OfficeLocations/>
   <ImAddresses/>
   <ImAddresses2/>
   <ImAddresses3/>
   <BusinessAddresses/>
   <HomeAddresses/>
   <OtherAddresses/>
   <Titles/>
   <Departments/>
   <CompanyNames/>
   <Managers/>
   <AssistantNames/>
   <Professions/>
   <SpouseNames/>
   <Children/>
   <Schools/>
   <Hobbies/>
   <WeddingAnniversaries/>
   <Birthdays/>
   <Locations/>
   <ExtendedProperties/>
</Persona>

```

 **PersonaType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

[PersonaId](personaid.md)  |  [PersonaType](personatype.md)  |  [PersonaObjectStatus](personaobjectstatus.md)  |  [CreationTime](creationtime.md)  |  [Corps](bodies.md)  |  [DisplayNameFirstLastSortKey](displaynamefirstlastsortkey.md)  |  [DisplayNameLastFirstSortKey](displaynamelastfirstsortkey.md)  |  [CompanyNameSortKey](companynamesortkey.md)  |  [HomeCitySortKey](homecitysortkey.md)  |  [WorkCitySortKey](workcitysortkey.md)  |  [DisplayNameFirstLastHeader](displaynamefirstlastheader.md)  |  [DisplayNameLastFirstHeader](displaynamelastfirstheader.md)  |  [FileAsHeader](fileasheader.md)  |  [DisplayName (chaîne)](displayname-string.md)  |  [DisplayNameFirstLast](displaynamefirstlast.md)  |  [DisplayNameLastFirst](displaynamelastfirst.md)  |  [FileAs](fileas.md)  |  [FileAsId](fileasid.md)  |  [DisplayNamePrefix](displaynameprefix.md)  |  [GivenName](givenname.md)  |  [MiddleName](middlename.md)  |  [Surname](surname.md)  |  [Génération](generation.md)  |  [Nickname](nickname.md)  |  [YomiCompanyName](yomicompanyname.md)  |  [YomiFirstName](yomifirstname.md)  |  [YomiLastName](yomilastname.md)  |  [Titre](title.md)  |  [Service](department.md)  |  [CompanyName](companyname.md)  |  [Emplacement](location.md)  |  [EmailAddress (EmailAddressType)](emailaddress-emailaddresstype.md)  |  [EmailAddresses (ArrayOfEmailAddressesType)](emailaddresses-arrayofemailaddressestype.md)  |  [PhoneNumber](phonenumber.md)  |  [ImAddress (String)](imaddress-string.md)  |  [HomeCity](homecity.md)  |  [WorkCity](workcity.md)  |  [RelevanceScore](relevancescore.md)  |  [FolderIds (ArrayOfFolderIdType)](folderids-arrayoffolderidtype.md)  |  [Attributions (ArrayOfPersonaAttributionsType)](attributions-arrayofpersonaattributionstype.md)  |  [DisplayNames](displaynames.md)  |  [FileAses](fileases.md)  |  [FileAsIds](fileasids.md)  |  [DisplayNamePrefixes](displaynameprefixes.md)  |  [GivenNames](givennames.md)  |  [MiddleNames](middlenames.md)  |  [Surnames](surnames.md)  |  [Générations](generations.md)  |  [Nicknames](nicknames.md)  |  [Initials (ArrayOfStringAttributedValuesType)](initials-arrayofstringattributedvaluestype.md)  |  [YomiCompanyNames](yomicompanynames.md)  |  [YomiFirstNames](yomifirstnames.md)  |  [YomiLastNames](yomilastnames.md)  |  [BusinessPhoneNumbers](businessphonenumbers.md)  |  [BusinessPhoneNumbers2](businessphonenumbers2.md)  |  [HomePhones](homephones.md)  |  [HomePhones2](homephones2.md)  |  [MobilePhones](mobilephones.md)  |  [MobilePhones2](mobilephones2.md)  |  [AssistantPhoneNumbers](assistantphonenumbers.md)  |  [CallbackPhones](callbackphones.md)  |  [CarPhones](carphones.md)  |  [HomeFaxes](homefaxes.md)  |  [OrganizationMainPhones](organizationmainphones.md)  |  [OtherFaxes](otherfaxes.md)  |  [OtherTelephones](othertelephones.md)  |  [OtherPhones2](otherphones2.md)  |  [Pagers](pagers.md)  |  [RadioPhones](radiophones.md)  |  [TelexNumbers](telexnumbers.md)  |  [TTYTDDPhoneNumbers](ttytddphonenumbers.md)  |  [WorkFaxes](workfaxes.md)  |  [Emails1](emails1.md)  |  [Emails2](emails2.md)  |  [Emails3](emails3.md)  |  [BusinessHomePages](businesshomepages.md)  |  [PersonalHomePages](personalhomepages.md)  |  [OfficeLocations](officelocations.md)  |  [ImAddresses (ArrayOfStringAttributedValuesType)](imaddresses-arrayofstringattributedvaluestype.md)  |  [ImAddresses2](imaddresses2.md)  |  [ImAddresses3](imaddresses3.md)  |  [BusinessAddresses](businessaddresses.md)  |  [HomeAddresses](homeaddresses.md)  |  [OtherAddresses](otheraddresses.md)  |  [Titres](titles.md)  |  [Services](departments.md)  |  [CompanyNames](companynames.md)  |  [Responsables](managers.md)  |  [AssistantNames](assistantnames.md)  |  [Professions](professions.md)  |  [SpouseNames](spousenames.md)  |  [Children (ArrayOfStringArrayAttributedValuesType)](children-arrayofstringarrayattributedvaluestype.md)  |  [Écoles](schools.md)  |  [Loisirs](hobbies.md)  |  [Anniversaries](weddinganniversaries.md)  |  [Anniversaires](birthdays.md)  |  [Emplacements](locations.md)  |  [ExtendedProperties (ArrayOfExtendedPropertyAttributedValueType)](extendedproperties-arrayofextendedpropertyattributedvaluetype.md)
  
### <a name="parent-elements"></a>Éléments parents

[AddNewImContactToGroupResponse](addnewimcontacttogroupresponse.md)  |  [AddNewTelUriContactToGroupResponse](addnewteluricontacttogroupresponse.md)  |  [GetPersonaResponseMessage](getpersonaresponsemessage.md)  |  [Personnes](people.md)  |  [Personas](personas-ex15websvcsotherref.md)
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |false  <br/> |
   


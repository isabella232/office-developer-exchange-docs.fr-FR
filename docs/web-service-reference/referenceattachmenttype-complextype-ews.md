---
title: Type complexe ReferenceAttachmentType (EWS)
manager: sethgros
ms.date: 03/9/2015
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 18bfa012-e903-d7f3-528a-31ccceb65463
ms.openlocfilehash: da9ff2b73f86bba3003c31dec009ea11a9b26b32
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829030"
---
# <a name="referenceattachmenttype-complextype-ews"></a><span data-ttu-id="07462-102">Type complexe ReferenceAttachmentType (EWS)</span><span class="sxs-lookup"><span data-stu-id="07462-102">ReferenceAttachmentType complexType (EWS)</span></span>

## <a name="type-information"></a><span data-ttu-id="07462-103">Informations sur le type</span><span class="sxs-lookup"><span data-stu-id="07462-103">Type information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="07462-104">**Espace de noms**</span><span class="sxs-lookup"><span data-stu-id="07462-104">**Namespace**</span></span> <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="07462-105">**Fichier de schéma**</span><span class="sxs-lookup"><span data-stu-id="07462-105">**Schema file**</span></span> <br/> |<span data-ttu-id="07462-106">types.xsd</span><span class="sxs-lookup"><span data-stu-id="07462-106">types.xsd</span></span>  <br/> |
|<span data-ttu-id="07462-107">**Base d’extension**</span><span class="sxs-lookup"><span data-stu-id="07462-107">**Extension base**</span></span> <br/> |<span data-ttu-id="07462-108">t:AttachmentType</span><span class="sxs-lookup"><span data-stu-id="07462-108">t:AttachmentType</span></span>  <br/> |
   
## <a name="definition"></a><span data-ttu-id="07462-109">Définition</span><span class="sxs-lookup"><span data-stu-id="07462-109">Definition</span></span>

```XML
<xs:complexType name="ReferenceAttachmentType">
    <xs:complexContent>
        <xs:extension base="t:AttachmentType">
            <xs:sequence>
                <xs:element name="AttachLongPathName" type="xs:string" maxOccurs="1" minOccurs="0"></xs:element>
            </xs:sequence>
        </xs:extension>
    </xs:complexContent>
</xs:complexType>

```

## <a name="elements-and-attributes"></a><span data-ttu-id="07462-110">Éléments et attributs</span><span class="sxs-lookup"><span data-stu-id="07462-110">Elements and attributes</span></span>

<span data-ttu-id="07462-111">Si le schéma définit des exigences spécifiques, telles que **sequence**, **minOccurs**, **maxOccurs**et **choice**, voir la section Définition.</span><span class="sxs-lookup"><span data-stu-id="07462-111">If the schema defines specific requirements, such as **sequence**, **minOccurs**, **maxOccurs**, and **choice**, see the definition section.</span></span> 
  
### <a name="child-elements"></a><span data-ttu-id="07462-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="07462-112">Child elements</span></span>

|<span data-ttu-id="07462-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="07462-113">**Element**</span></span>|<span data-ttu-id="07462-114">**Type**</span><span class="sxs-lookup"><span data-stu-id="07462-114">**Type**</span></span>|<span data-ttu-id="07462-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="07462-115">**Description**</span></span>|
|:-----|:-----|:-----|
|[<span data-ttu-id="07462-116">AttachLongPathName</span><span class="sxs-lookup"><span data-stu-id="07462-116">AttachLongPathName</span></span>](http://msdn.microsoft.com/library/98464422-2c13-8d33-0fe3-b1978f2d5b4a%28Office.15%29.aspx) <br/> |<span data-ttu-id="07462-117">xs:string</span><span class="sxs-lookup"><span data-stu-id="07462-117">xs:string</span></span>  <br/> ||
   
### <a name="attributes"></a><span data-ttu-id="07462-118">Attributs</span><span class="sxs-lookup"><span data-stu-id="07462-118">Attributes</span></span>

<span data-ttu-id="07462-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="07462-119">None.</span></span>
  


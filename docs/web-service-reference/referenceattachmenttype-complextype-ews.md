---
title: ComplexType ReferenceAttachmentType (EWS)
manager: sethgros
ms.date: 03/9/2015
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 18bfa012-e903-d7f3-528a-31ccceb65463
ms.openlocfilehash: 24f5a62eadd490b5b0000dfe048850c44540f266
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528733"
---
# <a name="referenceattachmenttype-complextype-ews"></a><span data-ttu-id="782cb-102">ComplexType ReferenceAttachmentType (EWS)</span><span class="sxs-lookup"><span data-stu-id="782cb-102">ReferenceAttachmentType complexType (EWS)</span></span>

## <a name="type-information"></a><span data-ttu-id="782cb-103">Informations sur le type</span><span class="sxs-lookup"><span data-stu-id="782cb-103">Type information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="782cb-104">**Namespace**</span><span class="sxs-lookup"><span data-stu-id="782cb-104">**Namespace**</span></span> <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="782cb-105">**Fichier de schéma**</span><span class="sxs-lookup"><span data-stu-id="782cb-105">**Schema file**</span></span> <br/> |<span data-ttu-id="782cb-106">types. xsd</span><span class="sxs-lookup"><span data-stu-id="782cb-106">types.xsd</span></span>  <br/> |
|<span data-ttu-id="782cb-107">**Base d’extension**</span><span class="sxs-lookup"><span data-stu-id="782cb-107">**Extension base**</span></span> <br/> |<span data-ttu-id="782cb-108">t:AttachmentType</span><span class="sxs-lookup"><span data-stu-id="782cb-108">t:AttachmentType</span></span>  <br/> |
   
## <a name="definition"></a><span data-ttu-id="782cb-109">Définition</span><span class="sxs-lookup"><span data-stu-id="782cb-109">Definition</span></span>

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

## <a name="elements-and-attributes"></a><span data-ttu-id="782cb-110">Éléments et attributs</span><span class="sxs-lookup"><span data-stu-id="782cb-110">Elements and attributes</span></span>

<span data-ttu-id="782cb-111">Si le schéma définit des exigences spécifiques, telles que **Sequence**, **minOccurs**, **maxOccurs**et **Choice**, reportez-vous à la section définition.</span><span class="sxs-lookup"><span data-stu-id="782cb-111">If the schema defines specific requirements, such as **sequence**, **minOccurs**, **maxOccurs**, and **choice**, see the definition section.</span></span> 
  
### <a name="child-elements"></a><span data-ttu-id="782cb-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="782cb-112">Child elements</span></span>

|<span data-ttu-id="782cb-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="782cb-113">**Element**</span></span>|<span data-ttu-id="782cb-114">**Type**</span><span class="sxs-lookup"><span data-stu-id="782cb-114">**Type**</span></span>|<span data-ttu-id="782cb-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="782cb-115">**Description**</span></span>|
|:-----|:-----|:-----|
|[<span data-ttu-id="782cb-116">AttachLongPathName</span><span class="sxs-lookup"><span data-stu-id="782cb-116">AttachLongPathName</span></span>](attachlongpathname.md) <br/> |<span data-ttu-id="782cb-117">XS : String</span><span class="sxs-lookup"><span data-stu-id="782cb-117">xs:string</span></span>  <br/> ||
   
### <a name="attributes"></a><span data-ttu-id="782cb-118">Attributs</span><span class="sxs-lookup"><span data-stu-id="782cb-118">Attributes</span></span>

<span data-ttu-id="782cb-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="782cb-119">None.</span></span>
  


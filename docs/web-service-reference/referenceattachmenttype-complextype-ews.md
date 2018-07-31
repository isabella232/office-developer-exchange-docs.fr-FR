---
title: Type complexe ReferenceAttachmentType (EWS)
manager: sethgros
ms.date: 03/9/2015
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 18bfa012-e903-d7f3-528a-31ccceb65463
ms.openlocfilehash: c53686ccd032cabcc3f64a3a6684f29afe63a9b1
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354175"
---
# <a name="referenceattachmenttype-complextype-ews"></a><span data-ttu-id="32ea9-102">Type complexe ReferenceAttachmentType (EWS)</span><span class="sxs-lookup"><span data-stu-id="32ea9-102">ReferenceAttachmentType complexType (EWS)</span></span>

## <a name="type-information"></a><span data-ttu-id="32ea9-103">Informations sur le type</span><span class="sxs-lookup"><span data-stu-id="32ea9-103">Type information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="32ea9-104">**Espace de noms**</span><span class="sxs-lookup"><span data-stu-id="32ea9-104">**Namespace**</span></span> <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="32ea9-105">**Fichier de schéma**</span><span class="sxs-lookup"><span data-stu-id="32ea9-105">**Schema file**</span></span> <br/> |<span data-ttu-id="32ea9-106">types.xsd</span><span class="sxs-lookup"><span data-stu-id="32ea9-106">types.xsd</span></span>  <br/> |
|<span data-ttu-id="32ea9-107">**Base d’extension**</span><span class="sxs-lookup"><span data-stu-id="32ea9-107">**Extension base**</span></span> <br/> |<span data-ttu-id="32ea9-108">t:AttachmentType</span><span class="sxs-lookup"><span data-stu-id="32ea9-108">t:AttachmentType</span></span>  <br/> |
   
## <a name="definition"></a><span data-ttu-id="32ea9-109">Définition</span><span class="sxs-lookup"><span data-stu-id="32ea9-109">Definition</span></span>

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

## <a name="elements-and-attributes"></a><span data-ttu-id="32ea9-110">Éléments et attributs</span><span class="sxs-lookup"><span data-stu-id="32ea9-110">Elements and attributes</span></span>

<span data-ttu-id="32ea9-111">Si le schéma définit des exigences spécifiques, telles que **sequence**, **minOccurs**, **maxOccurs**et **choice**, voir la section Définition.</span><span class="sxs-lookup"><span data-stu-id="32ea9-111">If the schema defines specific requirements, such as **sequence**, **minOccurs**, **maxOccurs**, and **choice**, see the definition section.</span></span> 
  
### <a name="child-elements"></a><span data-ttu-id="32ea9-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="32ea9-112">Child elements</span></span>

|<span data-ttu-id="32ea9-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="32ea9-113">**Element**</span></span>|<span data-ttu-id="32ea9-114">**Type**</span><span class="sxs-lookup"><span data-stu-id="32ea9-114">**Type**</span></span>|<span data-ttu-id="32ea9-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="32ea9-115">**Description**</span></span>|
|:-----|:-----|:-----|
|[<span data-ttu-id="32ea9-116">AttachLongPathName</span><span class="sxs-lookup"><span data-stu-id="32ea9-116">AttachLongPathName</span></span>](attachlongpathname.md) <br/> |<span data-ttu-id="32ea9-117">xs:string</span><span class="sxs-lookup"><span data-stu-id="32ea9-117">xs:string</span></span>  <br/> ||
   
### <a name="attributes"></a><span data-ttu-id="32ea9-118">Attributs</span><span class="sxs-lookup"><span data-stu-id="32ea9-118">Attributes</span></span>

<span data-ttu-id="32ea9-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="32ea9-119">None.</span></span>
  


---
title: Périodicités et EWS
manager: luken
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: fd9ef706-1e01-49fa-af6f-2f6d3e173c16
description: Découvrez les périodicités et les séries périodiques dans Exchange.
ms.openlocfilehash: 681dfee7e0a66a483b8638810da5e4e0ac0f05ac
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459327"
---
# <a name="recurrence-patterns-and-ews"></a><span data-ttu-id="4097e-103">Périodicités et EWS</span><span class="sxs-lookup"><span data-stu-id="4097e-103">Recurrence patterns and EWS</span></span>

<span data-ttu-id="4097e-104">Découvrez les périodicités et les séries périodiques dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="4097e-104">Learn about recurrence patterns and recurring series in Exchange.</span></span>
  
<span data-ttu-id="4097e-105">Une série périodique est un rendez-vous ou une réunion qui se répète en fonction d’un motif défini.</span><span class="sxs-lookup"><span data-stu-id="4097e-105">A recurring series is an appointment or meeting that repeats according to a defined pattern.</span></span> <span data-ttu-id="4097e-106">Une série périodique peut avoir un nombre d’occurrences spécifique ou se répéter indéfiniment.</span><span class="sxs-lookup"><span data-stu-id="4097e-106">A recurring series can either have a specific number of occurrences or can repeat indefinitely.</span></span> <span data-ttu-id="4097e-107">En outre, une série périodique peut avoir des exceptions qui ne suivent pas le modèle du reste des occurrences, et peuvent avoir des occurrences qui ont été supprimées du modèle.</span><span class="sxs-lookup"><span data-stu-id="4097e-107">Additionally, a recurring series can have exceptions that don't follow the pattern of the rest of the occurrences, and can have occurrences that have been deleted from the pattern.</span></span> <span data-ttu-id="4097e-108">Vous pouvez utiliser l’API managée EWS et EWS pour utiliser des séries périodiques et leurs éléments de calendrier associés.</span><span class="sxs-lookup"><span data-stu-id="4097e-108">You can use the EWS Managed API and EWS to work with recurring series and their associated calendar items.</span></span>
  
## <a name="recurring-calendar-items"></a><span data-ttu-id="4097e-109">Éléments de calendrier périodiques</span><span class="sxs-lookup"><span data-stu-id="4097e-109">Recurring calendar items</span></span>

<span data-ttu-id="4097e-110">Tous les éléments de calendrier appartiennent à l’une des quatre catégories suivantes :</span><span class="sxs-lookup"><span data-stu-id="4097e-110">All calendar items fall into one of the following four categories:</span></span>
  
- <span data-ttu-id="4097e-111">Éléments de calendrier non périodiques</span><span class="sxs-lookup"><span data-stu-id="4097e-111">Non-recurring calendar items</span></span>
    
- <span data-ttu-id="4097e-112">Masques périodiques</span><span class="sxs-lookup"><span data-stu-id="4097e-112">Recurring masters</span></span>
    
- <span data-ttu-id="4097e-113">Occurrences dans une série</span><span class="sxs-lookup"><span data-stu-id="4097e-113">Occurrences in a series</span></span>
    
- <span data-ttu-id="4097e-114">Occurrences modifiées dans une série, appelées exceptions</span><span class="sxs-lookup"><span data-stu-id="4097e-114">Modified occurrences in a series, known as exceptions</span></span>
    
<span data-ttu-id="4097e-115">Dans cet article, nous allons examiner les trois types d’éléments de calendrier qui font partie d’une série périodique.</span><span class="sxs-lookup"><span data-stu-id="4097e-115">In this article, we'll look at the three types of calendar items that are part of a recurring series.</span></span>
  
<span data-ttu-id="4097e-116">Il est utile de comprendre comment les séries périodiques sont implémentées sur le serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="4097e-116">It's helpful to understand how recurring series are implemented on the Exchange server.</span></span> <span data-ttu-id="4097e-117">Au lieu de créer un élément distinct distinct pour chaque occurrence dans une série périodique, le serveur ne crée qu’un seul élément réel dans le calendrier, connu sous le nom de forme de base périodique.</span><span class="sxs-lookup"><span data-stu-id="4097e-117">Instead of creating a separate distinct item for each occurrence in a recurring series, the server creates only one actual item in the calendar, known as the recurring master.</span></span> <span data-ttu-id="4097e-118">Le format d’une forme de base périodique est très similaire à un rendez-vous non périodique, avec l’ajout d’informations sur le modèle de récurrence.</span><span class="sxs-lookup"><span data-stu-id="4097e-118">The format of a recurring master is very similar to a non-recurring appointment, with the addition of recurrence pattern information.</span></span> <span data-ttu-id="4097e-119">Le serveur génère ensuite des occurrences en fonction de la périodicité en réponse aux demandes des clients pour les informations de rendez-vous, à l’aide d’un processus appelé expansion.</span><span class="sxs-lookup"><span data-stu-id="4097e-119">The server then generates occurrences based on the recurrence pattern in response to client requests for appointment information, using a process called expansion.</span></span> <span data-ttu-id="4097e-120">Ces occurrences générées ne sont pas stockées de façon définitive sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="4097e-120">These generated occurrences are not permanently stored on the server.</span></span> <span data-ttu-id="4097e-121">Ceci est important pour comprendre la façon dont vous recherchez des éléments de calendrier détermine les informations que vous recevez et si l’expansion se produit.</span><span class="sxs-lookup"><span data-stu-id="4097e-121">This is important to understand because the way that you search for calendar items determines what information you receive and whether expansion occurs.</span></span>
  
## <a name="recurrence-patterns"></a><span data-ttu-id="4097e-122">Périodicités</span><span class="sxs-lookup"><span data-stu-id="4097e-122">Recurrence patterns</span></span>

<span data-ttu-id="4097e-123">La clé d’une série périodique qui rend le développement possible est la périodicité.</span><span class="sxs-lookup"><span data-stu-id="4097e-123">The key piece to a recurring series that makes expansion possible is the recurrence pattern.</span></span> <span data-ttu-id="4097e-124">La périodicité se trouve sur la forme de base périodique et décrit un ensemble de critères permettant de calculer les occurrences en fonction de la date et de l’heure de la forme de base périodique.</span><span class="sxs-lookup"><span data-stu-id="4097e-124">The recurrence pattern is found on the recurring master, and describes a set of criteria for calculating occurrences based on the date and time of the recurring master.</span></span>
  
<span data-ttu-id="4097e-125">**Tableau 1. Périodicités disponibles**</span><span class="sxs-lookup"><span data-stu-id="4097e-125">**Table 1. Available recurrence patterns**</span></span>

|<span data-ttu-id="4097e-126">**Classe d’API managée EWS**</span><span class="sxs-lookup"><span data-stu-id="4097e-126">**EWS Managed API class**</span></span>|<span data-ttu-id="4097e-127">**Élément EWS**</span><span class="sxs-lookup"><span data-stu-id="4097e-127">**EWS element**</span></span>|<span data-ttu-id="4097e-128">**Exemples**</span><span class="sxs-lookup"><span data-stu-id="4097e-128">**Examples**</span></span>|
|:-----|:-----|:-----|
|[<span data-ttu-id="4097e-129">Recurrence. DailyPattern</span><span class="sxs-lookup"><span data-stu-id="4097e-129">Recurrence.DailyPattern</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.dailypattern%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="4097e-130">DailyRecurrence</span><span class="sxs-lookup"><span data-stu-id="4097e-130">DailyRecurrence</span></span>](https://msdn.microsoft.com/library/0aaf265d-b723-49c6-8e9c-9ba60141e9ab%28Office.15%29.aspx) <br/> |<span data-ttu-id="4097e-131">Répéter tous les jours.</span><span class="sxs-lookup"><span data-stu-id="4097e-131">Repeat every day.</span></span>  <br/> <span data-ttu-id="4097e-132">Répéter tous les deux jours.</span><span class="sxs-lookup"><span data-stu-id="4097e-132">Repeat every other day.</span></span>  <br/> |
|[<span data-ttu-id="4097e-133">Recurrence. MonthlyPattern</span><span class="sxs-lookup"><span data-stu-id="4097e-133">Recurrence.MonthlyPattern</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.monthlypattern%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="4097e-134">AbsoluteMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="4097e-134">AbsoluteMonthlyRecurrence</span></span>](https://msdn.microsoft.com/library/178fa0ae-9dfc-417f-933c-d657d31c2161%28Office.15%29.aspx) <br/> |<span data-ttu-id="4097e-135">Répétez chaque mois le dixième jour du mois.</span><span class="sxs-lookup"><span data-stu-id="4097e-135">Repeat every month on the tenth day of the month.</span></span>  <br/> <span data-ttu-id="4097e-136">Répétez tous les deux mois le vingt-premier jour du mois.</span><span class="sxs-lookup"><span data-stu-id="4097e-136">Repeat every other month on the twenty-first day of the month.</span></span>  <br/> |
|[<span data-ttu-id="4097e-137">Recurrence. RelativeMonthlyPattern</span><span class="sxs-lookup"><span data-stu-id="4097e-137">Recurrence.RelativeMonthlyPattern</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.relativemonthlypattern%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="4097e-138">RelativeMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="4097e-138">RelativeMonthlyRecurrence</span></span>](https://msdn.microsoft.com/library/a76595db-7460-44ac-ac2a-53241caa33a7%28Office.15%29.aspx) <br/> |<span data-ttu-id="4097e-139">Répétez le deuxième mardi de chaque mois.</span><span class="sxs-lookup"><span data-stu-id="4097e-139">Repeat on the second Tuesday of every month.</span></span>  <br/> <span data-ttu-id="4097e-140">Répétez le troisième jeudi du mois tous les trois mois.</span><span class="sxs-lookup"><span data-stu-id="4097e-140">Repeat on the third Thursday of the month every three months.</span></span>  <br/> |
|[<span data-ttu-id="4097e-141">Recurrence. RelativeYearlyPattern</span><span class="sxs-lookup"><span data-stu-id="4097e-141">Recurrence.RelativeYearlyPattern</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.relativeyearlypattern%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="4097e-142">RelativeYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="4097e-142">RelativeYearlyRecurrence</span></span>](https://msdn.microsoft.com/library/25b67876-9979-4a30-a637-357ea10a93b8%28Office.15%29.aspx) <br/> |<span data-ttu-id="4097e-143">Répétez l’opération le premier lundi d’août de chaque année.</span><span class="sxs-lookup"><span data-stu-id="4097e-143">Repeat on the first Monday of August every year.</span></span>  <br/> |
|[<span data-ttu-id="4097e-144">Recurrence. WeeklyPattern</span><span class="sxs-lookup"><span data-stu-id="4097e-144">Recurrence.WeeklyPattern</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.weeklypattern%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="4097e-145">WeeklyRecurrence</span><span class="sxs-lookup"><span data-stu-id="4097e-145">WeeklyRecurrence</span></span>](https://msdn.microsoft.com/library/69c41dd5-597c-45bc-be3f-e2f2b5615aa3%28Office.15%29.aspx) <br/> |<span data-ttu-id="4097e-146">Répéter tous les lundi.</span><span class="sxs-lookup"><span data-stu-id="4097e-146">Repeat every Monday.</span></span>  <br/> <span data-ttu-id="4097e-147">Répétez tous les mardis et tous les deux semaines.</span><span class="sxs-lookup"><span data-stu-id="4097e-147">Repeat every Tuesday and Thursday every other week.</span></span>  <br/> |
|[<span data-ttu-id="4097e-148">Recurrence. YearlyPattern</span><span class="sxs-lookup"><span data-stu-id="4097e-148">Recurrence.YearlyPattern</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.yearlypattern%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="4097e-149">AbsoluteYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="4097e-149">AbsoluteYearlyRecurrence</span></span>](https://msdn.microsoft.com/library/96f53e2c-3893-4f6e-a78a-ac179f45c5db%28Office.15%29.aspx) <br/> |<span data-ttu-id="4097e-150">Répétez le 1er septembre chaque année.</span><span class="sxs-lookup"><span data-stu-id="4097e-150">Repeat on September 1st every year.</span></span>  <br/> |
   
<span data-ttu-id="4097e-151">L’autre information importante pour un modèle de récurrence se trouve à la fin de la périodicité.</span><span class="sxs-lookup"><span data-stu-id="4097e-151">The other important piece of information for a recurrence pattern is when the recurrence ends.</span></span> <span data-ttu-id="4097e-152">Elle peut être exprimée sous la forme d’un nombre défini d’occurrences, d’une date de fin ou d’une absence de fin.</span><span class="sxs-lookup"><span data-stu-id="4097e-152">This can be expressed as either a set number of occurrences, as an end date, or as having no end.</span></span>
  
<span data-ttu-id="4097e-153">**Tableau 2. Options de la fin d’une série périodique**</span><span class="sxs-lookup"><span data-stu-id="4097e-153">**Table 2. Options for the end of a recurring series**</span></span>

|<span data-ttu-id="4097e-154">**Méthode/propriété de l’API managée EWS**</span><span class="sxs-lookup"><span data-stu-id="4097e-154">**EWS Managed API method/property**</span></span>|<span data-ttu-id="4097e-155">**Élément EWS**</span><span class="sxs-lookup"><span data-stu-id="4097e-155">**EWS element**</span></span>|<span data-ttu-id="4097e-156">**Description**</span><span class="sxs-lookup"><span data-stu-id="4097e-156">**Description**</span></span>|
|:-----|:-----|:-----|
|[<span data-ttu-id="4097e-157">Recurrence. NumberOfOccurrences</span><span class="sxs-lookup"><span data-stu-id="4097e-157">Recurrence.NumberOfOccurrences</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.numberofoccurrences%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="4097e-158">NumberedRecurrence</span><span class="sxs-lookup"><span data-stu-id="4097e-158">NumberedRecurrence</span></span>](https://msdn.microsoft.com/library/53746909-ef21-4764-8715-a7769b943cca%28Office.15%29.aspx) <br/> |<span data-ttu-id="4097e-159">La valeur de cette propriété ou de cet élément spécifie le nombre d’occurrences.</span><span class="sxs-lookup"><span data-stu-id="4097e-159">The value of this property or element specifies the number of occurrences.</span></span>  <br/> |
|[<span data-ttu-id="4097e-160">Recurrence. EndDate</span><span class="sxs-lookup"><span data-stu-id="4097e-160">Recurrence.EndDate</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.enddate%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="4097e-161">EndDateRecurrence</span><span class="sxs-lookup"><span data-stu-id="4097e-161">EndDateRecurrence</span></span>](https://msdn.microsoft.com/library/a5ee2504-db84-49ee-870c-cca9269f2e26%28Office.15%29.aspx) <br/> |<span data-ttu-id="4097e-162">La dernière occurrence de la série se situe au plus tard à la date spécifiée par cette propriété ou cet élément.</span><span class="sxs-lookup"><span data-stu-id="4097e-162">The last occurrence in the series falls on or before the date specified by this property or element.</span></span>  <br/> |
|[<span data-ttu-id="4097e-163">Recurrence. HasEnd</span><span class="sxs-lookup"><span data-stu-id="4097e-163">Recurrence.HasEnd</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.hasend%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="4097e-164">Recurrence. NeverEnds</span><span class="sxs-lookup"><span data-stu-id="4097e-164">Recurrence.NeverEnds</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.neverends%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="4097e-165">NoEndRecurrence</span><span class="sxs-lookup"><span data-stu-id="4097e-165">NoEndRecurrence</span></span>](https://msdn.microsoft.com/library/ab2ebd9c-388e-45f1-abf9-56e293ef123b%28Office.15%29.aspx) <br/> |<span data-ttu-id="4097e-166">La série n’a pas de fin.</span><span class="sxs-lookup"><span data-stu-id="4097e-166">The series has no end.</span></span>  <br/> |
   
## <a name="expanded-vs-non-expanded-views"></a><span data-ttu-id="4097e-167">Vues étendues et non étendues</span><span class="sxs-lookup"><span data-stu-id="4097e-167">Expanded vs. non-expanded views</span></span>

<span data-ttu-id="4097e-168">L’utilisation de la méthode **findappointmentspour** dans l’API managée EWS (ou l’opération **FindItem** avec un élément **CalendarView** dans EWS) appelle le processus d’expansion.</span><span class="sxs-lookup"><span data-stu-id="4097e-168">Using the **FindAppointments** method in the EWS Managed API (or the **FindItem** operation with a **CalendarView** element in EWS) invokes the expansion process.</span></span> <span data-ttu-id="4097e-169">Cette action masque les rendez-vous périodiques du jeu de résultats et présente une vue développée de cette série périodique.</span><span class="sxs-lookup"><span data-stu-id="4097e-169">This hides recurring master appointments from the result set, and instead presents an expanded view of that recurring series.</span></span> <span data-ttu-id="4097e-170">Les occurrences de la forme de base périodique qui correspondent aux paramètres de l’affichage Calendrier sont incluses dans le jeu de résultats.</span><span class="sxs-lookup"><span data-stu-id="4097e-170">Occurrences of and exceptions to the recurring master that fall within the parameters of the calendar view are included in the result set.</span></span> <span data-ttu-id="4097e-171">À l’inverse, l’utilisation de la méthode **FindItems** dans l’API managée EWS (ou l’opération **FindItem** avec un élément **IndexedPageItemView** ou **FractionalPageItemView** dans EWS) n’invoque pas le processus d’expansion, et les occurrences et les exceptions ne sont pas incluses.</span><span class="sxs-lookup"><span data-stu-id="4097e-171">Conversely, using the **FindItems** method in the EWS Managed API (or the **FindItem** operation with a **IndexedPageItemView** or **FractionalPageItemView** element in EWS), does not invoke the expansion process, and occurrences and exceptions are not included.</span></span> <span data-ttu-id="4097e-172">Examinons un exemple de comparaison des deux méthodes.</span><span class="sxs-lookup"><span data-stu-id="4097e-172">Let's look at an example comparing the two methods.</span></span> 
  
<span data-ttu-id="4097e-173">**Tableau 3. Méthodes et opérations de recherche de rendez-vous**</span><span class="sxs-lookup"><span data-stu-id="4097e-173">**Table 3. Methods and operations for finding appointments**</span></span>

|<span data-ttu-id="4097e-174">**Méthode d'API managée EWS**</span><span class="sxs-lookup"><span data-stu-id="4097e-174">**EWS Managed API method**</span></span>|<span data-ttu-id="4097e-175">**Opération EWS**</span><span class="sxs-lookup"><span data-stu-id="4097e-175">**EWS operation**</span></span>|<span data-ttu-id="4097e-176">**Développe la série ?**</span><span class="sxs-lookup"><span data-stu-id="4097e-176">**Expands series?**</span></span>|<span data-ttu-id="4097e-177">**Éléments inclus dans les résultats**</span><span class="sxs-lookup"><span data-stu-id="4097e-177">**Items included in results**</span></span>|
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="4097e-178">ExchangeService. Findappointmentspour</span><span class="sxs-lookup"><span data-stu-id="4097e-178">ExchangeService.FindAppointments</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="4097e-179">[Opération FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) avec un élément [CalendarView](https://msdn.microsoft.com/library/a4a953b8-0710-416c-95ef-59e51eba9982%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="4097e-179">[FindItem operation](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) with a [CalendarView](https://msdn.microsoft.com/library/a4a953b8-0710-416c-95ef-59e51eba9982%28Office.15%29.aspx) element</span></span>  <br/> |<span data-ttu-id="4097e-180">Oui</span><span class="sxs-lookup"><span data-stu-id="4097e-180">Yes</span></span>  <br/> |<span data-ttu-id="4097e-181">Rendez-vous non périodiques, occurrences uniques de la série périodique et exceptions à la série périodique</span><span class="sxs-lookup"><span data-stu-id="4097e-181">Non-recurring appointments, single occurrences of recurring series, and exceptions to recurring series</span></span>  <br/> |
|[<span data-ttu-id="4097e-182">ExchangeService. FindItems</span><span class="sxs-lookup"><span data-stu-id="4097e-182">ExchangeService.FindItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="4097e-183">[Opération FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) avec un élément [IndexedPageItemView](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) ou [FractionalPageItemView](https://msdn.microsoft.com/library/4111afec-35e7-4c6f-b291-9bbba603f633%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="4097e-183">[FindItem operation](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) with an [IndexedPageItemView](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) element or [FractionalPageItemView](https://msdn.microsoft.com/library/4111afec-35e7-4c6f-b291-9bbba603f633%28Office.15%29.aspx) element</span></span>  <br/> |<span data-ttu-id="4097e-184">Non</span><span class="sxs-lookup"><span data-stu-id="4097e-184">No</span></span>  <br/> |<span data-ttu-id="4097e-185">Rendez-vous non périodiques et rendez-vous périodiques récurrents</span><span class="sxs-lookup"><span data-stu-id="4097e-185">Non-recurring appointments and recurring master appointments</span></span>  <br/> |
   
<span data-ttu-id="4097e-186">Sadie vient de signer son fils pour l’équipe de natation.</span><span class="sxs-lookup"><span data-stu-id="4097e-186">Sadie has just signed her son up for swim team.</span></span> <span data-ttu-id="4097e-187">L’équipe s’est terminée tous les mercredi matin à 8:30 AM, à partir du 2 juillet, avec la dernière pratique du 6 août.</span><span class="sxs-lookup"><span data-stu-id="4097e-187">The team has practice every Wednesday morning at 8:30 AM, starting July 2, with the last practice being on August 6.</span></span> <span data-ttu-id="4097e-188">Ne souhaitant pas oublier de s’en entraîner, Sadie ajoute un rendez-vous périodique à son calendrier pour le rappeler.</span><span class="sxs-lookup"><span data-stu-id="4097e-188">Not wanting to forget about practice, Sadie adds a recurring appointment to her calendar to remind her.</span></span>
  
<span data-ttu-id="4097e-189">**Tableau 4. Rendez-vous périodique Sadie**</span><span class="sxs-lookup"><span data-stu-id="4097e-189">**Table 4. Sadie's recurring appointment**</span></span>

|<span data-ttu-id="4097e-190">**Champ de rendez-vous**</span><span class="sxs-lookup"><span data-stu-id="4097e-190">**Appointment field**</span></span>|<span data-ttu-id="4097e-191">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="4097e-191">**Value**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4097e-192">Subject</span><span class="sxs-lookup"><span data-stu-id="4097e-192">Subject</span></span>  <br/> |<span data-ttu-id="4097e-193">Expérience d’équipe de natation</span><span class="sxs-lookup"><span data-stu-id="4097e-193">Swim Team Practice</span></span>  <br/> |
|<span data-ttu-id="4097e-194">Démarrer</span><span class="sxs-lookup"><span data-stu-id="4097e-194">Start</span></span>  <br/> |<span data-ttu-id="4097e-195">2 juillet 2014 8:30 AM</span><span class="sxs-lookup"><span data-stu-id="4097e-195">July 2, 2014 8:30 AM</span></span>  <br/> |
|<span data-ttu-id="4097e-196">End</span><span class="sxs-lookup"><span data-stu-id="4097e-196">End</span></span>  <br/> |<span data-ttu-id="4097e-197">2 juillet 2014 10:00 AM</span><span class="sxs-lookup"><span data-stu-id="4097e-197">July 2, 2014 10:00 AM</span></span>  <br/> |
|<span data-ttu-id="4097e-198">Nouvelle occurrence</span><span class="sxs-lookup"><span data-stu-id="4097e-198">Recurs</span></span>  <br/> |<span data-ttu-id="4097e-199">Tous les mercredis</span><span class="sxs-lookup"><span data-stu-id="4097e-199">Every Wednesday</span></span>  <br/> |
|<span data-ttu-id="4097e-200">Dernière occurrence</span><span class="sxs-lookup"><span data-stu-id="4097e-200">Last occurrence</span></span>  <br/> |<span data-ttu-id="4097e-201">6 août 2014 8:30 AM</span><span class="sxs-lookup"><span data-stu-id="4097e-201">August 6, 2014 8:30 AM</span></span>  <br/> |
   
<span data-ttu-id="4097e-202">Un aperçu rapide d’un calendrier montre que l’équipe aura un total de six pratiques.</span><span class="sxs-lookup"><span data-stu-id="4097e-202">A quick look at a calendar shows that the team will have a total of six practices.</span></span> <span data-ttu-id="4097e-203">Toutefois, il n’y a pas six éléments de rendez-vous distincts dans le calendrier.</span><span class="sxs-lookup"><span data-stu-id="4097e-203">However, there aren't six distinct appointment items in the calendar.</span></span> <span data-ttu-id="4097e-204">Au lieu de cela, il n’existe qu’un seul rendez-vous périodique principal représentant la série.</span><span class="sxs-lookup"><span data-stu-id="4097e-204">Instead, there is just one recurring master appointment representing the series.</span></span>
  
<span data-ttu-id="4097e-205">Examinons à présent les rendez-vous sur le calendrier de Sadie qui se produisent au cours du mois de juillet.</span><span class="sxs-lookup"><span data-stu-id="4097e-205">Now let's look at finding appointments on Sadie's calendar that occur within the month of July.</span></span> <span data-ttu-id="4097e-206">L’exemple de code suivant utilise la méthode **FindItems** dans l’API managée Exchange pour produire une vue non développée du calendrier de Sadie.</span><span class="sxs-lookup"><span data-stu-id="4097e-206">The following code example uses the **FindItems** method in the Exchange Managed API to produce a non-expanded view of Sadie's calendar.</span></span> 
  
```cs
PropertySet propSet = new PropertySet(AppointmentSchema.Subject,
                                      AppointmentSchema.Location,
                                      AppointmentSchema.Start, 
                                      AppointmentSchema.End,
                                      AppointmentSchema.AppointmentType);
#region FindItems + ItemView method
ItemView itemView = new ItemView(100);
itemView.PropertySet = propSet;
List<SearchFilter> filterList = new List<SearchFilter>();
// Find appointments that start after midnight on July 1, 2014.
SearchFilter.IsGreaterThan startFilter = new SearchFilter.IsGreaterThan(AppointmentSchema.Start,
    new DateTime(2014, 7, 1));
// Find appointments that end before midnight on July 31, 2014
SearchFilter.IsLessThan endFilter = new SearchFilter.IsLessThan(AppointmentSchema.End,
    new DateTime(2014, 7, 31));
filterList.Add(startFilter);
filterList.Add(endFilter);
SearchFilter.SearchFilterCollection calendarFilter = new SearchFilter.SearchFilterCollection(LogicalOperator.And, filterList);
// This results in a call to EWS.
FindItemsResults<Item> results = service.FindItems(WellKnownFolderName.Calendar, calendarFilter, itemView);
foreach(Item appt in results.Items)
{
    Console.WriteLine(appt.Subject);
}
```

<span data-ttu-id="4097e-207">Ce code génère la demande d' [opération FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) suivante avec un élément [IndexedPageItemView](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="4097e-207">That code results in the following [FindItem operation](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) request with an [IndexedPageItemView](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) element.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Pacific Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="calendar:Location" />
          <t:FieldURI FieldURI="calendar:Start" />
          <t:FieldURI FieldURI="calendar:End" />
          <t:FieldURI FieldURI="calendar:CalendarItemType" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="100" Offset="0" BasePoint="Beginning" />
      <m:Restriction>
        <t:And>
          <t:IsGreaterThan>
            <t:FieldURI FieldURI="calendar:Start" />
            <t:FieldURIOrConstant>
              <t:Constant Value="2014-07-01T07:00:00.000Z" />
            </t:FieldURIOrConstant>
          </t:IsGreaterThan>
          <t:IsLessThan>
            <t:FieldURI FieldURI="calendar:End" />
            <t:FieldURIOrConstant>
              <t:Constant Value="2014-07-31T07:00:00.000Z" />
            </t:FieldURIOrConstant>
          </t:IsLessThan>
        </t:And>
      </m:Restriction>
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="calendar" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="4097e-208">La réponse du serveur inclut un seul élément, la forme de base périodique, indiquée par la valeur de l’élément [CalendarItemType](https://msdn.microsoft.com/library/1feb0788-adf7-4a7c-830c-005214ad930f%28Office.15%29.aspx) de **RecurringMaster**.</span><span class="sxs-lookup"><span data-stu-id="4097e-208">The server's response includes only a single item, the recurring master, indicated by the [CalendarItemType](https://msdn.microsoft.com/library/1feb0788-adf7-4a7c-830c-005214ad930f%28Office.15%29.aspx) element value of **RecurringMaster**.</span></span> <span data-ttu-id="4097e-209">La valeur de l’élément [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) a été raccourcie pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="4097e-209">The value of the [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) element has been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="939" MinorBuildNumber="16" Version="V2_11" 
        xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="1" TotalItemsInView="1" IncludesLastItemInRange="true">
            <t:Items>
              <t:CalendarItem>
                <t:ItemId Id="AAMkADA5..." ChangeKey="DwAAABYA..." />
                <t:Subject>Swim Team Practice</t:Subject>
                <t:Start>2014-07-02T15:30:00Z</t:Start>
                <t:End>2014-07-02T17:00:00Z</t:End>
                <t:Location>Neighborhood Swimming Pool</t:Location>
                <t:CalendarItemType>RecurringMaster</t:CalendarItemType>
              </t:CalendarItem>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="4097e-210">Nous allons maintenant comparer avec un affichage développé.</span><span class="sxs-lookup"><span data-stu-id="4097e-210">Now let's compare with an expanded view.</span></span> <span data-ttu-id="4097e-211">L’exemple de code suivant utilise la méthode **findappointmentspour** dans l’API managée EWS pour créer un affichage développé du calendrier de Sadie.</span><span class="sxs-lookup"><span data-stu-id="4097e-211">The following code example uses the **FindAppointments** method in the EWS Managed API to create an expanded view of Sadie's calendar.</span></span> 
  
```cs
PropertySet propSet = new PropertySet(AppointmentSchema.Subject,
                                      AppointmentSchema.Location,
                                      AppointmentSchema.Start, 
                                      AppointmentSchema.End,
                                      AppointmentSchema.AppointmentType);
CalendarView calView = new CalendarView(new DateTime(2014, 7, 1),
    new DateTime(2014, 7, 31));
calView.PropertySet = propSet;
FindItemsResults<Appointment> results = service.FindAppointments(WellKnownFolderName.Calendar, calView);
foreach(Appointment appt in results.Items)
{
    Console.WriteLine(appt.Subject);
}
```

<span data-ttu-id="4097e-212">Ce code génère la demande d' [opération FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) suivante avec un élément [CalendarView](https://msdn.microsoft.com/library/a4a953b8-0710-416c-95ef-59e51eba9982%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="4097e-212">This code results in the following [FindItem operation](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) request with a [CalendarView](https://msdn.microsoft.com/library/a4a953b8-0710-416c-95ef-59e51eba9982%28Office.15%29.aspx) element.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Pacific Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="calendar:Location" />
          <t:FieldURI FieldURI="calendar:Start" />
          <t:FieldURI FieldURI="calendar:End" />
          <t:FieldURI FieldURI="calendar:CalendarItemType" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:CalendarView StartDate="2014-07-01T07:00:00.000Z" EndDate="2014-07-31T07:00:00.000Z" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="calendar" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="4097e-213">Cette fois-ci, la réponse du serveur inclut cinq occurrences, une pour chaque mercredi en juillet.</span><span class="sxs-lookup"><span data-stu-id="4097e-213">This time, the server response includes five occurrences, one for each Wednesday in July.</span></span> <span data-ttu-id="4097e-214">Les éléments [CalendarItemType](https://msdn.microsoft.com/library/1feb0788-adf7-4a7c-830c-005214ad930f%28Office.15%29.aspx) de ces éléments ont tous la valeur **occurrence**.</span><span class="sxs-lookup"><span data-stu-id="4097e-214">The [CalendarItemType](https://msdn.microsoft.com/library/1feb0788-adf7-4a7c-830c-005214ad930f%28Office.15%29.aspx) elements on these items all have a value of **Occurrence**.</span></span> <span data-ttu-id="4097e-215">Notez que le masque périodique n’est pas présent dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="4097e-215">Note that the recurring master is not present in the response.</span></span> <span data-ttu-id="4097e-216">Les valeurs des éléments [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) ont été raccourcies pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="4097e-216">The values of the [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="939" MinorBuildNumber="16" Version="V2_11" 
        xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder TotalItemsInView="5" IncludesLastItemInRange="true">
            <t:Items>
              <t:CalendarItem>
                <t:ItemId Id="AAMkADA6..." ChangeKey="DwAAABYA..." />
                <t:Subject>Swim Team Practice</t:Subject>
                <t:Start>2014-07-02T15:30:00Z</t:Start>
                <t:End>2014-07-02T17:00:00Z</t:End>
                <t:Location>Neighborhood Swimming Pool</t:Location>
                <t:CalendarItemType>Occurrence</t:CalendarItemType>
              </t:CalendarItem>
              <t:CalendarItem>
                <t:ItemId Id="AAMkADA7..." ChangeKey="DwAAABYA..." />
                <t:Subject>Swim Team Practice</t:Subject>
                <t:Start>2014-07-09T15:30:00Z</t:Start>
                <t:End>2014-07-09T17:00:00Z</t:End>
                <t:Location>Neighborhood Swimming Pool</t:Location>
                <t:CalendarItemType>Occurrence</t:CalendarItemType>
              </t:CalendarItem>
              <t:CalendarItem>
                <t:ItemId Id="AAMkADA8..." ChangeKey="DwAAABYA..." />
                <t:Subject>Swim Team Practice</t:Subject>
                <t:Start>2014-07-16T15:30:00Z</t:Start>
                <t:End>2014-07-16T17:00:00Z</t:End>
                <t:Location>Neighborhood Swimming Pool</t:Location>
                <t:CalendarItemType>Occurrence</t:CalendarItemType>
              </t:CalendarItem>
              <t:CalendarItem>
                <t:ItemId Id="AAMkADA9..." ChangeKey="DwAAABYA..." />
                <t:Subject>Swim Team Practice</t:Subject>
                <t:Start>2014-07-23T15:30:00Z</t:Start>
                <t:End>2014-07-23T17:00:00Z</t:End>
                <t:Location>Neighborhood Swimming Pool</t:Location>
                <t:CalendarItemType>Occurrence</t:CalendarItemType>
              </t:CalendarItem>
              <t:CalendarItem>
                <t:ItemId Id="AAMkADAA..." ChangeKey="DwAAABYA..." />
                <t:Subject>Swim Team Practice</t:Subject>
                <t:Start>2014-07-30T15:30:00Z</t:Start>
                <t:End>2014-07-30T17:00:00Z</t:End>
                <t:Location>Neighborhood Swimming Pool</t:Location>
                <t:CalendarItemType>Occurrence</t:CalendarItemType>
              </t:CalendarItem>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="4097e-217">Une fois que vous disposez d’une page maître périodique, d’une occurrence ou d’une exception, vous pouvez toujours [récupérer les autres éléments associés](how-to-access-a-recurring-series-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="4097e-217">After you have a recurring master, an occurrence, or an exception, you can always [retrieve the other related items](how-to-access-a-recurring-series-by-using-ews-in-exchange.md).</span></span> <span data-ttu-id="4097e-218">Étant donné une occurrence ou une exception, vous pouvez récupérer la forme de base périodique, et inversement.</span><span class="sxs-lookup"><span data-stu-id="4097e-218">Given an occurrence or exception, you can retrieve the recurring master, and vice versa.</span></span>
  
## <a name="working-with-recurring-calendar-items"></a><span data-ttu-id="4097e-219">Utilisation d’éléments de calendrier périodiques</span><span class="sxs-lookup"><span data-stu-id="4097e-219">Working with recurring calendar items</span></span>

<span data-ttu-id="4097e-220">Vous utilisez toutes les mêmes méthodes et opérations pour utiliser les séries périodiques que pour utiliser des éléments de calendrier non périodiques.</span><span class="sxs-lookup"><span data-stu-id="4097e-220">You use all the same methods and operations to work with recurring series as you use to work with non-recurring calendar items.</span></span> <span data-ttu-id="4097e-221">La différence réside dans le fait que, en fonction de l’élément que vous utilisez pour appeler ces méthodes ou opérations, les actions que vous prenez peuvent s’appliquer à la série entière ou à une seule occurrence.</span><span class="sxs-lookup"><span data-stu-id="4097e-221">The difference is that, depending on the item you use to invoke those methods or operations, the actions you take can apply to the entire series, or just a single occurrence.</span></span> <span data-ttu-id="4097e-222">Les [actions effectuées sur la forme de base périodique](how-to-update-a-recurring-series-by-using-ews-in-exchange.md) s’appliqueront à toutes les occurrences de la série, tandis que les [actions effectuées pour une seule occurrence ou exception](how-to-update-a-recurring-series-by-using-ews.md) ne s’appliqueront qu’à cette occurrence ou exception.</span><span class="sxs-lookup"><span data-stu-id="4097e-222">[Actions taken on the recurring master](how-to-update-a-recurring-series-by-using-ews-in-exchange.md) will apply to all occurrences in the series, while [actions taken to a single occurrence or exception](how-to-update-a-recurring-series-by-using-ews.md) will only apply to that occurrence or exception.</span></span> 
  
## <a name="in-this-section"></a><span data-ttu-id="4097e-223">Dans cette section</span><span class="sxs-lookup"><span data-stu-id="4097e-223">In this section</span></span>

- [<span data-ttu-id="4097e-224">Accéder à une série périodique à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="4097e-224">Access a recurring series by using EWS in Exchange</span></span>](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="4097e-225">Créer une série périodique à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="4097e-225">Create a recurring series by using EWS in Exchange</span></span>](how-to-create-a-recurring-series-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="4097e-226">Supprimer des rendez-vous dans une série périodique à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="4097e-226">Delete appointments in a recurring series by using EWS in Exchange</span></span>](how-to-delete-appointments-in-a-recurring-series-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="4097e-227">Mettre à jour une série périodique à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="4097e-227">Update a recurring series by using EWS</span></span>](how-to-update-a-recurring-series-by-using-ews.md)
    
- [<span data-ttu-id="4097e-228">Mettre à jour une série périodique à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="4097e-228">Update a recurring series by using EWS in Exchange</span></span>](how-to-update-a-recurring-series-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="4097e-229">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4097e-229">See also</span></span>


- [<span data-ttu-id="4097e-230">Calendriers et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="4097e-230">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)
    
- [<span data-ttu-id="4097e-231">Développer des clients de service web pour Exchange</span><span class="sxs-lookup"><span data-stu-id="4097e-231">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    
- [<span data-ttu-id="4097e-232">Créer des rendez-vous et des réunions à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="4097e-232">Get appointments and meetings by using EWS in Exchange</span></span>](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)
    


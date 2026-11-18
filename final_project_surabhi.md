| [home page](./) | [data viz examples](dataviz-examples) | [critique by design](critique-by-design) | [final project I](final-project-part-one) | [final project II](final-project-part-two) | [final project III](final-project-part-three) | [final project I (Surabhi)](final_project_surabhi) |

[&larr; Back to main portfolio](./#portfolio)

# Final Project Part I

**Status: In progress.** The sketch images are placeholders that I will replace as they become available.

## Which U.S. Gateway Best Connects India to Pittsburgh?

**One-sentence summary:** This project examines which U.S. gateway provides travelers from India with the strongest potential connection to Pittsburgh by comparing international flight availability with onward service to Pittsburgh.

## Audience

The primary audience is travelers planning a journey from India to Pittsburgh, particularly students, families, professionals, and visitors who must connect through another U.S. airport. The project may also help travel planners understand which gateways provide the greatest range of potential flight options.

## User Story

As a traveler flying from India to Pittsburgh, I want to compare major U.S. connecting airports so that I can select a gateway with strong service on both parts of my journey. I can do this by comparing flights from India to each gateway with the frequency and capacity of onward flights from that gateway to Pittsburgh.

## Why This Matters

Travelers may choose a connection based on the availability of the first flight from India without considering the frequency of onward flights to Pittsburgh. A gateway with extensive India service may still offer relatively limited Pittsburgh service.

By examining both segments of the journey, this project will help readers understand that the strongest gateway is not necessarily the airport with the most international arrivals. The best potential gateway should provide a useful balance between India service and onward Pittsburgh connectivity.

## Project Summary

Traveling from India to Pittsburgh typically requires a connection through another U.S. airport. Travelers can enter the United States through gateways such as New York–JFK, Newark, Chicago, Washington–Dulles, or San Francisco. However, these airports differ in both the amount of service they receive from India and the availability of onward flights to Pittsburgh.

This project will compare major gateways using 2025 flight-segment data from the U.S. Department of Transportation. It will examine flight frequency, passenger volume, seat capacity, Indian cities served, airlines, and monthly availability. The objective is to identify which gateway offers the strongest potential connectivity based on the balance between India-to-gateway service and gateway-to-Pittsburgh service.

## Central Message

> The airport with the most flights from India is not automatically the strongest gateway to Pittsburgh. Travelers should evaluate both parts of the journey.

**Preliminary finding:** Early analysis suggests that Newark Liberty International Airport (EWR) may provide the strongest overall balance between India service and onward Pittsburgh service. This is a preliminary finding only, and it will be tested in the final analysis.

## Project Structure and Story Arc

1. **Opening: the traveler's problem**
    - Pittsburgh does not currently have nonstop service from India.
    - Travelers must connect through another U.S. airport.
    - The selected gateway affects the number of potential onward options.

2. **Build-up: how India connects to the United States**
    - Show where flights from Delhi, Mumbai, and Bengaluru arrive.
    - Compare flights, passengers, seats, airlines, and monthly availability.
    - Demonstrate that gateways differ considerably in India service.

3. **Turning point: the first flight is only half the journey**
    - Introduce onward service from each gateway to Pittsburgh.
    - Show that airports with substantial India service do not always have the greatest Pittsburgh frequency.
    - Compare both segments together.

4. **Resolution: finding the strongest balance**
    - Compare JFK, EWR, ORD, SFO, and IAD.
    - Explain the trade-offs associated with each airport.
    - Identify the gateway with the strongest potential connectivity.

5. **Call to action**
    - Before booking an India-to-Pittsburgh journey, compare both legs of the route and prioritize a gateway that provides strong international access and frequent onward service to Pittsburgh.

> **"Choose your gateway based on the whole journey—not just the first flight."**

## Initial Sketches

The sketches below are planned views for the story. Each placeholder will be replaced with an exported sketch image.

<!-- To add sketch images: save the exported files in images/final-project/ using the filenames listed under each sketch, then replace the placeholder text with an image reference such as ![descriptive alt text](images/final-project/sketch-1-journey-introduction.png). Do not add the image reference until the file exists, so the published page has no broken images. -->

### Prototype 1: Where Do Flights from India Enter the United States?

_Initial Tableau prototype, not a final visualization._

<div id="viz-india-gateways" style="width: 100%; max-width: 1100px; height: 420px; min-height: 340px; margin: 0 auto; overflow: hidden;">
  <iframe title="Initial Tableau prototype: bar chart of flights performed from India to five U.S. gateways in 2025, with New York-JFK highest at 1,028 and Washington-Dulles lowest at 109." src="https://public.tableau.com/views/FinalProject-sheet1_17950177411830/IndiatoU_S_Gateways?:showVizHome=no&amp;:embed=true" width="100%" height="100%" style="border: 0; display: block; width: 100%; height: 100%;" loading="lazy" allowfullscreen></iframe>
</div>

<p style="text-align: center;">
  <a href="https://public.tableau.com/app/profile/surabhi.byju/viz/FinalProject-sheet1_17950177411830/IndiatoU_S_Gateways?publish=yes" target="_blank" rel="noopener noreferrer">Open the interactive visualization on Tableau Public</a>
</p>

This initial Tableau prototype compares the number of scheduled passenger flights performed from India to five U.S. gateways that also provide onward service to Pittsburgh. JFK received the greatest number of India-originating flights in 2025, followed by San Francisco and Newark. However, this view represents only the first portion of the journey and does not yet show the strength of onward service to Pittsburgh.

**Intended takeaway:** The gateway receiving the most flights from India is not automatically the gateway offering the strongest complete connection to Pittsburgh.

### Prototype 2: Which Gateways Provide the Most Onward Flights to Pittsburgh?

_Initial Tableau prototype, not a final visualization._

<div id="viz-gateways-to-pittsburgh" style="width: 100%; max-width: 1100px; height: 420px; min-height: 340px; margin: 0 auto; overflow: hidden;">
  <iframe title="Initial Tableau prototype: bar chart of scheduled passenger flights performed from five U.S. gateways to Pittsburgh in 2025, with Chicago-O'Hare highest." src="https://public.tableau.com/views/FinalProject-sheet2_17950182342380/U_S_GatewaystoPittsburgh?:showVizHome=no&amp;:embed=true" width="100%" height="100%" style="border: 0; display: block; width: 100%; height: 100%;" loading="lazy" allowfullscreen></iframe>
</div>

<p style="text-align: center;">
  <a href="https://public.tableau.com/app/profile/surabhi.byju/viz/FinalProject-sheet2_17950182342380/U_S_GatewaystoPittsburgh?publish=yes" target="_blank" rel="noopener noreferrer">Open Prototype 2 on Tableau Public</a>
</p>

This initial Tableau prototype compares the number of scheduled passenger flights performed from five U.S. gateways to Pittsburgh in 2025. Chicago–O’Hare provided the most onward flights to Pittsburgh, followed by Newark and New York–JFK. This differs from the first visualization, where JFK received the most flights from India.

**Intended takeaway:** The airport receiving the most flights from India is not the same airport providing the most onward flights to Pittsburgh. Travelers therefore need to consider both parts of the journey.

### Prototype 3: Which Gateway Offers the Strongest Balance?

_Initial Tableau prototype, not a final visualization._

<div id="viz-gateway-balance" style="width: 100%; max-width: 1100px; height: 420px; min-height: 340px; margin: 0 auto; overflow: hidden;">
  <iframe title="Initial Tableau prototype: scatterplot comparing flights from India to each of five U.S. gateways on the horizontal axis with flights from each gateway to Pittsburgh on the vertical axis, with reference lines showing the average service levels." src="https://public.tableau.com/views/FinalProject-sheet3_17950200670440/GatewayBalance?:showVizHome=no&amp;:embed=true" width="100%" height="100%" style="border: 0; display: block; width: 100%; height: 100%;" loading="lazy" allowfullscreen></iframe>
</div>

<p style="text-align: center;">
  <a href="https://public.tableau.com/app/profile/surabhi.byju/viz/FinalProject-sheet3_17950200670440/GatewayBalance?publish=yes" target="_blank" rel="noopener noreferrer">Open Prototype 3 on Tableau Public</a>
</p>

This scatterplot compares both parts of the journey simultaneously. The horizontal axis represents flights from India to each gateway, while the vertical axis represents flights from that gateway to Pittsburgh. The reference lines show the average service levels among the five selected gateways.

**Intended takeaway:** No gateway leads both parts of the journey. JFK provides the most India service, Chicago–O’Hare provides the most Pittsburgh service, and Newark offers one of the strongest balances between the two measures.

The visualization measures potential flight connectivity rather than actual passenger connections. It does not show whether passengers arriving from India continued to Pittsburgh.

### Prototype 4: How Consistent Is India Service Across the Year?

_Initial Tableau prototype, not a final visualization._

<div id="viz-monthly-india-service" style="width: 100%; max-width: 1100px; height: 420px; min-height: 340px; margin: 0 auto; overflow: hidden;">
  <iframe title="Initial Tableau prototype: heatmap of monthly flights performed from India to five U.S. gateways in 2025. New York-JFK, San Francisco, and Newark have service in every month, while Chicago-O'Hare and Washington-Dulles have months without service." src="https://public.tableau.com/views/FinalProject-sheet4_17950338217190/MonthlyIndiaService?:showVizHome=no&amp;:embed=true" width="100%" height="100%" style="border: 0; display: block; width: 100%; height: 100%;" loading="lazy" allowfullscreen></iframe>
</div>

<p style="text-align: center;">
  <a href="https://public.tableau.com/app/profile/surabhi.byju/viz/FinalProject-sheet4_17950338217190/MonthlyIndiaService?publish=yes" target="_blank" rel="noopener noreferrer">Open Prototype 4 on Tableau Public</a>
</p>

This initial Tableau prototype is a heatmap of the number of scheduled passenger flights performed from India to each of the five gateways in every month of 2025, with darker cells indicating more flights. JFK, San Francisco, and Newark received India service in all twelve months. Chicago–O’Hare had no India service in June and July, and Washington–Dulles had service in only six months.

**Intended takeaway:** Some gateways offer consistent year-round service while others have limited or seasonal service.

## The Data

This project will use the Bureau of Transportation Statistics T-100 Segment (All Carriers) dataset published by the U.S. Department of Transportation. The downloaded file contains monthly flight-segment records for 2025, including domestic and international service. Relevant fields include origin and destination airports, countries, airlines, flights performed, seats, passengers, distance, air time, year, and month.

The analysis will first identify passenger flights traveling from India to U.S. gateway airports. It will then identify flights from those gateways to Pittsburgh International Airport. The two groups will be aggregated by airport and month to compare international access with onward Pittsburgh connectivity. Because the dataset records flight segments rather than complete passenger itineraries, the project will describe potential connectivity and will not claim that individual passengers continued from India to Pittsburgh.

### Dataset information

<div style="overflow-x: auto;" markdown="1">

| Item | Detail |
|------|--------|
| Dataset | T-100 Segment (All Carriers) |
| Publisher | U.S. Department of Transportation, Bureau of Transportation Statistics |
| Time period | January–December 2025 |
| Geographic scope | India-to-United States and United States-to-Pittsburgh flight segments |
| Unit of analysis | Aggregated flight-segment records |
| Date accessed | November 18, 2026 |
| Public dataset link | <a href="https://transtats.bts.gov/Fields.asp?QO_fu146_anzr=Nv4+Pn44vr45&amp;gnoyr_VQ=FMG" target="_blank" rel="noopener noreferrer">BTS T-100 Segment (All Carriers) data page</a> |

</div>

### Planned filters

<div style="overflow-x: auto;" markdown="1">

| Journey segment | Planned filter |
|-----------------|----------------|
| India to U.S. gateway | Origin country = India and destination country = United States |
| Gateway to Pittsburgh | Origin country = United States and destination airport = PIT |
| Service type | Scheduled passenger service, CLASS = F |
| Activity requirement | DEPARTURES_PERFORMED greater than 0 |
| Time period | January–December 2025 |
| Main gateways | JFK, EWR, ORD, SFO, and IAD |

</div>

`DEPARTURES_PERFORMED` will be used as the main flight-frequency measure because `DEPARTURES_SCHEDULED` is missing or recorded as zero for some international carrier records.

### Preliminary data coverage

<div style="overflow-x: auto;" markdown="1">

| Gateway | India-to-gateway flights | Gateway-to-PIT flights | Months with India service |
|---------|--------------------------|------------------------|---------------------------|
| JFK | 1,028 | 2,047 | 12 |
| SFO | 804 | 580 | 12 |
| EWR | 727 | 2,269 | 12 |
| ORD | 231 | 3,690 | 10 |
| IAD | 109 | 1,479 | 6 |

</div>

BOS and PHL were excluded from the main comparison because the dataset contains only a very small number of India-originating flights for these gateways.

## Limitations

The T-100 dataset contains aggregated flight-segment information rather than individual passenger itineraries. It cannot determine how many passengers arriving from India continued to Pittsburgh. It also does not contain ticket prices, immigration waiting times, terminal transfers, baggage-transfer experiences, scheduled connection times, or missed connections.

Therefore, the final recommendation will concern flight availability, capacity, and potential connectivity rather than the complete passenger experience. This project will not describe any gateway as the cheapest, fastest, easiest, or least stressful unless another appropriate dataset is added later.

## Method and Medium

The final project will be presented as an interactive narrative using Shorthand, with visualizations created in Tableau. Tableau will be used to aggregate and compare gateway airports, create interactive charts, and allow readers to examine different Indian departure cities and months.

Shorthand will organize the visualizations into a guided story that introduces the travel problem, compares the two journey segments, presents gateway trade-offs, and concludes with a practical recommendation.

## References

U.S. Department of Transportation, Bureau of Transportation Statistics. *T-100 Segment (All Carriers), 2025.* Accessed November 18, 2026. <a href="https://transtats.bts.gov/Fields.asp?QO_fu146_anzr=Nv4+Pn44vr45&amp;gnoyr_VQ=FMG" target="_blank" rel="noopener noreferrer">https://transtats.bts.gov/Fields.asp?QO_fu146_anzr=Nv4+Pn44vr45&amp;gnoyr_VQ=FMG</a>

## AI acknowledgements

I used ChatGPT to help refine the project topic, evaluate the suitability of the dataset, and develop the preliminary story structure. I used Kiro to help implement and check the Markdown page structure and navigation. I reviewed and revised all generated material and remain responsible for the final analysis, design, and conclusions.

---

| [&larr; back to main portfolio](./#portfolio) | [home page](./) | [data viz examples](dataviz-examples) | [critique by design](critique-by-design) | [final project II](final-project-part-two) | [final project III](final-project-part-three) |

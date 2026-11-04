| [home page](./) | [data viz examples](dataviz-examples) | [critique by design](critique-by-design) | [final project I](final-project-part-one) | [final project II](final-project-part-two) | [final project III](final-project-part-three) |

# Data Visualization Examples

This page collects data visualizations I built for the course. Each embed below is interactive; if a visualization does not load, use the direct link to open it on Tableau Public.

---

## Government Debt Map, 2023

**Interactive filled map of government gross debt as a percentage of GDP.**
[Open on Tableau Public](https://public.tableau.com/app/profile/surabhi.byju/viz/OECD_Government_Debt_2007_2024/GovernmentDebtMap2023)

<div class='tableauPlaceholder' id='viz-debt-map' style='position: relative; width: 100%; max-width: 1000px; margin: 0 auto;'>
  <noscript>
    <a href='https://public.tableau.com/app/profile/surabhi.byju/viz/OECD_Government_Debt_2007_2024/GovernmentDebtMap2023'>
      <img alt='Government Debt Map 2023' src='https://public.tableau.com/static/images/OE/OECD_Government_Debt_2007_2024/GovernmentDebtMap2023/1_rss.png' style='border: none' />
    </a>
  </noscript>
  <object class='tableauViz' style='display:none;'>
    <param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' />
    <param name='embed_code_version' value='3' />
    <param name='site_root' value='' />
    <param name='name' value='OECD_Government_Debt_2007_2024&#47;GovernmentDebtMap2023' />
    <param name='tabs' value='no' />
    <param name='toolbar' value='yes' />
    <param name='static_image' value='https://public.tableau.com/static/images/OE/OECD_Government_Debt_2007_2024/GovernmentDebtMap2023/1.png' />
    <param name='animate_transition' value='yes' />
    <param name='display_static_image' value='yes' />
    <param name='display_spinner' value='yes' />
    <param name='display_overlay' value='yes' />
    <param name='display_count' value='yes' />
    <param name='language' value='en-US' />
  </object>
</div>

For my redesigned visualization, I created an interactive filled map showing government gross debt as a percentage of GDP. The map defaults to 2023, but viewers can use the year filter to explore how the geographic distribution of government debt changed from 2007 through 2024. I selected 2023 as the default because it is a recent year with observations available for a substantial number of countries.

I used the `Ref Area` field, which contains three-letter country codes, and assigned it the Country/Region geographic role in Tableau. I excluded `OECD`, `OECD_REP`, and `EUOECD` because they represent aggregate groups rather than individual countries. Countries without an observation for the selected year are left uncolored rather than being represented as having zero debt.

I used a sequential blue color palette in which lighter shades represent lower government debt and darker shades represent higher debt. This provides a consistent visual hierarchy and allows countries with particularly high debt levels to stand out without introducing unrelated colors. The tooltip displays the country name, selected year, and government gross debt as a percentage of GDP.

In 2023, Japan had the highest government debt among the displayed countries at approximately 228.1% of GDP, followed by Greece at approximately 180.2% and Italy at approximately 148.2%. The map is more effective than the Part 2 highlight table for identifying geographic patterns and comparing countries in a selected year. However, the highlight table is more effective for examining changes across the full 2007–2024 period. The visualizations therefore serve complementary purposes: the map provides an interactive geographic comparison, while the highlight table provides greater historical context.

---

## Debt-to-GDP Highlight Table (Heatmap)

**Highlight table showing government gross debt as a percentage of GDP across years.**
[Open on Tableau Public](https://public.tableau.com/app/profile/surabhi.byju/viz/OECD_Government_Debt_2007_2024/Debt-to-GDPHighlightTable)

<div class='tableauPlaceholder' id='viz-debt-table' style='position: relative; width: 100%; max-width: 1000px; margin: 0 auto;'>
  <noscript>
    <a href='https://public.tableau.com/app/profile/surabhi.byju/viz/OECD_Government_Debt_2007_2024/Debt-to-GDPHighlightTable'>
      <img alt='Debt-to-GDP Highlight Table' src='https://public.tableau.com/static/images/OE/OECD_Government_Debt_2007_2024/Debt-to-GDPHighlightTable/1_rss.png' style='border: none' />
    </a>
  </noscript>
  <object class='tableauViz' style='display:none;'>
    <param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' />
    <param name='embed_code_version' value='3' />
    <param name='site_root' value='' />
    <param name='name' value='OECD_Government_Debt_2007_2024&#47;Debt-to-GDPHighlightTable' />
    <param name='tabs' value='no' />
    <param name='toolbar' value='yes' />
    <param name='static_image' value='https://public.tableau.com/static/images/OE/OECD_Government_Debt_2007_2024/Debt-to-GDPHighlightTable/1.png' />
    <param name='animate_transition' value='yes' />
    <param name='display_static_image' value='yes' />
    <param name='display_spinner' value='yes' />
    <param name='display_overlay' value='yes' />
    <param name='display_count' value='yes' />
    <param name='language' value='en-US' />
  </object>
</div>

The highlight table encodes government gross debt as a percentage of GDP across the full 2007–2024 period, making it well suited for tracking how individual countries' debt levels evolved over time. Read alongside the map above, it provides the historical context that a single-year geographic view cannot.

---

## References

Organisation for Economic Co-operation and Development. "Government Gross Debt." OECD Data. Government gross debt as a percentage of GDP, general government sector. <https://data.oecd.org/>

## AI Acknowledgements

I used ChatGPT to help troubleshoot Tableau errors and warnings. I used an AI assistant (Kiro) to help embed the finished Tableau Public visualizations into this portfolio page. The analysis, data preparation, design decisions, and written interpretations are my own.

<script type='text/javascript'>
  var divElements = document.getElementsByClassName('tableauPlaceholder');
  for (var i = 0; i < divElements.length; i++) {
    var divElement = divElements[i];
    var vizElement = divElement.getElementsByTagName('object')[0];
    vizElement.style.width = '100%';
    vizElement.style.height = (divElement.offsetWidth * 0.75) + 'px';
    var scriptElement = document.createElement('script');
    scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';
    vizElement.parentNode.insertBefore(scriptElement, vizElement);
  }
</script>

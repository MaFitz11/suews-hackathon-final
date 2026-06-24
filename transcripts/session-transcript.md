# SUEWS Hackathon Research Session Transcript

**Student:** Marina Fitzner  
**Lecturer/audience:** Dr. Ting Sun  
**Repository:** https://github.com/MaFitz11/suews-hackathon-final  
**Published site:** https://mafitz11.github.io/suews-hackathon-final/  
**Date:** 24 June 2026

## Purpose

This transcript records the main setup, modelling, analysis, interpretation, and communication steps carried out during the SUEWS Community Hackathon work session. It is written as a clear research-process record rather than as a verbatim chat export, so that the work can be reviewed without needing access to the original assistant conversation.

## 1. Repository and task setup

The public GitHub repository `MaFitz11/suews-hackathon-final` was created from the template repository `UMEP-dev/suews-hackathon-template`.

The task brief was read and interpreted as a neighbourhood-scale urban heat and vulnerability analysis. The working research goal became:

> Use the UDA-city SUEWS dataset to compare current and future heat exposure, identify socio-economic vulnerability patterns, and design a constrained but more equitable heat-adaptation scenario.

The public GitHub Pages site was configured from the `docs/` folder on the `main` branch.

## 2. Data exploration

The UDA-city hackathon data were explored. The dataset represents a synthetic hot-humid city with multiple neighbourhoods. The city is not a real municipality, which is important for interpretation: the work demonstrates a method and adaptation logic, not a direct policy prescription for a real place.

Neighbourhoods used in the analysis included:

- Jade Gardens
- Serendib Rise
- Taman Melati
- Kampong Lama
- Dhobi Lines
- Lusitano Square
- Mlima Moto
- Victoria Exchange
- Fuzhou Lanes
- Zheng He Towers

Neighbourhood types included refuge, hotspot, and core areas. The hotspot areas were especially important for the heat-vulnerability interpretation.

## 3. Key heat metric

The main urban climate metric selected for the research story was:

> Number of hours where 2 m air temperature, T2, is greater than 35 C.

This metric was chosen because it is easy to communicate, directly linked to dangerous heat exposure, and can be compared across neighbourhoods.

The term `2 m air temperature` was interpreted as the standard meteorological near-surface air temperature measured or modelled at approximately 2 metres above ground level, roughly the height relevant to human outdoor exposure.

## 4. Spin-up period

A spin-up period was discussed before running the simulations. In urban climate modelling, a spin-up period allows the model state, especially surface and storage variables, to settle before the analysis period is counted. This avoids interpreting early model adjustment artefacts as real results.

For the hottest-month analysis, a 30-day spin-up was used before analysing April-May heat exposure.

## 5. Present and future SUEWS simulations

SUEWS simulations were run for the present and future scenarios. The analysis focused on the hottest available months in the dataset.

The dangerous heat-hour results showed that future heat exposure increases strongly in every neighbourhood.

| Neighbourhood | Type | Present T2 > 35 C hours | Future T2 > 35 C hours | Increase |
|---|---:|---:|---:|---:|
| Jade Gardens | refuge | 26 | 169 | +143 |
| Kampong Lama | hotspot | 24 | 163 | +139 |
| Taman Melati | refuge | 21 | 153 | +132 |
| Dhobi Lines | hotspot | 15 | 141 | +126 |
| Fuzhou Lanes | hotspot | 13 | 136 | +123 |
| Serendib Rise | refuge | 9 | 123 | +114 |
| Mlima Moto | hotspot | 1 | 91 | +90 |
| Lusitano Square | core | 1 | 72 | +71 |
| Victoria Exchange | core | 1 | 66 | +65 |
| Zheng He Towers | core | 0 | 45 | +45 |

Main interpretation:

- The future scenario produces a major increase in dangerous heat exposure.
- The increase is citywide, but the burden is not spatially equal.
- Several high-exposure neighbourhoods also have social vulnerability signals, making the issue one of heat justice, not only climate warming.

## 6. Socio-economic heat vulnerability indicators

The PreventionWeb Extreme Heat Portal and UNDRR-style risk framing were used to guide the selection of socio-economic vulnerability indicators. The selected local heat-vulnerability subvariables were:

- Lack of AC / cooling access
- Outdoor work
- Deprivation
- Young children
- Older adults

These indicators were adjusted to the local characteristics of UDA-city, especially the distinction between hotspot, refuge, and core neighbourhoods.

| Neighbourhood | Lack of cooling access (%) | Outdoor work (%) | Deprivation (%) | Young children (%) | Older adults (%) |
|---|---:|---:|---:|---:|---:|
| Jade Gardens | 55 | 30 | 40 | 9 | 10 |
| Serendib Rise | 50 | 28 | 38 | 8 | 11 |
| Taman Melati | 58 | 32 | 42 | 9 | 10 |
| Kampong Lama | 92 | 62 | 82 | 13 | 7 |
| Dhobi Lines | 90 | 60 | 80 | 12 | 8 |
| Lusitano Square | 30 | 22 | 30 | 7 | 13 |
| Mlima Moto | 94 | 65 | 85 | 14 | 7 |
| Victoria Exchange | 28 | 20 | 28 | 6 | 14 |
| Fuzhou Lanes | 93 | 63 | 83 | 13 | 8 |
| Zheng He Towers | 22 | 18 | 25 | 6 | 15 |

Main interpretation:

- Hotspot neighbourhoods show the highest lack of cooling access, outdoor work, and deprivation.
- Core neighbourhoods generally show lower socio-economic vulnerability, although older-adult shares can be higher.
- Heat vulnerability is therefore concentrated where physical exposure and social sensitivity overlap.

## 7. Visualisations created during the process

The following charts were created and later included in the public story page:

1. Present vs future dangerous heat hours by neighbourhood.
2. Heatmap of socio-economic vulnerability subvariables by neighbourhood.
3. Grouped bar chart of main vulnerability drivers.
4. Future baseline vs greening/adaptation heat-hour comparison.
5. Targeted intervention risk-reduction chart.

The final website embeds these charts directly into `docs/index.html`, so they appear on the GitHub Pages site without requiring separate image hosting.

## 8. Adaptation scenario design

A constrained adaptation scenario was designed in response to the research question: how can UDA-city reduce heat vulnerability efficiently and more justly if resources are limited?

The constraints were:

- Only 20% of paved or bare-soil area across the whole city can be converted to evapotranspirative vegetation, grass, or water.
- Vehicle heat can only be reduced by 15%.
- AC / cooling access can only be increased by 50% citywide.

The intended strategy was not to distribute resources evenly. Instead, resources were targeted toward neighbourhoods where heat exposure and socio-economic vulnerability were highest.

## 9. Allocation logic

The allocation plan gave larger land-cover and cooling-access interventions to neighbourhoods with higher combined risk.

Examples:

- Kampong Lama received one of the largest combined supports because it has very high future heat exposure and high vulnerability.
- Dhobi Lines and Fuzhou Lanes also received strong targeted support because of high lack of cooling, high deprivation, and high outdoor work exposure.
- Mlima Moto received strong social adaptation support because of very high deprivation and outdoor work exposure.
- Lower-vulnerability neighbourhoods still received enough support to reach the minimum target of at least 5% risk-pressure reduction.

## 10. Adaptation scenario results

The targeted package achieved the intended justice-oriented pattern:

- Every neighbourhood reached at least a 5% risk-pressure reduction.
- The most vulnerable hotspot neighbourhoods received larger reductions.
- The citywide risk-pressure reduction was approximately 15.4%.

Selected results:

| Neighbourhood | Future baseline heat hours | Intervention heat hours | Risk-pressure reduction |
|---|---:|---:|---:|
| Kampong Lama | 163 | 157 | 19.6% |
| Dhobi Lines | 141 | 141 | 18.1% |
| Fuzhou Lanes | 136 | 138 | 17.8% |
| Mlima Moto | 91 | 94 | 13.8% |
| Jade Gardens | 169 | 162 | 5.0% |
| Taman Melati | 153 | 147 | 5.0% |
| Lusitano Square | 72 | 71 | 5.0% |
| Victoria Exchange | 66 | 69 | 5.0% |
| Serendib Rise | 123 | 119 | 5.0% |
| Zheng He Towers | 45 | 45 | 5.0% |

Important interpretation:

The physical land-cover intervention alone did not reduce dangerous heat hours everywhere. Some neighbourhoods showed little change or a small increase in T2 > 35 C hours. The stronger fairness result came from combining physical urban adaptation with targeted social cooling access.

## 11. Limitations

The final interpretation includes several limitations:

- UDA-city is synthetic, so the findings demonstrate a workflow rather than a direct real-world policy plan.
- The socio-economic vulnerability indicators are synthetic and should be replaced with local census, health, labour, and cooling-access data for real policy use.
- The future scenario is a hotter-climate stress test, not a full downscaled climate projection with uncertainty ranges.
- The social cooling-access calculation is a vulnerability-pressure analysis, not a direct indoor-health or mortality model.
- The current SUEWS configuration has anthropogenic heat set to zero, so the 15% vehicle-heat reduction could be discussed as a policy lever but was not credited as a physical model effect in the heat-hour results.

## 12. Final communication product

A public GitHub Pages story was created with the title:

> Targeted Cooling for a Hotter UDA-city

The story presents three scenarios:

1. Current climate.
2. Original hotter future scenario.
3. Targeted heat-vulnerability-reduced adaptation scenario.

The narrative argument is:

> The future gets much hotter; vulnerability is concentrated in hotspot neighbourhoods; and a constrained targeted package can reduce heat risk more efficiently and more justly than a uniform allocation.

The final page uses a warm red, orange, and teal palette and includes a limitations section to keep the argument convincing but scientifically transparent.

## 13. Final outputs

- Public repository: https://github.com/MaFitz11/suews-hackathon-final
- Public story page: https://mafitz11.github.io/suews-hackathon-final/
- Transcript file: `transcripts/session-transcript.md`

## 14. One-line status summary

- Repository setup: completed.
- Task brief interpretation: completed.
- SUEWS present and future simulations: completed.
- Heat-hour metric analysis: completed.
- Socio-economic vulnerability analysis: completed.
- Constrained targeted adaptation scenario: completed.
- Public data-journalism website: completed and deployed.
- Transcript for lecturer review: completed.

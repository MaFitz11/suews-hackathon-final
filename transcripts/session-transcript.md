# SUEWS Hackathon Session Summary

**Student:** Marina Fitzner  
**Lecturer:** Dr. Ting Sun  
**Repository:** https://github.com/MaFitz11/suews-hackathon-final  
**Website:** https://mafitz11.github.io/suews-hackathon-final/  
**Date:** 24 June 2026

## Research Goal

The goal was to use the SUEWS hackathon dataset for UDA-city to understand heat risk by neighbourhood and to test whether a targeted adaptation package could reduce heat vulnerability more fairly.

The final research story is:

> The future gets much hotter. Heat vulnerability is concentrated in hotspot neighbourhoods. A limited but targeted cooling package can reduce risk more efficiently and more justly.

## What Was Done

1. A public GitHub repository was created from the SUEWS hackathon template.
2. The UDA-city data and task brief were reviewed.
3. SUEWS simulations were run for present and future heat conditions.
4. The main heat metric was defined as hours where 2 m air temperature is above 35 C.
5. Socio-economic heat vulnerability indicators were selected and adapted to the neighbourhoods.
6. A constrained adaptation scenario was designed and tested.
7. A public GitHub Pages website was created to present the results.

## Main Heat Metric

The key metric was:

**Hours with T2 > 35 C**

T2 means air temperature at 2 metres above ground, which is a standard near-surface temperature relevant for human heat exposure.

## Present and Future Heat Results

Future dangerous heat hours increased strongly in every neighbourhood.

| Neighbourhood | Type | Present hours T2 > 35 C | Future hours T2 > 35 C |
|---|---|---:|---:|
| Jade Gardens | refuge | 26 | 169 |
| Kampong Lama | hotspot | 24 | 163 |
| Taman Melati | refuge | 21 | 153 |
| Dhobi Lines | hotspot | 15 | 141 |
| Fuzhou Lanes | hotspot | 13 | 136 |
| Serendib Rise | refuge | 9 | 123 |
| Mlima Moto | hotspot | 1 | 91 |
| Lusitano Square | core | 1 | 72 |
| Victoria Exchange | core | 1 | 66 |
| Zheng He Towers | core | 0 | 45 |

## Vulnerability Indicators

The socio-economic indicators used were:

- Lack of AC / cooling access
- Outdoor work
- Deprivation
- Young children
- Older adults

The most vulnerable hotspot neighbourhoods were mainly Kampong Lama, Dhobi Lines, Fuzhou Lanes, and Mlima Moto. These areas combined heat exposure with weaker cooling access, higher outdoor work, and higher deprivation.

## Adaptation Scenario

The adaptation package was intentionally limited:

- Only 20% of paved or bare-soil land could be converted to vegetation, grass, or water.
- Cooling access could increase by only 50% citywide.
- Vehicle heat reduction of 15% was considered, but not counted in the physical SUEWS result because anthropogenic heat was zero in this setup.

Instead of spreading resources equally, the package was targeted toward the neighbourhoods with the highest combined heat and social vulnerability.

## Main Adaptation Results

The targeted package reduced risk-pressure in every neighbourhood by at least 5%, with bigger reductions in the most vulnerable areas.

| Neighbourhood | Risk-pressure reduction |
|---|---:|
| Kampong Lama | 19.6% |
| Dhobi Lines | 18.1% |
| Fuzhou Lanes | 17.8% |
| Mlima Moto | 13.8% |
| All other neighbourhoods | at least 5% |

Citywide risk-pressure reduction was about **15.4%**.

## Main Conclusion

A fair heat adaptation strategy should not treat every neighbourhood the same. In UDA-city, the most efficient and just approach was to protect all neighbourhoods while giving stronger support to the places where heat exposure and social vulnerability overlap.

## Limitations

- UDA-city is synthetic, so this is a method demonstration, not a direct real-world policy plan.
- The socio-economic indicators are synthetic and should be replaced with real local data for real decisions.
- The future scenario is a heat stress test, not a full climate projection.
- Cooling access was represented as a vulnerability reduction, not as a direct indoor health model.
- Vehicle heat reduction was discussed but not physically counted in SUEWS because anthropogenic heat was zero.

## Final Outputs

- Public repository: https://github.com/MaFitz11/suews-hackathon-final
- Public website: https://mafitz11.github.io/suews-hackathon-final/
- Transcript file: `transcripts/session-transcript.md`

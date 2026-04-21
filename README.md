<div align="center">
# Prix denrées - Togo 2026

**20 948 prix DPSSE** (Nov25-Mar26) | R/tidyverse

[![Rapport](screenshots/report_preview.png)](prix_marche_analysis.html)
</div>

## 📊 Données
| Métrique | Valeur |
|----------|--------|
| Observations | 20 948 |
| Médiane | **600 FCFA/kg** |
| Max | 13 072 FCFA/kg |

![Distribution](screenshots/histo_prix.png)

## Résultats
- **Grand Lomé** : +89% vs Savanes
- **Arachide/Poulet** : σ > 500 FCFA/kg

## Code
```r
library(tidyverse)
prix_marche <- prix_marche2%>% 
  group_by(marches, produits, mois) %>% 
  summarise(prix_moy = mean(prix_moy))
```

## 🇬🇧 English
**20k food prices** | Togo markets | Data cleaning | ggplot2

**KAGNIRA Bihèbè** - Data Analyst Lomé
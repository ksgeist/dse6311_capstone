# README

## Dataset description
This dataset contains daily store-product sales series designed for research on retail demand forecasting and stockout-aware prediction. It includes hourly sales and stock-status information, discounts, promotions, calendar features, and weather covariates. Primary uses could include:

- forecasting product demand across stores and time
- identifying stockout patterns and examining how availability affects observed sales
- comparing demand forecasts with and without stock-availability information
- simulating replenishment policies under different assumptions about inventory costs and stockout risk

### Possible Question
Can we estimate true product demand and make better replenishment decisions when recorded sales are limited by stockouts?

## Source Citation
FreshRetailNet-50K (2025). Research dataset for stockout-aware retail demand forecasting. Hugging Face. https://huggingface.co/datasets/kush316/FreshRetailNet-50K

Research paper: https://arxiv.org/abs/2505.16319

## Data documentation
Dataset files, feature descriptions, and access instructions are provided on the dataset page: https://huggingface.co/datasets/kush316/FreshRetailNet-50K
Dataset card states CC BY 4.0, but verify use before distributing. You may need to ask for permission from the authors to publish publicly.

## Additional notes
These data are a **research benchmark**, thus you should treat this as a a simulation. Thus, if you simulate inventory policies, you must state assumptions about lead times, holding costs, and stockout costs because these are not necessarily observed in the dataset.

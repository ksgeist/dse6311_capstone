# README

## Dataset description
This dataset captures hourly household electricity consumption during the Norwegian iFlex dynamic-pricing field experiment, alongside experimental price signals, outdoor temperature, and household survey information. Price signals were tested across several Norwegian regions over two winter periods in 2020 and 2020–2021. Primary uses could include:

- forecasting hourly household electricity demand
- investigating household demand flexibility under variable hourly prices
- comparing consumption patterns across price-signal and control groups
- combining time-series usage data with household survey characteristics

### Possible question
Which households shift electricity use in response to variable pricing, and can we predict their flexibility?

## Source Citation
Hofmann, Matthias; Siebenbrunner, Turid (2023). A rich dataset of hourly residential electricity consumption data and survey answers from the iFlex dynamic pricing experiment. *Data in Brief*, 50, 109571. https://doi.org/10.1016/j.dib.2023.109571

Dataset repository: Zenodo. https://doi.org/10.5281/zenodo.8248802

## Data documentation
The data article describes the files and variables, including `participants.csv`, `experiment_days.csv`, `data_hourly.csv`, `price_signals.csv`, and the survey question and answer files: https://pmc.ncbi.nlm.nih.gov/articles/PMC10539631/

## Additional notes
The hourly file is approximately 1.1 GB. Consider whether file size will create compute concern for your needs. A subsample (structured or random - think through your design carefully!) could be used instead if size is a concern.

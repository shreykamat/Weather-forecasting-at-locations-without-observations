# Weather-Forecasting-at-unobserved-locations

This is a MSc project performed at the University of Leeds, UK, in collaboration with the UK Met Office.

The idea is to improve weather forecasts/predictions across the globe by building climatology models using temperature observations. The observations include more than 9 million entries collected from over 7000 locations around the globe, covering all continents.

We aim to quantify how machine learning methods (neural networks and random forests) perform for temperature climatology and identify the best configurations.
The selected configurations are further integrated with the Standard Anamoly Model Output Statistics (SAMOS) framework, to improve forecasts.

The evaluation is carried out across two spatial scopes; one focusing on the UK and the other on a global scale. This enables us to examine the potential for regional adaptability and compare the effectiveness of models trained locally versus those trained globally.

The datasets and code for model integration with the SAMOS framework are not included in this repository as they are a part of Met Office internal resources.

Repository contains notebooks that build climatology (ML) models and compare following configurations:
1. UK-only training domain versus a global training domain.
2. Neural network versus random forest performance.


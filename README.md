# kNN Continent Classifier

## Description

In this analysis, I will be creating a *k*-nearest neighbors (kNN) classifier to predict the continent of any location based solely on its geographical coordinates. To do this, two underlying data sets are used: the first contains the coordinates of thousands of cities around the world and the country those cities belong to, and the second contains the countries of the world and the continent those countries belong to. Joining these two datasets yields a further dataset that effectively maps each set of coordinates to a continent. This is the dataset the model is trained on. Tuning of the *k* parameter is achieved using cross-validation in the train set, with the resulting model evaluated on the test set and then applied to an example (in this case, predicting the continent of Alert, Nunavut).  

## Dependencies

- NumPy
- Pandas
- Scikit-learn
- Matplotlib

For a full list of dependencies—both direct and transitive—please refer to the provided requirements.txt file.

## Usage

The model itself is located at ```/model/kNN Continent Classifier.ipynb```. This file walks you through the overall process from beginning to end, from importing and preprocessing to building and evaluating. The two underlying datasets are stored in  ```/data```, which the .ipynb file references when importing.

## Data Sources

Cities dataset: [GeoNames, via public.opendatasoft.com](https://public.opendatasoft.com/explore/dataset/geonames-all-cities-with-a-population-1000/table/?disjunctive.cou_name_en&sort=name)<br>

Country-continent dataset: [Our World in Data](https://ourworldindata.org/grapher/continents-according-to-our-world-in-data)
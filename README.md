# weather_NLP_model
## Preprocessing Data
1. Convert emoticons to word
2. Removed stopwords
3. Remove punctuations

Multiple combination of preprocessing methods are done and tested. The performance after removing stopwords and punctuation aren't good, so only the first one 
was chosen

## Feature Engeneering
1. TF-IDF, N-of grams,  one hot encoding were tested to vectorized the tweets but TF-IDF performed the best.
2. Train data were splits into train and test data

## Cross Validation
1. Cross validation was done on each model to choose the best parameters for them
2. Cross validation was involved in ensemble model as well

## Modelling
1. Final model was an ensemble model (with stacking method) where Random Forest, Gradient Boost and Ridge Regression Model were selected as 
base model.
2. Linear regression was the meta model which make the final prediction based on the predictions from the three base models.

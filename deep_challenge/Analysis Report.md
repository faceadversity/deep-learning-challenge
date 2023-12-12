
# OVERVIEW
The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. I need to implement features in the dataset provided to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

# RESULTS
## Data Preprocessing
    * Metrics such as EIN and NAME were excluded from the dataset while other target variables left were considered in the analysis.
    * Both Classification and Application Type were features of the model.
## Compiling, Training, and Evaluating the Model
The first model had a deep neural network with 2 hidden nodes containing much larger sample sizes (99, 66 respectively). The optimized model got improved with an additional hidden node and smaller sample sizes (9, 16, 21 respectively) to improve accuracy measures requested over 75%.
![finalNN](https://github.com/faceadversity/deep-learning-challenge/assets/137361966/c0af7418-18cc-46c1-a851-091d8053c919)

The exact parameters for the final model can be found below:

![finalnnparam](https://github.com/faceadversity/deep-learning-challenge/assets/137361966/3270ce99-2c2e-4e80-9b1b-df86b0264dd0)




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

There were several steps taken in my attempts to increase model performance and they are as follows:

    * Kept the NAME ID and dropped the non-beneficial EIN ID column.
    * Used NAME value counts rather than APPLICATION_TYPE for binning procedures.
    * For list of classifications to be replaced I reduced the count number from 1000 to 100.
    * Drastically reduced sample sizes and added an additional hidden node to improve accuracy measures as I already illustrated above.
    * Increased intensity for the final trained model by including a 'validation_split' library and raising epochs significantly 5x the original metrics (from 60=>300).

Largely thanks to all the measures listed above, I was able to improve the model using test data by well over 75% as shown below:

Original test parameters and accuracy scores

![prior_optnumbers](https://github.com/faceadversity/deep-learning-challenge/assets/137361966/d23443a1-ee3c-4186-a01f-6c987bf96908)

Final test parameters and accuracy scores

![final_optnumbers](https://github.com/faceadversity/deep-learning-challenge/assets/137361966/b9cbd966-681d-41a9-86ee-5491d5c70a72)

## Summary
I would follow guidelines illustrated clearly here on optimal methods to ensure accuaracy numbers meet expected targets over 75%. Going well beyond this accuracy measure (90%+ as an example) would probably involve several more layers and a much larger epoch sample to pull from (1000+).

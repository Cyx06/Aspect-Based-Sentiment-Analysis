# Aspect-Based-Sentiment-Analysis(ABSA)

This project from NLP final project, our team implemented an ABSA system, which included designing data augmentation algorithm, implementing and training the model, and conducting follow-up discussions.

The following is an introduction to ABSA and the steps to train the model, parts of data augmentation method and follow-up discussions are shown in report.pdf.

## What is ABSA?
Aspect-Based Sentiment Analysis (ABSA) is a fine-grained approach to sentiment analysis that not only identifies the overall sentiment of a text but also determines the sentiment expressed toward specific aspects or components mentioned within it.

For instance, in a restaurant review:
"The food was delicious, but the service was terrible."

- Overall sentiment: Mixed (positive about food, negative about service)
- Aspect-specific sentiments:
1. Food: Positive
2. Service: Negative

## Steps to start a new training
1. Download the dataset to "Dataset/asap_NLP_2022_Spring".
2. Create "Sentiment_Analysis" folder to store the check point and the model.:
3. Select IDE according to the running environment:
4. Change batch_size according to the GPU memory:
5. Switch USE_WANDB to decide whether to use wandb for logging.
6. Set RESUME to False to generate a new run_id.
7. Use brief_name to name the main change of this experiment.
8. Delete previous check point of model if exists.
9. Run all cells.
10. A new run_id will be generated, copy it and replace the old.


## Steps to resume a old training after an interruption

1. Make sure the run_id is replaced with the new one.
2. Make sure the check point has been synchronized the the drive.
3. Run all cells:

## Steps to test

1. Resume to an existing experiment using the 1st and 2nd step above.
2. Run the cells include "Load check point" and all above.
3. Skip the cells "Run experiment"... to prevent a training
4. Run the all cells of "Testing".
5. Two csv files will be generated for submission.

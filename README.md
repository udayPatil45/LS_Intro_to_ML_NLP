# LS_Intro_to_ML_NLP

Assignment 3

Sentiment Analysis Pipeline Using BERT                                        
In this assignment, I designed a sentiment analysis pipeline using Hugging Face’s transformers and i downloaded the dataset from imdb, and i finetunned a pre-trained bert-base-uncased model on a custom poem sentiment dataset. The dataset was provided in .parquet format and split into training, validation, and test sets. Each entry contained poetic text (verse_text) and an associated sentiment label (0 = neutral, 1 = positive, 2 = negative).
The pipeline began by converting the data into Hugging Face Datasets and applying BERT’s tokenizer with padding and truncation. A BERT model was loaded with a classification head for 3-class output. I used the Trainer API to handle training, with manual control over batch size, number of epochs, and weight decay.
Evaluation was done using accuracy and F1 score metrics. Finally, I saved the fine-tuned model and demonstrated inference on a custom poem line. The model successfully predicted sentiment with confidence scores.   
Challenges:                                
i faced Challenges included handling .parquet data format, and dealing with Trainer compatibility issues. These were resolved by checking schema, using from_pandas, and disabling incompatible arguments.
and also one more challenge is that currently the accuracy that i am getting is not good so i will try to do necessary changes to increse that accuracy and make model more better.

LINK - [ https://colab.research.google.com/drive/1QEke4jiBg46LPtgafRyEeFs4u2Dn1X4O#scrollTo=veKREzjmXe_F ] same file i also uploaded in repo use this link if that block is not opening.

Link of Assignment 1 - [https://colab.research.google.com/drive/1Wdv8aGKvtLbhtYCQpAkTfFFGQjNAnT12#scrollTo=wlkwJmwu0WeZ]

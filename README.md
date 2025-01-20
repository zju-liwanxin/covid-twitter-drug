# covid-twitter-drug
This repository contains related code and data of the paper Re-examing COVID-19 drug discussions on Twitter with large language models and co-occurrence networks. We thank all the contributors.

3_drugfilter.ipynb: Used to screen out drug-related tweets from tweets that have already been identified by the CT-BERT-NER, subsequent drug tweet merges were done manually and thus without code rendering.

5_five_drugs.ipynb: Used to merge the tweets belonging to a certain drug according to the list of the colloquial drug expressions and their standardized concepts (i.e., drug trade names, chemical names, and generic names) found on Wikipedia, and took the tweets of the top 5 drugs, and then extracted the corresponding frequency and sentiment tendencies and summarize them into a dataframes over time.

6_time_trend.ipynb: Used to plot the change of the top five drugs occurrence frequency over time.

7_sentidis.ipynb: Used to plot the distribution and change of the top five drugs entities sentiment over time.

8_lda.ipynb: Used to generate the appropriate topics of drug-related tweets.

9_1drug_co_occurence.ipynb：Used to obtain the drug-drug co-occurrence matrix.

9_2drug_symp_cooccurence.ipynb:Used to obtain the drug-symp co-occurrence matrix.

Due to privacy restriction of Twitter, only tweet ID can be released. Tweets IDs can be obtained at: https://github.com/echen102/COVID-19-TweetIDs

Datasets and model for NER and TSA models are public available at:  https://github.com/YLab-Open/METS-CoV

All codes are based on Python software (version 3.8) and the NER, TSA models are developed by PyTorch (version 1.0).

# Sentiment-Analysis-Event-Studies

This project was executed on 5000 SEC 8-K documents from 1995 to 2020.

SENTIMENT ANALYSIS: The main task for this notebok is to compute abnormal stock returns around 8-K filings, and study how these measures vary depending on the positivity/negativity of the filing. Dictionary taken from: https://sraf.nd.edu/textual-analysis/resources.

EVENT STUDIES: Calculated abnormal stock returns and abnormal trading volume around 8-K filings. Abnormal returns are defined in the added picture. the windows are, in relation to the event date, {0}, {-1,+1}, {-2,+2}, {-3,+3}, {-5,+5}

For each paragraphs, broken the filings into sentences, assigned a tone value to each sentence using VADER snetiment analysis (https://stanfordnlp.github.io/CoreNLP/). For each document, calculated the average tone value of all sentences in the document, sort the measure constructed in the above step into quintiles at an annual frequency. Generated a report highlighting the difference in descriptive statistics for CAR for the different quintiles of 8-K filings

# Text-Summariser
A simple document summariser. Uses SpaCy to perform extractive summarisation of the document

## Preprocessing
All the stop words are eliminated from the original text.

## Algorithm

1. The word frequency for each word in the document is calculated. Each of the frequencies is divided by the max frequency to normalize the frequencies.

2. A dictionary consisting of the sentence and it's corresponding sentence score is generated. The sentence scores are calculated by taking the average of the normalized word frequencies of each word appearing in the sentence.

3. The dictionary is sorted in decreasing order of sentence score which is an indicator of importance of a given sentence in context of the document.

4. The top N sentences are displayed in the summary in the order of appearance in the original document.

## License
[MIT](https://choosealicense.com/licenses/mit/)

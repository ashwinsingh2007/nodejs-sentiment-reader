# NodeJs Sentiment Reader
A sentiment analysis app with nodeJS

# Walthorugh and process package follows to ensure accuracy in sentimental analysis

## Data preprocessing
The raw data we get from our user is often filled with a lot of noise and is likely to contain many errors, hence the need to transform it into an understandable/usable format.
To maintain uniform structure in our text data, we need to convert contractions (e.g., I’m, you’re, etc.) to their standard lexicon (i.e., I am, you are, etc.)

## Converting our text data to lowercase
During our sentiment analysis, we want all the data in a uniform format. This step ensures that our algorithm treats good and GOOD as the same words

## Removing non-alphabetical and special characters
To improve our accuracy in classifying the user’s sentiment, we’ll remove special characters and numerical tokens since they don’t contribute to sentiment. This process will ensure that our text data is left with only alphabetical characters.

## Tokenization
This is the process of splitting a text into its individual meaningful units. We can think of a word as a token of a sentence, and a sentence as a token of a paragraph.

## Correcting misspelled words
Since the product reviews will be manually written by our users, there is a high chance of typographic errors. Before passing our data to our sentiment analysis algorithm, let’s use the spelling-corrector package to correct misspelled words, so that if our user inputs lov by mistake, the correct spelling, love, will be passed to our algorithm.

## Removing stop words
Stop words are generally the most common words in a language, which are filtered out before processing. Some examples of stop words include but, a, or, and what. Since these words have no effect on a user’s sentiment, removing them will help us focus on the important keywords.

## Stemming
This is a process of word normalization in NLP that is used to convert derived or inflected words to their base or root form. For example, a stemmer algorithm is expected to reduce the words “giving,” “gave,” and “giver” to their root word, “give.”

## Sentiment analysis with the Natural library
we use the SentimentAnalyzer from Natural to make an analysis of our user’s review.


# Text Mining and Sentiment Analysis using tidytext

The tidytext library in R is one of the most innovative I’ve come across within the language.

tidytext is the cornerstone library for developing text mining algorithms in R (developed by Julia Silge and David Robinson).

Here, I conduct a text mining analysis on one of my former blog posts – “Big Data Helps You Target The Right Market”.

We will see how text mining can:

- Create a “tibble” which can identify the most frequent words in the text
- Develop a wordcloud showing a graphical illustration of word frequency
- Conduct a sentiment analysis to illustrate positive and negative words in the text
- Use of tidytext and word frequency

Firstly, we’re going to load the blog post from a text file – we could link to it directly but I am using a text file to simplify the illustration for the meantime.

To determine word frequency, we are going to do the following:

- Convert text into a data frame suitable for analysis with tidytext
- Remove stop words – or words with no inherent value (and, but, etc.), from the text
- Form a tibble to sort words by frequency in descending order
- Filter this tibble to only include words which appear in the text more than once

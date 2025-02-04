# nytimes-books

Has the demographic representation of best selling authors changed over time? And can GPT fill in the demographic information for authors in its training data. 

To answer the first question, I'm working with data from the NYTimes Bestsellers list ([sourced from Kaggle](https://www.kaggle.com/datasets/sujaykapadnis/new-york-times-bestsellers?resource=download)). It includes books from 1931 to 2020. 

To answer the second, I'm using the gpt api to fill in the missing data and cross checking a random 1% of the dataset. 

## Data cleaning decisions
For 'author', I'm taking a somewhat liberal approach and treating some editors as authors, only looking into demographics of the first author and not the second or further, ignoring illustrators, and treating those who compile the pieces as authors themselves. 

In the process of doing this project, I made a mistake with the cleaning that I should have gone back and fixed (preserving the original author column), but I didn't, resulting in ~5% data loss. 

## Key Takeaways
* There is more female representation on the NYTimes Bestseller list since around 1995.
* Ivy league degrees are less well representated than in the mid 1960's.
* From 1982 until 2020 there were virtually no best sellers from China.

## Next steps
* Figure out how old each author was when they first hit the nytimes best seller list.
* Take this data out into Tableau to visualize it more nicely.   

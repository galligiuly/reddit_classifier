# Which subreddit best fits my post?

#### Preamble

This work comes from a TFM project I've done for my Master of Data Science from Kschool Madrid. 

In this version I have omitted the didactic and descriptioning steps and I've applied, in a more efficient way, improvements that I've been discovering and studying during the development of the master's final job.



#### Project purpose

The purpose of my project is to train an NLP model that could be able to suggest the fittest subreddit for bloggers who want publish in Reddit.
Given a text from a post or a blog, my NLP model would suggest in which subreddit it could be published

_Multiclass Classification problem_



## Project Presentation

Original Idea

https://slides.com/galligiuly/galligiuly/live?context=editing#/



Final results

https://slides.com/galligiuly/tfm-recommendation-of-subreddit-for-blogs-results/live?context=editing#/



## Data

The following [link](https://bigquery.cloud.google.com/dataset/fh-bigquery:reddit_comments?pli=1) refers to a collection of 1.7 billion comments uploaded to BigQuery and from where I started to analyze and query the data used for my work.

#### reddit_comments

The table of comments gives me a huge amount of text that helps me with my purpose. 

Analyzing `number of comments` and `number of unique authors` that write comments, has been a filter used to find the most popular subreddits that grow at a specific time during the life of Reddit and still remain active.

#### reddit_posts

Apart from the analysis of comments I decided to make an analysis for posts because the original post (title and corpus of it) should contain more key words that better identify the subreddit, precious information for my study.

The idea is the same as for the comments, filter the parameters most important that give me the most popular subreddits still actives nowadays.

#### Objective

What I need is to find the subreddits that have a large amount of data, a good ratio of popularity during the years and belongs to different thematic categories.

I explored my data, analyzing number of wrintng authors and number of comments comparing them and searching a criteria for my selection.

# Project organization

| Folder                                                       | Description                                                |
| :----------------------------------------------------------- | ---------------------------------------------------------- |
| [01_inspection](https://github.com/galligiuly/reddit_classifier/tree/master/01_inspection) | Process applied to find the subreddit's target for my job. |
| [02_cleaning](https://github.com/galligiuly/reddit_classifier/tree/master/02_cleaning) | Data clieaning and pre-processing                          |
| [03_final_model](https://github.com/galligiuly/reddit_classifier/blob/master/03_final_model/06_reddit_LSTM_model_V2.ipynb) | LSTM final model implementation                            |

#### 

# Subreddit Selection

| Category    | subreddit  |
| ----------- | ---------- |
| Health      | Fitness    |
| Religion    | atheism    |
| Cute        | aww        |
| Geography   | europe     |
| Video Games | gaming     |
| Movies      | movies     |
| Sport       | nba        |
| Politic     | politics   |
| cience      | science    |
| Technology  | technology |





# Tools used

- BigQuery
- DataStudio
- Colab
- Jupyter notebook





# Programming lenguages used

- Python

- BigQuery SQL





# Libraries

`pandas`

`numpy`

`nltk`

`sklearn`

`gensim`

`matplotlib`

`altair`

`spacy`

`keras`

`tensorflow`

`seaborn`



# Steps to exectute the job

### gcloud 

Make shure you have `gcloud` SDK installed (here the [link](https://cloud.google.com/sdk/docs/quickstart-macos) to do it) and that you can use it Jupyter notebook.

Once it's installed, you need to add the `gcloud` executable to the `$PATH` environment variable.  Default installation process does this automatically, but if you haven't followed it, you can edit your `.bashrc` or `.zshrc` file and add it as follows:

```bash
export PATH=/Users/<youruser>/<gcloud-downloaded-folder>/bin:$PATH
```

After adding it to your path, you will need to run `jupyter notebook` from a shell that has the new path already, the easiest way is to restart the terminal.



### Testing the project

If you just want to test the project, you can execute [the testing notebook](https://github.com/galligiuly/reddit_classifier/blob/master/project_testing_V2.ipynb) which is already prepared to run with the best performing model.



# References

[My Linkedin](https://www.linkedin.com/in/giulia-galli-7669ba85/?locale=en_US)

[Kschool](https://kschool.com/)


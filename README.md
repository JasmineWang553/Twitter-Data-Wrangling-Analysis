# Twitter-Data-Analysis

- **Intro**: [WeRateDogs](https://twitter.com/dog_rates?lang=en) is a Twitter account that posts pictures of other people’s dogs with a humorous comment and gives them a rating out of 10 per dog in the picture.  However, the uniqueness comes in that the numerator of the rating can exceed the denominator 10 depending on the content. 
- **Goal**: Therefore it will be interesting to investigate if WeRateDogs' unique rating follows the trend of popularity, which is measured by number of retweets and favorites. 
- **Tech used**: Twitter API, Tweepy, Requests, JSON, Numpy, Pandas, Seaborn

![alt text](https://d17h27t6h515a5.cloudfront.net/topher/2017/October/59dd378f_dog-rates-social/dog-rates-social.jpg)

## Project Details
1. **Data Wrangling**
    - Gathering data
    - Assessing data
    - Cleaning data
3. **Data Analyzing**
    - Storing, analyzing, and visualizing your wrangled data

Reporting on 1) your data wrangling efforts and 2) your data analyses and visualizations

### Gathering Data for this Project
** Original Tweets up to August 1st, 2017 will be investigated
<br>
1. WeRateDogs downloaded their Twitter archive and shared it exclusively for use in this project. This archive contains basic tweet data (tweet ID, timestamp, text, etc.) for all 5000+ of their tweets as they stood on August 1, 2017. Downloaded manually from an URL provided by Udacity <code><mark>twitter_archive_enhanced.csv</mark></code>.
2. The tweet image predictions, i.e., what breed of dog (or other object, animal, etc.) is present in each tweet according to a neural network. This file (<code><mark>image_predictions.tsv</mark></code>) hosted on Udacity's servers and should be downloaded programmatically using the [Requests](http://docs.python-requests.org/en/master/) library and the following URL: https://d17h27t6h515a5.cloudfront.net/topher/2017/August/599fd2ad_image-predictions/image-predictions.tsv
3. Each tweet's retweet count and favorite (i.e. "like") count at minimum, and any additional data you find interesting. Using the tweet IDs in the WeRateDogs Twitter archive, query the Twitter API for each tweet's JSON data using Python's [Tweepy](http://www.tweepy.org/) library and store each tweet's entire set of JSON data in a file called <code><mark>tweet_json.txt</mark></code> file. Each tweet's JSON data should be written to its own line. Then read this .txt file line by line into a pandas DataFrame with (at minimum) tweet ID, retweet count, and favorite count.

### Assessing and Cleaning Data for this Project

After gathering each of the above pieces of data, assess them visually and programmatically for quality and tidiness issues. Detect and document at least **eight (8) quality issues** and **two (2) tidiness issues** in your <code><mark>wrangle_act.ipynb</mark></code> Jupyter Notebook. To meet specifications, the issues that satisfy the below mentioned **Key Points** must be assessed.


### Storing, Analyzing, and Visualizing Data for this Project

Store the clean DataFrame(s) in a CSV file with the main one named <code><mark>twitter_archive_master.csv</mark></code>. If additional files exist because multiple tables are required for tidiness, name these files appropriately. Additionally, you may store the cleaned data in a SQLite database (which is to be submitted as well if you do).

Analyze and visualize your wrangled data in your <code><mark>wrangle_act.ipynb</mark></code> Jupyter Notebook. At least **three (3) insights and one (1) visualization** must be produced.

### Reporting for this Project

Create a **300-600 word written report** called <code><mark>wrangle_report.pdf</mark></code> that briefly describes your wrangling efforts. This is to be framed as an internal document.

Create a **>250 word written report** called <code><mark>act_report.pdf</mark></code> that communicates the insights and displays the visualization(s) produced from your wrangled data. This is to be framed as an external document, like a blog post or magazine article, for example.

# News_Popularity_prediction
A hackathon in machine_hack

Dataset Description:<br>
<br>
Train.csv - 7928 rows x 59 columns<br>
Test.csv - 31716 rows x 58 columns<br>
Sample_Submission.csv - Acceptable submission format<br>
Attribute Information:<br>
<br>
Number of Attributes: 59(includes 1 target field)<br>
<br>
n_tokens_title: Number of words in the title <br>
n_tokens_content: Number of words in the content<br>
n_unique_tokens: Rate of unique words in the content<br>
n_non_stop_words: Rate of non-stop words in the content<br>
n_non_stop_unique_tokens: Rate of unique non-stop words in the content<br>
num_hrefs: Number of links<br>
num_self_hrefs: Number of links to other articles published by Mashable<br>
num_imgs: Number of images<br>
num_videos: Number of videos<br>
average_token_length: Average length of the words in the content<br>
num_keywords: Number of keywords in the metadata<br>
data_channel_is_lifestyle: Is data channel 'Lifestyle'?<br>
data_channel_is_entertainment: Is the data channel 'Entertainment'?<br>
data_channel_is_bus: Is data channel 'Business'?<br>
data_channel_is_socmed: Is data channel 'Social Media'?<br>
data_channel_is_tech: Is the data channel 'Tech'?<br>
data_channel_is_world: Is data channel 'World'?<br>
kw_min_min: Worst keyword (min. shares)<br>
kw_max_min: Worst keyword (max. shares)<br>
kw_avg_min: Worst keyword (avg. shares)<br>
kw_min_max: Best keyword (min. shares)<br>
kw_max_max: Best keyword (max. shares)<br>
kw_avg_max: Best keyword (avg. shares)<br>
kw_min_avg: Avg. keyword (min. shares)<br>
kw_max_avg: Avg. keyword (max. shares)<br>
kw_avg_avg: Avg. keyword (avg. shares)<br>
self_reference_min_shares: Min. shares of referenced articles in Mashable<br>
self_reference_max_shares: Max. shares of referenced articles in Mashable<br>
self_reference_avg_sharess: Avg. shares of referenced articles in Mashable<br>
weekday_is_monday: Was the article published on a Monday?<br>
weekday_is_tuesday: Was the article published on a Tuesday?<br>
weekday_is_wednesday: Was the article published on a Wednesday?<br>
weekday_is_thursday: Was the article published on a Thursday?<br>
weekday_is_friday: Was the article published on a Friday?<br>
weekday_is_saturday: Was the article published on a Saturday?<br>
weekday_is_sunday: Was the article published on a Sunday?<br>
is_weekend: Was the article published on the weekend?<br>
LDA_00: Closeness to LDA topic 0<br>
LDA_01: Closeness to LDA topic 1<br>
LDA_02: Closeness to LDA topic 2<br>
LDA_03: Closeness to LDA topic 3<br>
LDA_04: Closeness to LDA topic 4<br>
global_subjectivity: Text subjectivity<br>
global_sentiment_polarity: Text sentiment polarity<br>
global_rate_positive_words: Rate of positive words in the content<br>
global_rate_negative_words: Rate of negative words in the content<br>
rate_positive_words: Rate of positive words among non-neutral tokens<br>
rate_negative_words: Rate of negative words among non-neutral tokens<br>
avg_positive_polarity: Avg. polarity of positive words<br>
min_positive_polarity: Min. polarity of positive words<br>
max_positive_polarity: Max. polarity of positive words<br>
avg_negative_polarity: Avg. polarity of negative words<br>
min_negative_polarity: Min. polarity of negative words<br>
max_negative_polarity: Max. polarity of negative words<br>
title_subjectivity: Title subjectivity<br>
title_sentiment_polarity: Title polarity<br>
abs_title_subjectivity: Absolute subjectivity level<br>
abs_title_sentiment_polarity: Absolute polarity level<br>
shares: Number of shares (target)<br>
<br>

<p> In this Hackathon we need to predict the number of shares of a article given above information.</p><br>

<ul>
  <li> Initial Observation this is Regression Problem </li>
  <li> Next, here we observed that the co-relation of the target with attributes is not quite good  So,my initial intial test_model ended up in high Bias and variance.</li>
  <li> To make my model to perform best,i plotted every attribute vs target and tried to get some information_gain.In this Process I found some of the features are useless and
    So,i decided not to include  them in the model</li>
  <li>  Still my model doesn't perform well high bias and variance.</li>
  <li> Next i decided to do Two things,To reduce bias using the plots
      <ul>
        <li> I thought to get new attributes that are more informative about target </li>
        <li> use more advanced regression techniques.</li>
    </ul>
   </ul>
   
   
    

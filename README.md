# Sentiments Evoked by WHO Public Health Posts during COVID-19 Pandemic: A Neural Network based Machine learning Analysis
Since the establishment of the WHO in 1948, it has played a pivotal role in improving public health all over the world. But in 2019, with the onset of COVID-19, the WHO, for the first time, faced a pandemic of such a mamothian magnitude and global span. Spanning 220 region and with over 200 Million reported cases (as of Aug’21), it has been the biggest public health crisis since the inception of the WHO. The spread of the virus and the perceived inability of the WHO to contain it has raised many questions about its efficacy and need. Thus with the present study we attempt to explore the range of sentiment and emotions evoked by public health information posts by the WHO on its official Facebook page throughout the pandemic. 
_________________________________________________________________________________________________________________________________________________________________
# Methods used in the Study

<p align="center">
  <img width="644" alt="pipeline" src="https://user-images.githubusercontent.com/44245211/137946308-e01e26ff-e8c0-4a43-b012-d242faa5b5d7.png">
  </p>

## Dataset - Timeline of Facebook Posts 
We first defined 3 timeframes of 5 months each, starting from March 2020. We choose a total of 6 posts, two posts from each timeframe. The posts were identified on the basis of their content and engagement, which addressed the primary concerns of the public in that particular time frame. The chosen posts had at least 1800 comments to ensure a tenable prediction model and to have a general sense of prevailing sentiments. 

<p align="center">
  <img width="937" alt="posts" src="https://user-images.githubusercontent.com/44245211/137947709-7794d8d5-501a-4d40-b0ae-4c6c683a0915.png">
  </p>
  
1. The first time frame T1 spans from March 2020 to July 2020
- Post-1 (or P1) consisted of a cartoon depicting a man sneezing into his elbow in a public transport and advocating for this action. None of the characters in the cartoon had worn a mask. [LINK](https://www.facebook.com/WHO/photos/a.167668209945237/3340903362621690)
- Post-2 (or P2) comprised of suggestion to health care workers on stress coping strategies during the pandemic. [LINK](https://www.facebook.com/WHO/photos/a.167668209945237/3340899275955432)

2. The next timeframe T2 extends from August 2020 to December 2020
- Post-3 (or P3) attempted to bring back feeling of normalcy by indicating that the COVID virus is here to stay and called the period “New Normal”. [LINK](https://www.facebook.com/WHO/photos/a.167668209945237/3484521414926550)
- Post-4 (P4) suggested guidelines to avoid 3 C’s - Crowded Places, Close Contact Sitting and Confined Settings. [LINK](https://www.facebook.com/WHO/photos/a.167668209945237/3771444976234191)

3. The final time frame T3- spans from January 2021 to May 2021
- Post-5 (or P5) attempted to squash rumours pertaining to the safety and efficacy of the vaccine. [LINK](https://www.facebook.com/WHO/photos/a.167668209945237/4473264166052265)
- Post-6 (or P6) depicted an animation asserting the role of COVAX in managing COVID. Through the post the WHO urged that even with the introduction of the vaccines “no one is safe till everyone is safe”. [LINK](https://www.facebook.com/watch/?v=1012908982851652)

## Data labelling - labels used
<p align="center">
  <img width="871" alt="data" src="https://user-images.githubusercontent.com/44245211/137949226-5bbe6f93-3128-46de-a5da-b00e91e37570.png">
  </p>
The data was labelled into five categories which encompassed a broad range of positive and negative emotions associated with the comments. The labels are shown in the bubbles with example comments above them. <br />
1.  Angry labelled as A consisted of Hateful and angry comments.<br />
2.  Concerned sentiments labelled as B consisted of negatively sarcastic comments and comments displaying emotions of concern.<br />
3.  Comments which included personal advice and irrelevant stats along with comments which had no remote connection to the post were labeled as C.<br />
4.  Labels D and E were associated with positive comments, with comments of agreement being labelled as D and laudatory comments showing emotions of thankfulness labelled as E.

## Data labelling - labels used
<p align="center">
  <img width="593" alt="nn" src="https://user-images.githubusercontent.com/44245211/137950490-3b5bdbb6-043b-4fae-b88c-b225347d610c.png">
  </p>
This flow diagram explains the basic working of the classifier. We hand labelled 3000 comments (1000 from each timeframe) which were used to train and test the neural network. We achieved an accuracy of 85.27%. Next we used the same, trained, neural network to sort 4420 comments from T1, 5256 from T2 and 3902 from T3.

# Results
<p align="center">
  <img width="765" alt="res1" src="https://user-images.githubusercontent.com/44245211/137950759-9a814c03-182e-4a53-b5c3-4ef38fb1f696.png">
  </p>
These graphs represent the raw results from the classifier. Each graph indicating the number of posts classified in each sentiment category. Although the graphs allow us to observe domination for negative sentiments, we can’t compare the results across time periods. Hence, we use another metric - percentage of posts.

### Sentiment Evolution - percentage of posts
<img width="430" alt="pp" src="https://user-images.githubusercontent.com/44245211/137956721-254b43e6-3842-4b6f-82bd-c3f51906611e.png">

# Inferences
- We see that the posts received an overwhelmingly negative response and among the negative sentiments, anger dominated in all three timeframes. As we saw previously the negative sentiments peak in the T2 time period. 
- Further analysis of comments tell us that the negative sentiments where directed primarily towards the WHO, governments and other influential personalities. On the other hand, positive comments were expressed primarily towards health workers.
- Angry individuals tend to misconstrue false claims to be scientifically credible which might lead to vaccine hesitancy that may severely compromise the fight against COVID-19.
- Mass media & social media has contributed to the spread of misinformation and denial of scientific literature.

# Conclusions - Concerns & Suggestions
- WHO is the only source of legally binding international regulations for pandemic response, and hence the establishment of its authority and integrity is paramount. WHO is an international public health watchdog but the apparent damage to its credibility, which is reflected by the current study, is alarming.
- The enormity of the health crisis which led to isolation and economic crisis coupled with questionable information sources on social media and aspersions on credibility of WHO created a concoction such that even the innocuous public health information posts by WHO were misconstrued, generating an overall negativity in public psyche.<br /><br />
- WHO should work on increasing its credibility with particular attention to transparency, political and business neutrality, and adapting evidence-based policy. WHO ought to be insulated from political and global strategic games.
- During such a crisis it is very important to realise concerted efforts have to be made to address both the psychological and emotional well-being so as to uphold the public morale.



# Sentiments Evoked by WHO Public Health Posts during COVID-19 Pandemic: A Neural Network based Machine learning Analysis
Since the establishment of the WHO in 1948, it has played a pivotal role in improving public health all over the world. But in 2019, with the onset of COVID-19, the WHO, for the first time, faced a pandemic of such a mamothian magnitude and global span. Spanning 220 region and with over 200 Million reported cases (as of Aug’21), it has been the biggest public health crisis since the inception of the WHO. The spread of the virus and the perceived inability of the WHO to contain it has raised many questions about its efficacy and need. Thus with the present study we attempt to explore the range of sentiment and emotions evoked by public health information posts by the WHO on its official Facebook page throughout the pandemic. 

## Methods - Pipeline Representation

<p align="center">
  <img width="644" alt="pipeline" src="https://user-images.githubusercontent.com/44245211/137946308-e01e26ff-e8c0-4a43-b012-d242faa5b5d7.png">
  </p>

## Methods - Pipeline 
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
The data was labelled into five categories which encompassed a broad range of positive and negative emotions associated with the comments. The labels are shown in the bubbles with example comments above them.
- Angry labelled as A consisted of Hateful and angry comments
- Concerned sentiments labelled as B consisted of negatively sarcastic comments and comments displaying emotions of concern
- Labels D and E were associated with positive comments, with comments of agreement being labelled as D and laudatory comments showing emotions of thankfulness labelled as E.
- Comments which included personal advice and irrelevant stats along with comments which had no remote connection to the post were labeled as C.


+++
title = "Gender Stereotypes in STEM in Latin America"
date = 2022-07-01
summary = "Using satellite and minimal survey data to predict regional poverty rates in Ethiopia."
+++

**What it does**  
Using over 1 million tweets from Latin American users between 2019 and 2020, this project employs Natural Language Processing (NLP) techniques to analyze the tone and content of STEM discourse on social media. Our findings reveal the pervasive presence of gender stereotypes: girls and young women are more likely than their male counterparts to post and resonate with content promoting negative views of STEM subjects. Positive mentions of women in STEM largely originate from networks explicitly focused on gender equality, highlighting the underrepresentation of women’s participation in STEM careers. Additionally, our analysis uncovers a strong overrepresentation of male researchers and scientists in mentions of STEM discoveries, leaving women’s contributions largely invisible in the Latin American social media landscape.


<iframe src="https://gender-analysis-of-stem.github.io/visualizations/community_detection/pt_2019_RTN.html"
        width="100%" 
        height="600" 
        style="border: none;">
</iframe>


**Why I made it**  
Gender gaps in STEM are driven not only by educational or economic barriers but also by narratives and role models — or their absence. We wanted to understand how online discourse reflects and reinforces these barriers, especially among younger users. This project explores the digital side of STEM inequality in Latin America, using Twitter data to measure visibility, sentiment, and the representation of women in science conversations.


**Tools & Technologies**  
- **Tools**: Python, Pandas, scikit-learn, octis, contextualized_topic_models, nltk, twint


**What I learned**  
- Text mining and preprocessing large-scale multilingual tweet datasets
- Topic modeling and sentiment classification using libraries like spaCy, scikit-learn, and TextBlob
- Network analysis using retweet and mention graphs to detect echo chambers
- Gender inference from usernames and linguistic patterns (with ethical safeguards)


**Team**  
Built in collaboration with Mariana Consuelo Fernández Espinoza.

🔗 **Code**  
[View on GitHub](https://github.com/Gender-Analysis-of-STEM)
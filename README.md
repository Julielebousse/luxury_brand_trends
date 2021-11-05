# Luxury Groups stock market listing & Luxury brands Google trends
Julie Le Bousse & Anh Nguyen
## Content
- [Description](https://github.com/anhfrenay/luxury_brand_trends/blob/main/README.md#description)
- [Dataset](https://github.com/anhfrenay/luxury_brand_trends/blob/main/README.md#dataset)
- [Workflow](https://github.com/anhfrenay/luxury_brand_trends/blob/main/README.md#workflow)
- [Insights](https://github.com/anhfrenay/luxury_brand_trends/blob/main/README.md#insights)
- [Delivrables](https://github.com/anhfrenay/luxury_brand_trends/blob/main/README.md#delivrables)

## Description
In this project, we were trying to find the link between Google searches on the most notorious French luxury brands and the stock marlet listing price of the related luxury groups.
The scope of our analysis:
- Time interval : 2020
- Luxury groups : LVMH, Kering and Hermes
- Luxury brands : Louis Vuitton, Dior, Gucci, Bottega Veneta and Hermes
- Geographical scope for the Google trends data : world wide

## Dataset 
We use multiple datasets but only 2 types :
- csv. files for the stock market listing price (Source : [abcbourse.com](https://www.abcbourse.com/marches/))
- API from Google : pytrends (documentation [here](https://towardsdatascience.com/google-trends-api-for-python-a84bc25db88f))

## Workflow
Our project can be divided into different phases  :

**Phase 1** : Define the subject and planning for the project
- Look for an interesting topic
- Research to see if there open data available
- Get validated by the Lead Teacher
- Define timeline for each deadline of the project and split the taskload between team members (create Trello to follow the timeline)

**Phase 2** : Looking and trying to get the datasets
Our initial idea were : Finding correlation between vintage luxury offer prices from websites like Vinted or Vestiaire Collective and the brands' hashtags on Instagram
However data on Vestiaire Collective and Instagram were very complicated
- Vestiaire Collective doesn't allow scraping on their website
- Instagram API to get posts from a certain hashtag is possible but not when it's a popular hashtag (Ex: #LouisVuitton has 47 millions posts) and Instagram will block the request after a certain time.

**Phase 3** : Facing the challenges and changing our strategy
After spending a lot of time to reseach and work on the initial idea, we decided to change our topic
Stock market listing price is easy to find and we can get the data in csv format.
Google searches data is possible to get with the Google API pytrends

**Phase 4** : Coding in Python to obtain the data from the 2 sources for each brand/group

**Phase 5** : Creating the database using jointure through SQL and calculating some statistics

**Phase 6** : Working on our Github repository and presentation slides

## Insights
We calculated the correlation coefficient between Google trend data and Stock market listing price of the three groups and compare the coefficients between them.

As expected, the correlation is positive, meaning that the more people search on a brand the more likely the groups stocking price is going up

However, the correlation between Google trends data and Stock market listing price is not the same between three groups. LVMH’s stocking price seems to be more correlated to the Google trends.

This could be explained by the fact that we took the 2 most know brands from LVMH and Kering but there are more brands that can affect the stocking price of the group (Saint Laurent, Balenciaga for Kering for example)

However, the same explication is not applicable to Hermes since the group only has one brand. We will need to find data from social medias since they are the real platforms where consumers of luxury goods express their interest.

## Delivrables
- [Presentation slides](https://docs.google.com/presentation/d/1uAlIWsiG8aCCxZidgZiFtRdCZoaXaIYV/edit?usp=sharing&ouid=105534248596026120360&rtpof=true&sd=true)
- [Github repository](https://github.com/anhfrenay/luxury_brand_trends)
- [Trello](https://trello.com/b/xF3n6xPi)

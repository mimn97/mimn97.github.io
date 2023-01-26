---
layout: project
title: Towards developing NLP tools for extracting SBDH from Twitter 
---


# Why SBDH on Twitter? 

- Openly available data, thus a good resource for public health surveillance. 
- Several previous literature on applying NLP to health-related tweets. However, there is little prior work on identifying SBDH from general tweets. 


# Current Procedures (updating)

## (from the last work...)
- Collected 100K English-written tweets that were created within the U.S. (geo-tagged tweets), using Twarc2 API. 

- Selected SBDH-related keywords (curated by experts) to be used in the search query of Twarc2 API. 

- Manually selected SBDH-related tweets that used figurative language (e.g., metaphor and sarcasm) and tweets that exactly mentioned the keywords. 

- Corrected grammatical errors and misspellings in our tweets by using language-check API. 

- Analyzed the spatial distributions of the collected tweets (e.g., # of tweets that were created in higher/lower socio-economic block groups in the U.S., etc.) and language characteristics (e.g., average # of corrections, length of tweets).

- Tested zero-shot transferability of the existing clinical language models on these collected tweets.
Evaluated the models’ performance by manually annotating the models’ results with humans. 

----------

## (new approach..)
- Collecting COVID-19

- Set up Amazon MTurk for filtering SBDH-related tweets, provided with the detailed annotation guideline.

- Currently annotating the filtered tweets with SBDH evidence (e.g., word span, presence, and period). 

- Hydrating a longitudinal set of tweets of users who were identified from our expert annotation, using Twarc2 API.

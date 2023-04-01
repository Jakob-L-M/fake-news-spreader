# Misinformation spreaders in Reddit data

## Abstract
This repository summarizes different analysis
approaches on the [FACTOID dataset](https://doi.org/10.48550/arxiv.2205.06181) intending to understand
the underlying structure. We will further discuss different models and their effectiveness
in misinformation classification on a post level
as well as proposals regarding better labeling
techniques. Finally, my proposals include an
improved way of labeling users as well as insights gained through manual labeling.


## Introduction
Misinformation Detection is as difficult as it is important. Given the structure of noisy social media text and often used constructs like irony even human readers face difficulties distinguishing real news from misinformation. This report will discuss the structure and possible flaws in the FACTOID dataset, methods to train models for misinformation detection and propose improvements to the labeling process.

Current datasets and researchers classify misinformation spreaders based on the amount of misinformation links users have posted. Usually a threshold of 2 or 3 is chosen and if some user surpasses this threshold they are considered to be a misinformation spreader. To classify a post a set of known domains is used. A user would post some text including a link and if this link is considered to be directed to a domain spreading misinformation the post is classified as misinformation. In the FACTOID dataset, a threshold of 1 is used. This report will discuss challenges regarding the described approach and propose a different way of assigning user labels with the result that the current user labels are not considering major factors such as the number of total posts or posts including more than one link.

A strong misinformation detecting model could heavily reduce the spread of such information as well as the emergence of echo chambers. Social Media platforms such as Instagram introduced automatic warning banners related to potential misinformation about COVID-19 . These banners show up on posts related to COVID-19 and are supposed _"to keeping people safe and informed about coronavirus (COVID-19), COVID-19 vaccines and reducing the spread of false information"_. FACTOID is a user centered dataset which raises the question of user labeling as well as post labeling. The report will cover statistics and models in both regards.

With the thought of extending or building another dataset we would like to understand if the used gathering approach of the FACTOID dataset yielded promising results. A split of 50:50 in real news and misinformation users was enforced during scraping using pre-defined thresholds.  
# Collection of plots

Everything is sorted based on the written summary. Navigate through the folder structure to find a certain plot.

## Folder structure
<pre>
<code>./plots
│   🗎 README.md                    # This File
│   
└───📁 post_level_overview         # Overview over all 3.4mil posts 
│   └─  🗎 <a href="#post-distribution">post_distribution.pdf</a>
|   └─  🗎 <a href="#political-bias">political_bias.pdf</a>
|   └─  🗎 <a href="#factual-factor">factual_factor.pdf</a>
|
└───📁 topic_group_distributions   # Overviews inside topic groups
|   └─  📁 5G
|   └─  📁 Abortion
|   └─  ...
|
└───📁 Group 3</code>
</pre>

# Explanation for plots

## Post Level Overview

### Post Distribution
Post level distribution of all posts. Split in five sub plots.
- (1) The first shows the percentages of labeled and unlabeled post. 

- (2) Second displays the percentage of real- and fake-news posts within the labeled posts.

- (3) The third bar show the topic group distributions based on the number of posts in that group

- (4) Next up a bar similar to (3) be only looking at real news

- (5) Analog to (4) but with fake news posts.

### Political Bias

A Grouped bar chart by topic groups. Displays the relative post level political bias distribution of each topic within the different bias bins.

### Factual Factor

Analog to [political bias](#political-bias) but for factual factor bins

## Topic Group Distributions
There are four plots for each topic group. Three of them are analog to the plots in [Post Level Overview](#post-level-overview). The 4th one is a plot showing where each subreddit associated with the group is positioned based on its aggregated political bias and factual factor. This is a more in depth view of the aggregated grouped bar charts of [the previous chapter](#post-level-overview).
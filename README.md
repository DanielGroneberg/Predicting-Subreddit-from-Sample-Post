## BACKGROUND

r/AntiWork and r/Jobs are two similar subreddits based on advice, stories, etc. related to the workplace. As the name implies, r/AntiWork is a occasionally hostile to the idea of work in general, whereas r/Jobs is more mild, although both contain plenty of workplace horror stories. r/AntiWork reached the height of its fame several years ago when one of its moderators appeared on an ill-fated and Fox News interview, which subsequently brought widespread negative attention to the subreddit. Despite this, the sub has grown to 2.7M followers, with r/Jobs at 1.3M.

## PROBLEM STATMENT

Due to these subreddits discussing similar topics and using similar language, classifying their posts will present an interesting challenge. My goal is to create a model which can classify the subreddit of a new post based on its selftext (the original poster's initial post). On top of this, I will compare the sentiment and wordcount of the posts in both subreddits, to see if my general characterization of the sentiment between the two is accurate.

## DATA DICTIONARY

The Reddit API originally returned about 100 features. I primarily used 'selftext' and 'subreddit'. 'subreddit' is the target variable, so I set it to be the index in the cleaning, modeling and EDA notebooks. I set 'selftext' to be the sole feature in these notebooks as well. As a result, my models only use one feature.

## SUMMARY

As expected, the sentiment of posts in r/Jobs is more positive than those in r/AntiWork, although both were quite polarized. In both cases, the least common sentiment was neutral sentiment. Key words like "manager" and "interview" were polarizing, with r/Jobs users having even more positive sentiment for both words, and r/AntiWork users having even more negative sentiment for both words.

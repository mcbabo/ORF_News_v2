# ORF News Wrapper #

A simple News Wrapper of https://orf.at/ made by mcbabo

## How to use ##

Install package with

```
pip install orfnews
```

### Get top news ###
Create your main.py file

```python
import orf_news
import asyncio

# Create orf class
orf = orf_news.ORF_News()

# Call getTopicNews
newest_post = asyncio.run(orf.getTopicNews("inland"))

# Print out dictionary
print(newest_post)
```

### Get all available topics ###

```python
import orf_news
import asyncio

# Create orf class
orf = orf_news.ORF_News()

# Call getTopics
topics = asyncio.run(orf.getTopics())

# Print out dictionary
print(topics)
```

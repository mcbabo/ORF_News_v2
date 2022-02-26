# ORF News Wrapper #

A simple News Wrapper of https://orf.at/ made by mcbabo

## How to use ##

Install package with

```pip
pip install orfnews
```

### Get top news ###
Create your main.py file

```python
import OrfNews
import asyncio

# Create orf class
orf = OrfNews.ORF_News()

# Call getTopicNews
newest_post = asyncio.run(orf.getTopicNews("inland"))

# Print out dictionary
print(newest_post)
```

### Get all available topics ###

```python
import OrfNews
import asyncio

# Create orf class
orf = OrfNews.ORF_News()

# Call getTopics
topics = asyncio.run(orf.getTopics())

# Print out dictionary
print(topics)
```
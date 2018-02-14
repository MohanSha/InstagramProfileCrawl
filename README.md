<img src="https://s3-eu-central-1.amazonaws.com/centaur-wp/designweek/prod/content/uploads/2016/05/11170038/Instagram_Logo-1002x1003.jpg" width="200" align="right">

# Instagram-Profilecrawl

[![MIT license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/MohanSha/TwitterBot/blob/master/LICENSE)
[![built with Selenium](https://img.shields.io/badge/built%20with-Selenium-red.svg)](https://github.com/SeleniumHQ/selenium)
[![built with Python3](https://img.shields.io/badge/built%20with-Python3-green.svg)](https://www.python.org/)


## Quickly crawl the information (e.g. followers, tags etc...) of an instagram profile. No login required!
Automation Script for crawling information from ones instagram profile.  
Like e.g. the number of posts, followers, and the tags of the the posts

#### Getting started
Just do:
```bash
git clone https://github.com/MohanSha/InstagramProfileCrawl.git
```

It uses selenium to get all the information so install it with:
```bash
pip install selenium
```

Install the proper `chromedriver` for your operating system.  Once you (download it)[https://sites.google.com/a/chromium.org/chromedriver/downloads] just drag and drop it into `instagram-profilecrawl/assets` directory.

## Use it!
Now you can start it using:
```bash
python3.5 crawl_profile.py username1 username2 ... usernameX
```

#### The information will be saved in a JSON-File in ./profiles/{username}.json.
> Example of a files data
```
{
  "alias": "Mohan Sha",
  "username": "mohan.sha",
  "num_of_posts": 34,
  "posts": [
    {
      "tags": ["#fun", "#good", "#goodday", "#goodlife", "#happy", "#goodtime", "#funny", ...],
      "comments": 12,
      "img": "https://scontent.cdninstagram.com/",
      "likes": 284
     },
     {
      "tags": ["#vegan", "#veganfood", "#vegansofig", "#veganfoodporn", "#vegansofig", ...],
      "comments": 6,
      "img": "https://scontent.cdninstagram.com/t51.2885-15/e35",
      "likes": 206
     },
     .
     .
     .
     ],
  "prof_img": "https://scontent.cdninstagram.com/t51.2885-19/",
  "followers": 1950,
  "following": 310
}
```

#### With the help of [Wordcloud](https://github.com/amueller/word_cloud) you could do something like that with your used tags
![](http://i65.tinypic.com/2nkrrtg.png)

<hr />

###### Have Fun & Feel Free to report any issues

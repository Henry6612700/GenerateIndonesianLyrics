# GenerateIndonesianLyrics

How to generate the Indonesian Lyrics

We will gather data (indonesian lyrics) with web scraping technique using _scrapy_ library and lirik.kapanlagi.com as the target.
The information that we should extract is song’s lyric and title.

1.	Create the scrapy project by using this command in your terminal or command prompt:  
	
scrapy startproject filename

2.	Change to the directory by using this command in your terminal or command prompt:
	
cd filename 

3. 	Make the command below in your terminal or command prompt    
	
scrapy crawl filename lirik.kapanlagi.com

It will create a lyricscrapper.py inside the tutorial/spiders folder. We will call it web-crawler because it scrape by 'crawling' into the targeted website.
Here’s our code:
import scrapy
from scrapy.spiders import CrawlSpider, Rule
from scrapy.linkextractors import LinkExtractor
class LyricScrapperSpider(CrawlSpider):
    name = 'lyric_scrapper'

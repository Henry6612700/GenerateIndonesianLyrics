# GenerateIndonesianLyrics
How to generate the Indonesian Lyrics

1.	Create the scrapy project by using this command in your terminal or command prompt:  
	
scrapy startproject filename

2.	Change to the directory by using this command in your terminal or command prompt:
	
cd filename 

3. 	Make the command below in your terminal or command prompt    
	
scrapy crawl filename lirik.kapanlagi.com

It will create a lyricscrapper.py inside the tutorial/spiders folder. We will call it web-crawler because it scrape by ‘crawling’ into the targeted website.
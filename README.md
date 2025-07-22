# project02-canada-news-trending-stories
Scraping + updating top stories across Canada's main national news sites, scraping their trending stories boxes on home page.


For this project I practiced web scraping with beautiful soup and playwright as well as making live-updating tables in Datawrapper using github actions. 

I chose to scrape five of Canada's top news sites, specifically their trending or top stories boxes. Each outlet has their own algorithm for which stories go in there, but on the whole you can assume they're trending or popular in some way. 

I have set these to update every two hours using github actions, which should then be pulled by datawrapper every hour and reflected on the site. 

The Globe and Mail, National Post and Global News are scraped with Beautiful Soup, and CBC and CTV are first scraped with Playwright, which loads the required articles onto the page, and then a saved .html is parsed by Beautiful Soup. 

Each file is overwritten with each new scrape, so I hope in future editions to save a copy of the old .csv and push a new one to datawrapper, to enable me to do some analysis of the top stories over time. 

None of these sites currently pull from an API, thought I believe that would be possible, so it's something I'd like to do in the future. 

I'd like to include a timestamp of when the changes occurred, so readers can know how fresh what they're looking at is, but I couldn't figure it out before submitting. 

I also hope to expand to more news sites in Canada in the future. 

This project and the site design lean heavily on Jonathan Soma's auto-updating websites tutorial https://jonathansoma.com/. 
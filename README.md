# Feature-Film-Analysis

## Background

By now we have all come to understand that one of the industries were technology has effected most is the film /entertainment industry. Streaming services such as Netlfix, Prime and others have taken a massive chunk of this market and as a result the number of people going to see movies in cinemas have dwindled thus feature movies have dropped since. if this hasnt already been bad, the pandemic and delays in big production films have accelerated this even further. According to Independant Newspaper article published on the 8th October 2020, the biggest names in the cinema industry have closed more than 150 cinemas in the UK including CineWorld, Picturehouse and Odean. I therefore have chosen the Feature Films industry which has long been considered as a source of entertainment for many years and generations. When i say Feature Film, i am referring to Academy of Motion Picture of Art and Science in American Film Institute and British Film Institute produced in english. According to British Film Industry - BFI - the film industry contributed £14 billion to the GDP in 2017.

History of the Feature Films According to Wikipedia the term refers to the main film presented in cinemas and one which was promoted and advertised. This is different from shorter films such as newsreels, serials, animated cartoons, live-action comedies and documentaries that used to be presented in the old days before the main feature.

## Aims of the Project

My aim of this project to first confirm the decline of the feature film industry using data and find out the key underlying drives/trends of the feature film industry. The project will focus specifically on feature movie releases world-wide from the top production companies in hollywood. To acheive this, i will be looking to find a comprehensive data on feature films as far back as 1900 and to evaluate the sucess of each movie, i will be using the box office sales and movie ratings. What better way of doing then scrapping the data from the Internet Movie DataBase otherwise known as IMDB, as the IMDB movie database do not contain the box office sales, i will be using a website called The-numbers.com to to collect the commulative box office sales world wide.

## Method of Analysis

This project will mainly be an exploratory data analysis project and will be using python data analysis techniques such as data handing, cleaning, manipulation, aggregation mainly pandas library as well as data visualisation using matplotlib.pyplot. There will be a mix of both qualative and quantative approachs to the project. I will be using mainly data visualisation to get the industry pictures across. Visualising data is the most effective way to of communicating the result of data exploration outcome.

## Method of data collection

I will be using python web Scrapping technique using Requests & BeautifulSoup libraries to collect and tabulate data consisting of movie meta data from IMDB and The-Numbers.com. Both websites support web scrapping and have deployed '/robots.txt' URL extension to check if permission is required before scrapping data. I will also be completing some pre-processing to cleana and sanitise the data as much as possible.

Movie Meta Data - First set of data will contain a comprehensive collection of moevies meta data in pandas data frame scrapped from Internet Movies Database(IMDB).
Box Office Income Data - Second will contain commulative gross income for each title from the Numbers website.
in both of these website, the data is present in a number of consecutive pages starting from the initial page in which the required data is present in. Therefore my approach will be to to build a function which will scrape the data from the pages using BeauituflSoup and another which will crawl through the pages HTML structures and to collect all teh required URLs into one list which i can then use a loop to scrape the data from each URL and append to dataframe. With respect to IMDB, i will build a crawl function which will also append the production comapny name the URL and append to the dataframe for each movie.

The box office data observations are limited and not as expansive as the IMDB so will be performing an inner join with commulative box office sales globally.
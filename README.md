# IMDB-Script
Innovaccer Summer Intern Hiring Challenge - IMDB Script

The Script takes following input from users in the Input/Output Console:
1). User Name
2). Email address 
3). Favourite Shows Name

This is followed by storing these data into MySQL Database.

Now, the long string of TV_Series_input is split into Individual Series.

Now, web scraping for each individual series begins. :)
First, the series name having spaces, is replaced by '+' and search on IMDb occurs for the series name.
Now, we select the first search result and read from that page.

The current page is reading the series base page.
We will now read data from the latest season page of the series.

Now, using the BeautifulSoup4 library, we will gather the episode dates from class: "airdate".

Three cases of Series are:
1. Exact date is mentioned for next episode.
2. Only year is mentioned for next season.
3. All the seasons are finished and no further details are available.

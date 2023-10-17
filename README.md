# Files
- HW2.ipynb: Main notebook with all steps and intermediate results
- pipeline.log: Log file to track API hits of the ORES model
- json_data/: Folder with JSON dumps of the page info requests
- ores_json_data/: Folder with JSON dumps of the ORES model requests

- us_cities_by_state_SEPT.2023.csv: Crawled list of US cities inside states, taken from https://en.wikipedia.org/wiki/Category:Lists_of_cities_in_the_United_States_by_state     
- wp_scored_city_articles_by_state.csv: Results with merged datasets of cities, articles and population made according to HW schema
- NST-EST2022-POP.xlsx: Annual Estimates of the Resident Population for the United States, Regions, States, District of Columbia and Puerto Rico: April 1, 2020 to July 1, 2022 (NST-EST2022-POP), downloaded from https://www.census.gov/data/tables/time-series/demo/popest/2020s-state-total.html. 


- wp_ores_liftwing_example.ipynb: Sample notebook by Dr. David W. McDonald to illustrate requesting ORES data
- wp_page_info_example.ipynb: Sample notebook by Dr. David W. McDonald to illustrate requesting page info data


# Research Implications
A significant takeaway from this analysis was that despite the US being an economically and technologically advanced country, we see a lack of public articles and information about several regions across the country and a strong skew towards specific high population/highly dense regions, which might be for a variety of reasons. This sparks a follow-up research to conduct similar analyses on other countries in Europe, Africa, and Asia. Public data sources like Wikipedia suffer from implicit and explicit biases. In our case, the simple issue of a lack of articles about specific cities and states stands out, which is an implicit bias. The existence of explicit biases, such as ideological differences, would require further analysis.


- What biases did you expect to find in the data (before you started working with it), and why?
I expected significant cities with many inhabitants and higher population densities to have better articles because of higher contributions from interested parties. I also expected the larger states, especially those with a prolific economy, to have better quantity and quality of articles than economically backward and otherwise smaller states. 

- What (potential) sources of bias did you discover during your data processing and analysis?
One of the most significant sources of bias in an open-source, crowd-sourced data source like Wikipedia is the skewed interest of contributors. People tend to write articles and contribute to topics of interest. In our specific case, people will tend to write more about their cities for various reasons; they might be more interested in doing so or simply because their knowledge only goes as far as their surroundings. This kind of implicit bias is very apparent in our analysis. You might notice that states like Nebraska had yet to be mentioned in the earlier crawl to get names of cities.

- What might your results suggest about (English) Wikipedia as a data source?

Despite having biased data, Wikipedia is a publically available, barrier-free source of data with a plethora of information that would be ideal for making a foundational first-attempt analysis. Our analysis shows that Wikipedia is subject to some implicit bias of knowledge about certain cities/states not existing.



# LICENSE
The analysis uses data from Wikipedia and its use is covered under - Wikimedia Terms of use: https://www.mediawiki.org/wiki/API:REST_API#Terms_and_conditions

Other APIs used and their documentation:
- MediaWiki Action API: https://www.mediawiki.org/wiki/API:Main_page 
- ORES API: https://www.mediawiki.org/wiki/ORES

This work also has code written by Dr. David W. McDonald for use in DATA 512, a course in the UW MS Data Science degree program.

MIT License

Copyright (c) 2023 Vaibhav Mehrotra

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.


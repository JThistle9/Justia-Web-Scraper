# Justia-Web-Scraper
I needed the entire New York penal code in a single CSV to train a language model for an NLP task, but all I could find was https://law.justia.com/codes/new-york/2018/pen/part-3/ which has links to links to links to the citations. So, I built a web scraper in python to go through all the links, get the citations, format the text, and write it to a CSV file.

Most of the code was just me playing around and experimenting, but the last method called get_justia_penal_codes() is the final version of the function to write all of the citations to the csv

NOTE: the title/article/citation ids are arbitrary and merely represent the order in which they were taken. Order and id did not matter for training my language model, but if it matters for you then you should probably tweek my code.

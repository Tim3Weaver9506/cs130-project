# Methodology of My Process

## Data Source

1. I got elements-by-episode.csv straight from fivethirtyeight github page
1. I got bob_ross_paintings.csv from jwilber github page

## Data Cleaning/Preperation

1. The data sources on their own were fairly long, due to the amount of episodes that have been made (403). 
1. I started with the obvious, stripping the data for elements_by episode. From there, I converted the the bob_ross_paintings and elements by episode columns via pandas to make the indexes. 
1. The elements by episode columns includes only the elements whilst leaving out the episode title and number.
1. bob_ross_paintings columns was stripped of everything except the colors that were used in each episode.

## Assumptions
1. For my data, I wished to use the data to make it easier to search for episodes with certain themes and vice versa. Using the elements-by-episode.csv, I dont believe this was inconsistent with the logic of behind the indivduals who made this csv since I didnt alter the columns. 
1. For the bob_ross_paintings on the otherhand, I had to section the colmuns off on the csv since it contained information I didnt really need at all. 

## Limitations
1. The elements-by-episode.csv columns, especially with the episode name/number, made it a bit strange to use my function that finds elements based on the season + episode. Since the format goes like this (S01E01), I had to circumvent by adding a example in the input
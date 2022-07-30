# Use Case

The department of data analysts and content creation of the healthcare company you are working for are facing some challenging time in data retrieval from internet.
They need to scan lots of URLs and content to take some needed piece of information for further usage (marketing for example).
A team leader there approached you with a request for software that assists them in URL and webpage categorization to provide them a simple way to look things up.
After couple of calls/meetings you understand that they are talking about a simple `crawler` that ranks some pages according to the interest of content creation team. 

# Requirements

You are asked to design and implement a program that accepts a seed group of URLs as a JSON input file and perform the following:
- Categorization: After talking with the content creation team, you understand that they are interested in the following categories:
    - Sports
    - Food & Nutrition
    - Medical Articles
So your program would categorize URLs into three different categories.    

- Page Rank: You need to rank these URLs based on some importance metrics you understand from content creation team - listed accorind to importance:
    - Sports
        - `Walking` and `running` are the main sports to focus on at the coming period.
        - `Football` is another sport that they need to focus on.
    - Food & Nutrition
        - `Vegetables` and food that decreases depression would be an aim for the marketing department.
        - `Baby` nutrition is another subject of interest.
        - `Protein` relation to `muscle building`. 
    - Medical Articles
        - Sport injuries
        - Fat reduction operations.
        
- Search Support: Your program is also expected to provide a search feature based on rank. For instance, a content creator expected to get running URLs as first matches matches when looking for sport articles.

# Metrics

Ranks are to be determined by:
- Phrase/Word Frequency
- Article Length

`Hint: Phrase frequency is stronger than length as a metric`

# Expected Rank

- Sports 
    - `Walking` and `running`
        - Rank 1:
            - URL_1
            - URL_2
            - URL_3
        - Rank 2:
            - URL_1
            - URL_2
    - `Football`
        - Rank 1:
            - URL_1
            - URL_2
            - URL_3
        - Rank 2:
            - URL_1
            - URL_2
    and so forth...
# Revenue_assessment
A tab seperated hit file (data.tsv) is input file which is placed in S3 bucket. This file contains hit level record information from a visitor on Client side. A lambda function is written to automatically trigger when the file is placed in S3 bucket. This function processes the file and returns the solution to Business problem as a tab separated file with naming convention as [Date]_SearchKeywordPerformance.tab where Date format is YYYY-mm-dd. This output has Search Engine Domain, Search Keyword and Revenue (descending order) information. This output file is placed in another S3 bucket.

# Business Problem
How much revenue is the client getting from external Search Engines, such as Google, Yahoo and MSN, and which keywords are performing the best based on revenue?

# Findings
It was observed that revenue generated from search engines based on data was 730. Google.com was the better performing search engine with 'Ipod/ipod' as the keyword resulting in actual sales. It was also observed that users using Mac machines were searching and completing purchase for more apple products (ipod) as compared to non Mac users.

# Future Considerations
Due to limitations in the data sample that was provided, further analytics were not performed. Funnel analysis could be done on the data to check where the drop of users is happening in the process, improve the experience and increase the sales and overall revenue for client.

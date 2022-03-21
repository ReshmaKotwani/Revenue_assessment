# Revenue_assessment
A tab seperated hit file (data.tsv) is input file which is placed in S3 bucket. This file contains hit level record information from a visitor on Client side. A lambda function is written to automatically trigger when the file is placed in S3 bucket. This function processes the file and returns the solution to Business problem as a tab separated file with naming convention as [Date]_SearchKeywordPerformance.tab where Date format is YYYY-mm-dd. This output has Search Engine Domain, Search Keyword and Revenue (descending order) information. This output file is placed in another S3 bucket.

# Business Problem
How much revenue is the client getting from external Search Engines, such as Google, Yahoo and MSN, and which keywords are performing the best based on revenue?

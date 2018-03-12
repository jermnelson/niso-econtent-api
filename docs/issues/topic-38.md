#  Web awareness of Library System
The vendor systems should provide robot.txt for indexing by 
[Google](https://google.com/),  [Bing](https://bing.com/), and 
other web indexers

## Comments from [Best Practice Review][BEST_PRACTICES] Topic ID #38
As much as possible, the patrons should be using or taken to a 
library-branded interface so they are not concerned with privacy or 
quality issues.

Library applications should have specialized SEO APIs that can be 
used to generate robots.txt and meta tags for increased SEO 
friendliness of OPAC and Discovery layers.

## FASTEN Alignment with [ResourceSync][RS]
As [ResourceSync][RS] extends the [Sitemap](https://www.sitemaps.org/protocol.html) 
protocol, the FASTEN recommendation is to support the following REST verbs:

*   A **GET** request for `/sitemap.xml` returns a valid and 
    well-formed xml document containing urls to available resources
*   A **GET** request for `/sitemapindex.xml` returns a valid
    and wel-formed xml document listing all of the available site maps
    published by the vendor. 


[BEST_PRACTICES]: https://docs.google.com/spreadsheets/d/1iQrdLVUSCW-0FWlrKNGjZJkB8nPO5Z94pg1Ie8GIKhg/
[RS]: http://www.openarchives.org/rs/toc

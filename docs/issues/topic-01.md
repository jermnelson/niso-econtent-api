# Path to Resource

##  Comments from [Best Practice Review][BEST_PRACTICES] Topic ID #1
Path from finding a resource to accessing it should be intuitive, 
seamless and offer few/no barriers to the end user.  The user should 
not have to leave the environment in which the resource was found. 
The resource should be displayed within the library catalogue/discovery 
layer and should not be taken to a third party website, e.g., publisher 
or aggregator site.

## FASTEN Alignment with [NCIP][NCIP]

*   A **POST** request with an NCIP Item Id or Request Id and returns optional
    data by requesting agent. Aligns with [NCIP][NCIP] 
    [5.3.2 Lookup Item Service](http://www.ncip.info/uploads/7/1/4/6/7146749/z39-83-1-2012_ncip.pdf#page=8)


## FASTEN Alignment with [LCF][LCF]

Could be inplemented via an extension to the [E04 LOCATION record](https://github.com/anthonywhitford/bic-lcf/wiki/LCF-1.0.1-Information-Entity-XML-bindings#e04-location)

## FASTEN Alignment with [BIC Library Web Services][BICWS]

## FASTEN Alignment with [OpenID][OID]

Not applicable

## FASTEN Alignment with [ResourceSync][RS]

*   A **GET** request to a resource linked from a `/sitemap.xml` should be a url with a stable and
    seemless path.
    

[BEST_PRACTICES]: https://docs.google.com/spreadsheets/d/1iQrdLVUSCW-0FWlrKNGjZJkB8nPO5Z94pg1Ie8GIKhg/
[OID]:  https://openid.net/
[NCIP]: http://www.ncip.info/ 
[RS]: http://www.openarchives.org/rs/toc
[LCF]: http://www.bic.org.uk/114/Library-Communications-Framework-(LCF)/
[BICWS]: http://www.bic.org.uk/files/pdfs/Library%20Web%20Services%20TandFWG%20Project%20Brief_Final%20v.1.1.pdf


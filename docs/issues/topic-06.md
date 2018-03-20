# DRM Authentication 

##  Comments from [Best Practice Review][BEST_PRACTICES] Topic ID #6
Media should allow for Library/Open Source readers that allow DRM 
authentication

## FASTEN Alignment with [NCIP][NCIP]

*   A **POST** request to a [5.4.3 Check-out Item Service](http://www.ncip.info/uploads/7/1/4/6/7146749/z39-83-1-2012_ncip.pdf#page=16) returns a
    Problem response of *Required Item Use Restriction Type* or
    a *Required Fee Amount* 

## FASTEN Alignment with [LCF][LCF]

## FASTEN Alignment with [BIC Library Web Services][BICWS]

## FASTEN Alignment with [OpenID][OID]

*   A **GET** request to the system with either a `code`, `token`, or `id_token` to an authorization
    server will return a `access_token`, `token_type`, `id_token`, and an optional `expires_in`.
    From this [5. Definitions of Multiple-Valued Response Type Combinations](http://openid.net/specs/oauth-v2-multiple-response-types-1_0.html#rfc.section.5). If user is not authorized to access the resource, a `None` response is given.

## FASTEN Alignment with [ResourceSync][RS]
Not applicable

[BEST_PRACTICES]: https://docs.google.com/spreadsheets/d/1iQrdLVUSCW-0FWlrKNGjZJkB8nPO5Z94pg1Ie8GIKhg/
[OID]:  https://openid.net/
[NCIP]: http://www.ncip.info/ 
[RS]: http://www.openarchives.org/rs/toc
[LCF]: http://www.bic.org.uk/114/Library-Communications-Framework-(LCF)/
[BICWS]: http://www.bic.org.uk/files/pdfs/Library%20Web%20Services%20TandFWG%20Project%20Brief_Final%20v.1.1.pdf


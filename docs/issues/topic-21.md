# Personal patron information 

##  Comments from [Best Practice Review][BEST_PRACTICES] Topic ID #21
No personal patron information should move from the identity provider 
(or ILS or discovery layer) to a third-party eContent vendor.  That way 
there's no potential for abuse.

## FASTEN Alignment with [NCIP][NCIP]

*   A **POST** request with a [NCIP][NCIP] User Id or Authentication Input with optional
    data is restricted to outputs defined in 
    [5.3.4 Lookup User Service](http://www.ncip.info/uploads/7/1/4/6/7146749/z39-83-1-2012_ncip.pdf#page=10). 

## FASTEN Alignment with [OpenID][OID]
*   A **GET** request to the system with either a `code`, `token`, or `id_token` to an authorization
    server will return a `access_token`, `token_type`, `id_token`, and an optional `expires_in`.
    From this [5. Definitions of Multiple-Valued Response Type Combinations](http://openid.net/specs/oauth-v2-multiple-response-types-1_0.html#rfc.section.5). No other personal information is transmitted to the vendor.

## FASTEN Alignment with [ResourceSync][RS]
Not applicable


[BEST_PRACTICES]: https://docs.google.com/spreadsheets/d/1iQrdLVUSCW-0FWlrKNGjZJkB8nPO5Z94pg1Ie8GIKhg/
[OID]: https://openid.net/
[NCIP]: http://www.ncip.info/ 
[RS]: http://www.openarchives.org/rs/toc


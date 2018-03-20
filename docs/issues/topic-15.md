# Checkouts should apply at the "title" level 
This references Topic 16 from the [Best Practices][BEST_PRACTICES] document.
(A "title" in this context may be better understood in a Linked-Data
context as a BIBFRAME Item).


## FASTEN Alignment with [NCIP][NCIP]

*  A **POST** request to a [5.4.3 Check-out Item Service](http://www.ncip.info/uploads/7/1/4/6/7146749/z39-83-1-2012_ncip.pdf#page=16)
   with a [NISO][NISO] User Id or Authentication Input and an Item Id  
   returns an *Item Id*, *User id*, and ether a *Date Due*, *Indeterminate Loan Period Flag*, or *Non Returnable Flag*. 

## FASTEN Alignment with [LCF][LCF]

(See [11 Check-out / Renewal](https://github.com/anthonywhitford/bic-lcf/wiki/LCF-1.0.1-REST-Web-Service-Specification#11-check-out--renewal))

A new check-out is performed by creating a new loan record, using LCF function 03 (see above), e.g.

```
POST http://192.168.0.99:80/lcf/1.0/loans
```

An XML document that conforms to the XML schema for a loan entity (E05) must be uploaded with the request.

The response to a check-out or renewal may be the same response as for creating any entity, i.e. 
status code 201 (Created) and a Location field in the HTTP header, or it may contain an XML payload,e.g.
```
<lcf-check-out-response xmlns="http://ns.bic.org/lcf/1.0">
 <loan-ref>http://192.168.0.99:80/lcf/1.0/loans/1234567890</loan-ref>
 <sensitive-media-warning>00</sensitive-media-warning>
</lcf-check-out-response>`
```

## FASTEN Alignment with [BIC Library Web Services][BICWS]

## FASTEN Alignment with [OpenID][OID]
Not applicable

## FASTEN Alignment with [ResourceSync][RS]
Not applicable

[BEST_PRACTICES]: https://docs.google.com/spreadsheets/d/1iQrdLVUSCW-0FWlrKNGjZJkB8nPO5Z94pg1Ie8GIKhg/
[NCIP]: http://www.ncip.info/ 
[OID]: https://openid.net/
[RS]: http://www.openarchives.org/rs/toc
[LCF]: http://www.bic.org.uk/114/Library-Communications-Framework-(LCF)/
[BICWS]: http://www.bic.org.uk/files/pdfs/Library%20Web%20Services%20TandFWG%20Project%20Brief_Final%20v.1.1.pdf


CONTENTdm
================================

## COMMAND CHEAT SHEET
If you want to check specific records for the existence of a WC number, I'd suggest the CDM API.  
Parse the output for a record for the dmoclclo value.  
e.g.:  https://server17142.contentdm.oclc.org/dmwebservices/index.php?q=dmGetItemInfo/p17142coll5/1/json

If you want to create a "report" listing all of the CDM items and any corresponding dmoclcno values without creating an API call for every record, then I'd start by pulling down the main metadata file for the collection, then parse it. e.g.  http://server16007.contentdm.oclc.org/cgi-bin/getdesc.exe?CISOROOT=/p16007coll1&CISOOP=desc

You can see the corresponding field definitions for a collection using a "CISOOP=config" URL:
http://server16007.contentdm.oclc.org/cgi-bin/getdesc.exe?CISOROOT=/p16007coll1&CISOOP=config

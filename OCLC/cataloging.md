OCLC - Cataloging
================================

## Encoding Levels
* Align OCLC-MARC encoding levels with MARC 21's
* OCLC cataloging libraries may now use most MARC21 and OCLC codes:
  * -- blank, 1, 2, 3, 4, 5, 7, 8 or K
* Previously, OCLC cataloging participating libraires could only enter records with I -- Full Level, K -- Minimal Level, or 3 -- Abbreviated Level
* Libraries are encouraged to use blank instead of I for Full level and 7 instead of K for Minimal level cataloging

## RECORD MANAGER CHEAT SHEET


| How to find...           |                                   |                   | 
|--------------------------|-----------------------------------|-------------------|
| All records              | li:OHI                            |                   |
| All records without LHRs | li:OHI NOT l4:OHI                 |                   |
| All journals             | li:OHI AND x0:Jrnl                | li:OHI AND mt:ser |
| All print journals       | li:OHI AND x0:Jrnl NOT x4:Digital |                   |
| All books                | li:OHI AND x0:Book                |                   |
| All eBooks               | li:OHI AND x0:Book AND x4:Digital |                   |
| All print books          | li:OHI AND x0:Book NOT x4:Digital |                   |
| All videos               | li:OHI AND x0:Video               |                   |
| ---                      |                                   |                   |
| Limit by year            | li:OHI AND yr:2000-2014           |                   |
| Ohio Memory records      | li:OHI AND am:ohiomemory          |                   |

| Material Types |                                 |
|----------------|---------------------------------|
| ser            | Serials                         |
| per            | Periodicals (subset of Serials) |
| bks            | Books                           |
| ebk            | eBooks (subset of Books)        |
| vis            | Visual Materials                |
| dvv            | DVDs                            |
| url            | Electronic                      |

| Holdings |                              |
|----------|------------------------------|
| li       | Institutional holdings       |
| l4       | Institutional local holdings |
| zu       | Group holdings               |
| l5       | Group local holdings         |

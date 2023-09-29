Alma - Cataloging
================================

# 001 / 003 / 035

**Q:** Why do some records have two OCLC / 035 fields for example, let’s say this record had just one OCLC number like many records I see but one field would be ‡a (OCoLC)1227789882 and the other one is ‡a (OCoLC)on1227789882 or ‡a (OCoLC)ocn1227789882.  What do the letters mean?

**A:** I suspect that your ILS is Alma.  Alma puts its own identifier into the 001 field when importing into their system (as is proper).  To retain the original 001 information, Alma will create a new 035 field by putting the 003 field value in parentheses and following it by the 001 field value.  As indicated by Cynthia, OCLC records have 001 values which are preceded by ocm, ocn, and on, and 003 values of OCoLC.  This results in an 035 field with a value like (OCoLC)on1227789882 in Alma records derived from OCLC.  Alma will also copy the values in the 019 field into 035 fields.  As you suspected, the 019 field is a record OCLC keeps of the OCLC numbers merged into the current record.

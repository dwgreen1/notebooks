YAZ-CLIENT
==========

Install Homebrew

```bash
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

Install Yaz

```bash
brew install yaz
```


Read the [YAZ Docs](http://www.indexdata.com/yaz/doc/), [find a z39.50 target](http://irspy.indexdata.com/), review [bib-1 attribute set](https://www.loc.gov/z3950/agency/defns/bib1.html), and give it a whirl.


```bash
# start Yaz connection to Library of Congress z39.50
# z39.50 server is running on port 7090, via voyager
yaz-client z3950.loc.gov:7090/voyager

# open the connection for searching
open z3950.loc.gov:7090/voyager

# Send a boolean query
find @and cats hot

# Use Bib-1 Attributes (find "" in 245)
find @attr 1=4 "rocco di pietro"

# Use Bib-1 Attributes to search ISBN
find @attr 1=7 "9780674015432"

# Return one record
s 1

# Change record format
format xml
format marc21

# Display client settings
list_all

# capture records in file
set_marcdump /Users/Derek/Desktop/download.mrc

# find available commands and options
help

# close the connection
close

# Exit the client
exit

```
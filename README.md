# doc-it
Document generator for (in theory) any programming language with comments

primairaaly for c though

I will add suport for uthor languages like python and javascript (not java because they have their own and are pretty close to c anyways)


## Base concept:

char * comment = "//" // example in c (can be anything eg. # for python)

comment + ">" 

will indicate a start of a comment header
(ex: //> Title: title of comment block)

comment + "."

will indicate a continuation of a comment
(ex: //. title is continued on the next line)

comment + "<"

will indicate the end of a comment
(ex: //<) 

## Headers

### Mandatory
Title: gives the name of the comment block 

### Optional
#### functional
in the form 
type name:
description

Args: describes arguments of the function (will find type and display it if possible)
Returns: describes the return value (will find type and display it if possible)

#### other
any header in the form "Header: " will be accepted and displayed in the form 

Header:
description

tag options will be available
-c "comment" will set the comment 
-l "language" will set language (might be useful later for Args and Returns headers, also class headers when I add those)

others when I think of them 


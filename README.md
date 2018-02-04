
## URI definition :
    
 - URI is a string of characters that identifies a resource. 
 - also URI is a refrence that points to the actuall data/resource.
 
## formal format of URI: 
   #### Scheme:[//[user:password@]host[:port]] [/]path[?query][#fragment]
(anything between square the brackets is optional).

## Breakdown of URI:
-so URI can be broken down into 5 parts given below.
 - Scheme =  scheme describe what type of resource we are pointing to (eg mailto ,geo,https).
 - authority= authority is the part where we describe user name,password and host.
 - path=      path is further navigation to resource eg (/courses/ud851/lessons..)
 - query=     query is used to filter the resource.
 - fragment=  fragment contains data used by path of query.    
 
 ## Rules for building legitmate URI:
 
 ### Identify which part of URI is optional
 
 - Scheme     = Not Optional
 - authority  = Optional
 - path       = Not Optional
 - query      = Optional
 - fragment   = Optional
 - if authority is present than path should be preceded by "/" ,otherwise its optional.
 
 #### inside Authority
 - Authority has 3 parts
 - UserName and password = Optional
 - host = Not optional
 - port=  Optional
 - "//" in start = Not Optional
 
 ##### inside "UserName and Password"
 - userName =Not optional
 - password=Not optional
 - "UserName and Password" ends with "@" character.
 ##### inside "Port"
 - port = Not Optional
 - ":" in start = Not Optional
 
#### inside query
- query = Not Optional
- "?" in start = Not Optional

#### inside fragment
- fragment = Not Optional
- "#" in start = Not Optional

## Some example types
 - Content URI , has scheme content ,A content URI is a URI that identifies data in a provider .
 - formal format #### content://authority/path/id
 - #### content://user_dictionary/words
 
 - geo URI
 - formal formate #### geo:latitude,longitude?z=level
 - #### geo:0,0?q=Antwarp,Belgium & Z=10 
 - geo URI has scheme geo:
 - in above URI example geo is scheme ,geo scheme describes that the resource/data type to which this URI points is a physical location.
 - in above example scheme geo: is followed by path 0,0 . 0,0 is latitude and longitude .its 0,0 because according to rules if
 - we decribe a string address than lat and long should be 0,0.    
 - their is not authority in above example because we don't need it also authority is optional.
 
 ### Are geo URI and Content URI legitmate URI's ?
 - lets find out 
 - general URI format #### Scheme:[//[user:password@]host[:port]] [/]path[?query][#fragment]
 - content URI format #### content://authority/path/id
 - content URI exampe #### content://user_dictionary/words
 
 - geo URI format #### geo:latitude,longitude?z=level
 - geo URI example #### geo:0,0?q=Antwarp,Belgium & Z=10  
 -
 

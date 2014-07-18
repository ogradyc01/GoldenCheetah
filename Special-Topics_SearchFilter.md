Special Topics: Search & Filter (Version 3.1)
****

## Search

The 'Search' function in GoldenCheetah is pretty straight forward. All texts in rides are automatically indexed when a ride is imported or changed. If 'Search' is active (check if the right Icon - "magnifying glass" is shown) and just enter the text you are search for. The ride list will be reduced/filtered to those rides where the text appears.

The search engine used by GoldenCheetah offers more options - e.g. field specific searches. Some of them which might be helpful (and which appear to work in GoldenCheetah's way to use the search engine) are:

* Wildcard searches 
  * Single character wildcard is "?"
  * Multiple character wildcard is "*"

_Note: Using a wildcard charater as first character of a search is not possible._

* Boolean operators
  * `AND` or `&&` - to find rides where both term exists
  * `OR` or `||` - to find rides where any of the terms exist

_Note: Here AND, resp. OR have to be in UPPER CASE - otherwise they are interpreted as search terms_

_Note: Since the search engine has more capabilities - there may be more usable, but since the documentation on the query snytax is quite basic, you need to find out on your own. A usefull search term to get further information is the name of the search engine used: 'Lucene' and the implementation GoldenCheetah is using is 'CLucene'._
  

## Filter


## Filter Syntax 

* String Functions
  * `MATCHES`
  * `BEGINSWITH`
  * `ENDSWITH`
  * `CONTAINS`

* Value Operator
  * `=`
  * `<>` 
  * `<`
  * `<=`
  * `>`
  * `>=`

* Logical Operator
  * `&&` or `AND`
  * `||` or `OR`

* Calculation Operator
  * `+`
  * `-`
  * `*`
  * `\`
  * `^`

* Special Functions
 * `BEST`apower|power|hr|cadence|speed|torque|vam|xpower|np|wpk (BEST ( xx, DURATION in seconds) returns 0 
 * `TIZ` power|hr (Time in Zone-> TIZ ( xx, ZoneNumber) return float value (seconds)
-> Check "RideFileCache" for further details

* Constants 
 * Integer - format examples `12345`, `-12345`
 * Float - format examples `1234e-3`
 * String - format example `abcde`

* GoldenCheetah Symbols
 * Names of GoldenCheetah metrics which can be used on formulas (most, but not all field are supported yet - e.g. there is no support for Date or Time fields in formulas) 

 

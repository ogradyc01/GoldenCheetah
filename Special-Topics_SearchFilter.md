Special Topics: Search & Filter (Version 3.1)
****

## Search

The 'Search' function in GoldenCheetah is pretty straight forward. All texts in rides are automatically indexed when a ride is imported or changed. If 'Search' is active (check if the right Icon - "magnifying glass" is shown) and just enter the text you are search for. The ride list will be reduced/filtered to those rides where the text appears.

The search engine used by GoldenCheetah offers more options - e.g. field specific searches. Some of them which might be helpful (and which should work) are:

* Wildcard searches
  * Single character wildcard is "?"
  * Multiple character wildcard is "*"
_Note: Using a wildcard charater as first character of a search is not possible._





 - but since this is not very well documented, and the simple search is considered to cover pretty much all

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

 

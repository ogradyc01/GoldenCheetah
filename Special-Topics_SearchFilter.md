Special Topics: Search & Filter (Version 3.1)
****

## Search & Filter - Common Functions

Before going into any details, here the common functions available for both Search and Filter queries. The logic for Search and Filter is similar in all places of GoldenCheetah:

### UI Handling

The UI is multifunctional. It has a selector to switch between 'Search' and 'Filter', a drop-down menu contain the pre-defined queries and related functions, and an input field to enter your queries.

_Note: Please do always check if you have selected the right type for your query 'Search' or 'Filter' as they have a slightly different query syntax and purpose and will most likely create unexpected results._

![Search Filter - UI] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/Search_Filter_UI.gif)

### Manage Filters (Manage Queries)

You can create and store 'Search' and 'Filter' queries using the 'Manage Filters' menu. Queries stored here are appear in the drop-down menu for faster access.

![Search Filter - ManageFilters] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/Search_Filter_ManageFilters.jpg)

* Add - adds the query defined in the Name/Filter input field to the list
* Update - updates an existing query with changes from Name/Filter input fields
* Delete - delete the query marked in the list

_Note: Again be sure to use the correct query type (Search/Filter)._

### Applying Queries

You can always just enter the query into the text field and press `Enter` to apply the query. By using pre-defined queries you save the time for typing and get always the same result (without any typing errors.)

![Search Filter - Apply/Remove] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/Search_Filter_Apply_Remove.gif)

_Note:To de-activate a 'Search/Filter' query, just click on the little (x) on the right end of the text box._

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
 * `BEST`apower|power|hr|cadence|speed|torque|vam|xpower|np|wpk 
   (BEST ( xx, DURATION in seconds) return the value (power,...) which is the meanMax for the duration (basically the data from the CP chart for that duration) which then still needs a comparison again a constant to filter the rides
 * `TIZ` power|hr (Time in Zone-> TIZ ( xx, ZoneNumber) return float value (seconds) which then can be used in comparison (1h = 3600 seconds)

* Constants 
 * Integer - format examples `12345`, `-12345`
 * Float - format examples `1234e-3`
 * String - format example `abcde`

* GoldenCheetah Symbols
 * Names of GoldenCheetah metrics which can be used on formulas (most, but not all field are supported yet - e.g. there is no support for Date or Time fields in formulas) 

 

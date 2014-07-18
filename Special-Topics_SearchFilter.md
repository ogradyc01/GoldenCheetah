Special Topics: Search & Filter (Version 3.1)
****

Searching and Filtering are ways to find rides which fulfill specific criteria (e.g. to limit the number of rides shown in the ride navigator - or to find a particular ride). But also to only consider specific rides in summary and cumulative charts, like on the 'Trends' view.

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

You can always just enter the query into the text field and press `Enter` to apply the query. Or use a pre-defined queries which applies directly and saves the time of typing.

![Search Filter - Apply/Remove] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/Search_Filter_Apply_Remove.gif)

_Note:To de-activate a 'Search/Filter' query, just click on the little (x) on the right end of the text box._

## Search

The 'Search' function in GoldenCheetah is pretty straight forward. All texts in rides are automatically indexed when a ride is imported or changed. If 'Search' is active (check if the right Icon - "magnifying glass" is shown) and just enter the text you are search for. The ride list will be reduced/filtered to those rides where the text appears.

### Search Query Syntax

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

Filtering is like searching, a way to find rides which fulfill specific criteria. Where searching mainly works on text fields, filtering can do a lot more. But this 'more' also means you have to make yourself familiar with the query syntax for filtering.

### Filter Query Syntax 

In a simple view, a filter query is a bit like a database query - (which is different to free-text search engines). As a minimum you need to define

  * the field you want to look at
  * a rule how to look at that field
  * a comparison value

Easy example: The query `TSS >= 100` - finds all rides where TSS is 100 or more. And this example already illustrates the major point of what a 'Filter' can do better than a 'Search'. You will not define a search which can do this. (But, also 'Filter' queries cannot do it all and easy. E.g. 'Search' makes absolutely sense for text fields and is perfect if e.g. you do not even know in which field you have stored your text - 'Search' will find it.)

## A simple query looks like: `<field_name> <operator> <value>`

### `<field_name>`

GoldenCheetah uses a "semi"technical field name for the queries - which is basically the english metric name, where all 'spaces' are substited by '_' to get the <field> as one textstring. Since it's difficult to remember all the field names, and for longer field names to type the name correctly, you can "Drag&Drop" field field name in the required format using the 'Column Chooser' tool. (It's in the filter menu - next to 'Manage Filter').

_Note: In releases below 3.1 the field names were partly translated into your preferences - language. Depending on the use of "special characters" in the translated field names, the filtering on such field partly worked, partly not. In order to be independent on of translation, from 3.1 on, only the english fieldnames (as described above) are valid <field_name>s for 'Filter' queries._

### `<operator>`

* Strings and String Functions
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


## A more complex query: `<field_name> <operator> <value> AND <other_field> <o`

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

 

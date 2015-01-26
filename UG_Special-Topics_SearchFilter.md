Special Topics: Search & Filter (Version 3.11) 
****

Searching and Filtering are ways to find rides which fulfill specific criteria (e.g. to limit the number of rides shown in the ride navigator - or to find a particular ride). But also to only consider specific rides in summary and cumulative charts, like on the 'Trends' view.

## Search & Filter - Common Functions

Before going into any details, here the common functions available for both 'Search' and 'Filter' queries. The logic for 'Search' and 'Filter' is similar in all places of GoldenCheetah:

### UI Handling

The input box for 'Search/Filter' functionality contains multiple functions. It has 
* a selector to switch between 'Search' and 'Filter' mode, 
* a drop-down menu contain the pre-defined queries and related functions, 
* and is the text input field to enter your queries.

_Note: Please do always check if you have chosen the right type for your query 'Search' or 'Filter' as they have a slightly different query syntax and purpose._

![Search Filter - UI](https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/Search_Filter_UI.gif)

### Manage Filters (Manage Queries)

You can create and store 'Search' and 'Filter' queries using the 'Manage Filters' menu. Queries stored here  appear in the drop-down menu for faster access.

![Search Filter - ManageFilters](https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/Search_Filter_ManageFilters.jpg)

* `Add`- adds the query defined in the Name/Filter input field to the list
* `Update` - updates an existing query with changes from Name/Filter input fields
* `Delete` - deletes the query selected in the list

_Note: Please be sure to use the correct query type (Search/Filter)._

### Applying Queries

You can always just enter the query into the text field and press `Enter` to run the query. Or use a pre-defined queries which applies directly and saves the time of typing.

![Search Filter - Apply/Remove](https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/Search_Filter_Apply_Remove.gif)

_Note:To de-activate a 'Search/Filter' query, just click on the little (x) on the right side of the input field._

## Search

The 'Search' function in GoldenCheetah is pretty straight forward. All texts in rides are automatically indexed when a ride is imported or changed. If 'Search' is active (check if the correct icon - "magnifying glass" is shown) and just enter the text you are search for. The ride list will be reduced/filtered to those rides where the text appears in any of the text fields.

### Search Query Syntax

The search engine used by GoldenCheetah offers more options. Some of them which seem to be helpful (and which appear to work in GoldenCheetah's implementation to use the search engine) are:

* Wildcard searches 
  * Single character wildcard is "?"
  * Multiple character wildcard is "*"

_Note: Using a wildcard charater as first character of a search query is not possible._

* Boolean operators
  * `AND` or `&&` - to find rides where both term exists
  * `OR` or `||` - to find rides where any of the terms exist

_Note: Here AND, resp. OR have to be in UPPER CASE - otherwise they are interpreted as search terms_

_Note2: The search engines operators are considered as "reserved" words, so that they cannot be found if you are looking for them - known cases are - "NOT", "AND", "OR", "TO" as well as "*", "?", "+", "-", but there may be more.

_Note3: Since the search engine has more capabilities - there may be more usable, but since the documentation on the query snytax is quite basic, you need to find out on your own. A usefull search term to get further information is the name of the search engine used: 'Lucene' and the implementation GoldenCheetah is using is 'CLucene'._
  
## Filter

Filtering is like searching, a way to find rides which fulfill specific criteria. Where searching mainly works on text fields, filtering can do a lot more. But this 'more' also means you have to make yourself familiar with the query syntax for filtering.

### Filter Query Syntax 

In a simplified way, a filter query is a bit like a database query - (which is different to free-text search engines). As a minimum you need to define

  * the field you want to look at (FieldName)
  * a rule how to look at that field (Operator)
  * a comparison value (Value)

Easy example: The query `TSS >= 100` - finds all rides where TSS is 100 or more. This example already illustrates the major point of what a 'Filter' can do better than a 'Search'. You cannot define a search which can do this (in GoldenCheetah). (But, also 'Filter' queries cannot do it all and easy. E.g. 'Search' makes most sense for text fields and is perfect if e.g. you do not even know in which field you have stored your text - 'Search' will find it.)

_Note: You need to separate field names, operator, keywords, function as well as values or string by " " (Space) so that the query parser can recognize them - otherwise you will see the query text color changing to "red". To see the error text, just click into the query text and wait until an error text appears._

## Simple Queries

A simple query is structured: `<field_name> <operator> <value_or_string>`

### `<field_name>`

GoldenCheetah uses a "semi"technical field name for the queries - which is basically the english metric or field name, where all 'spaces' are substited by '_' to get the `<field>` as one textstring. Since it's difficult to remember all the field names, and (for longer field names) to type the name correctly, you can "Drag&Drop" field name in the required format using the 'Column Chooser' tool. (It's in the filter menu - next to 'Manage Filter').

_Note: In releases before 3.1 the field names were partly translated into your "preferences - language". Depending on the use of "special characters" in the translated field names, the filtering on such field partly worked, partly not. In order to be independent of any translation, from 3.1 on, only the english fieldnames (as described above) are valid <field_name>s for 'Filter' queries._

### `<operator>`

* Text Operators (make only sense for text fields/strings)
  * `MATCHES` - checks if the field text has a exact match with the regular expression in `MATCHES(<reg_expr>)`
  * `BEGINSWITH` - checks if the field text begins with the text you are comparing to
  * `ENDSWITH` - checks if the field text ends with text your are comparing to
  * `CONTAINS` - checks if the field text at any position contains the text you are comparing to

* Value Operator (work for value fields and text fields)
  * `=` - Equal
  * `<>` - Not equal
  * `<` - Smaller
  * `<=` - Smaller or equal
  * `>` - Greater
  * `>=` - Greater or equal

_Note: For text fields mainly `=` and `<>` make sense, comparison of text on 'greater' or 'smaller' works as well, but uses the character codes to compare_

### `<value_or_string>`

* `<string>` can be a single word, or a sequence of words (which then need to be put into quotes "" or '')
* `<value>` can be an 'integer' (like 123 or -456) or a 'float' (like 123.567 or -123.456 or 123.567e3 or 123.567e-3 )

## Combined Queries

You can combine multiple simple queries with 

* Boolean operators
  * `AND` or `&&` - both simple queries have to be fulfilled 
  * `OR` or `||` - either one or both simple queries have to be fulfilled

_Note: This can be done as often as the query input field allows for a text size perspective. In contrast to the 'Search' queries, the filter queries don't care on upper/lower case for the operator keywords._

* Using bracket "(" ")" - in more complex queries it is often either required / and useful to put certain sub-query or calculations in brackets - so that execution is done in the right sequence. 

### Special Operators

In addition to the quite common operators before, GoldenCheetah has some build-in extras you can use.

* Calculation Operators
  * `+` - plus
  * `-` - minus
  * `*` - multiply
  * `\` - divide
  * `^` - power

The syntax is `<value_or_field> <calculation_operator> <value_or_field>`. With this you can create queries like: "show me all rides where the sum of L2_Time and L3_Time is more than 2 hours: `( L2_Time_in_Zone  + L3_Time_in_Zone ) > 7200`. Please note that duration fields (here 2h) are always assumed to contain their value in "seconds" (here 7200 seconds).

## Special Functions

GoldenCheetah provides two functions which return rides specific metrics very easily:

 * `BEST` - syntax is `BEST ( <data_series>, <duration)` and returns the MEAN MAX value of the chosen data series for the ride to filter. This value then can be used in a query e.g. to compare to a <`value>`.

The supported `<data_series>` are: "apower", "power", "hr", "cadence", "speed", "torque", "vam", "xpower", "np", "wpk" 

Example: You want to select all rides, where your 5min mean max power was higher than 200 watts. This query then looks: `BEST ( power, 300) > 200`. Again the duration (5min) has to be entered in seconds (300sec) into the query.

 * `TIZ` - (Time in Zone) - syntax is `TIZ ( <tiz_series>, <zone>)` and returns the time you have spend in a particular zone for the rides to filter. This value then needs to be used in the complete query e.g. to compare to a `<value>`.

The supported `<tiz_series>` are: "power" and "hr"

Example: You want to select all rides, where you have spend 60min or more in power zone 4. This query then looks: `TIZ ( power, 4 ) > 3600`. Again the duration (60min) has to be entered in seconds (3600sec) into the query.

### NEW with 3.11

 * `SB` - (Stress Balance) - syntax is `SB(<metric>)` and returns the PMC value for the metric in question for the date of the ride and therefore allows to select rides based upon PMC data.

 * `LTS` - (Long Term Stress) - syntax is `LTS(<metric>)` and returns the PMC value for the metric in question for the date of the ride and therefore allows to select rides based upon PMC data.

 * `STS` - (Short Term Stress) - syntax is `STS(<metric>)` and returns the PMC value for the metric in question for the date of the ride and therefore allows to select rides based upon PMC data.

The supported `<metric>` are e.g. `TSS`, and the similar ones.

## Additional Information

* Duration fields and values - always have to be provided in "seconds" in a query.
* Date and Time fields - are currently not supported in the queries - for some needs you may use 'Date Ranges' instead
* Some technical fields are also not supported - when you enter such a field with the 'Column Chooser' you will get a 'syntax error' e.g. "field not known".
* Syntax errors - when a query is invalid, the query input field text color changes to "red". By clicking at any part of the query text with your mouse and waiting a short moment, an error text will appear, telling you why GoldenCheetah failed to parse your query. 

BACK: [Special Topics: Overview](https://github.com/GoldenCheetah/GoldenCheetah/wiki/UG_Special-Topics_Overview)  
BACK: [Table of contents](https://github.com/GoldenCheetah/GoldenCheetah/wiki/UG_Main-Page_Table-of-contents)
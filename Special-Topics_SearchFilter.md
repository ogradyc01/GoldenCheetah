Special Topics: Search & Filter (Version 3.1)
****



## Filter Syntax 

* String Operator
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

 

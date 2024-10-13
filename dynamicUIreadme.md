# dynamic UI, based on JSON file

## json structure for UI

### json fields

1. fieldname - name of field in data source
2. fieldlabel - Label in UI
3. fieldtype - string, integer(whole number), float(decimals), boolean, date, datetime, email, url , password, blob, array
   - string - textbox, maxlength property
   - ineger - html type number with min, max - default to integer min max
   - float - tdb
     - consider number of decimal position
   - boolean - checkbox
   - date - html date control
   - datetime - html datetime control
   - email - html inpyt type email
   - url - html input type url
   - password - html input type password, use for content needs to be hidden
   - blob - text area, limit with max length
   - array - tbd
     - can array be array of fieldtype
4. extra proporties to use with fieldtype
   - string - min, max length, default to 255
   - interger, float - min, max value
   - blob - max length, default to 1024
5. rownumber - required
   - use to build UI to have labels in order for row number
7. columnnumber - required
   - use to buld UI to have labels in order of columns in same row
   - how to limit max columns *TBD*

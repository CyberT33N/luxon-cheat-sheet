# Luxon Cheat Sheet
Luxon Cheat Sheet with the most needed stuff..



## Datetime instance


<br><br>

### Create Datetime instance from JS date
```javascript
const date = new Date();
const datetime = DateTime.fromJSDate(date); 
```

### Create Datetime instance from ISO String
```javascript
const startDate = DateTime.fromISO('2017-04-01')
```


<br><br>
________________________________________________________________
________________________________________________________________

<br><br>








<br><br>

## Add days

```javascript
const luxon = require('luxon')
const { DateTime } = luxon

DateTime.fromJSDate(dtstart).plus({days: maxDays}).toJSDate()
```




<br><br>

## Compare dates
- https://moment.github.io/luxon/#/math?id=comparing-datetimes

```javascript
var DateTime = luxon.DateTime;

var d1 = DateTime.fromISO('2017-04-30');
var d2 = DateTime.fromISO('2017-04-01');

console.log(d2 < d1); //=> true
console.log(d2 > d1); //=> false
```

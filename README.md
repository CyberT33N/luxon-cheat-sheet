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













<br><br>
________________________________________________________________
________________________________________________________________

<br><br>



## Calculate a duration between two dates
```javascript
const date1 = luxon.DateTime.fromISO("2020-09-06T12:00")
const date2 = luxon.DateTime.fromISO("2019-06-10T14:00")

## Method #1
const diff = Interval.fromDateTimes(date2, date1)
const diffDays = diff.length('days')

// Method #2
const diff = date1.diff(date2, ["years", "months", "days", "hours"])
console.log(diff.toObject())
```


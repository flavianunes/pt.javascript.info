importance: 4

---

# Format the relative date

Write a function `formatDate(date)` that should format `date` as follows:

- If since `date` passed less than 1 second, then `"right now"`.
- Otherwise, if since `date` passed less than 1 minute, then `"n sec. ago"`.
- Otherwise, if less than an hour, then `"m min. ago"`.
- Otherwise, the full date in the format `"DD.MM.YY HH:mm"`. That is: `"day.month.year hours:minutes"`, all in 2-digit format, e.g. `31.12.16 10:00`.

For instance:

```js
alert( formatDate(new Date(new Date - 1)) ); // "right now"

alert( formatDate(new Date(new Date - 30 * 1000)) ); // "30 sec. ago"

alert( formatDate(new Date(new Date - 5 * 60 * 1000)) ); // "5 min. ago"

<<<<<<< HEAD
// yesterday's date like 31.12.2016, 20:00
=======
// yesterday's date like 31.12.16 20:00
>>>>>>> e074a5f825a3d10b0c1e5e82561162f75516d7e3
alert( formatDate(new Date(new Date - 86400 * 1000)) );
```

# Store as UTC but display locally
```javascript
const moment = require('moment')

let date = new Date()
console.log(date)

let m = moment(date).format('YYYY-MM-DD HH:mm:ss')
console.log(m)

let mUITC = moment.utc(date).format('YYYY-MM-DD HH:mm:ss')
console.log(mUITC)

let mUTC = moment.utc(date)
let mLoc = moment(mUTC).local().format('YYYY-MM-DD HH:mm:ss')
console.log(mLoc)
```

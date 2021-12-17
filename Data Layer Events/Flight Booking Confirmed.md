# Flight Booking Confirmed

### 

## Javascript Code
```js
window.appEventDataORM = window.appEventDataORM || [];;;
appEventDataORM.push({
  "event": "Flight Booking Confirmed",
    "airTravel": {
        "bookingLeadTime": "<bookingLeadTime>",
        "flightList": [
            {
                "tripId": "<tripId>"
            }
        ]
    }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|bookingLeadTime|string|Number of days ahead of departure for the first segment of a trip.|zero, 1, 20, 22, 33|^([0-9])|(zero)$||||||
|tripId|string|A unique representation of the main departure and arrival points for all primary trip legs \(not including connections\). |SFO&gt;YYC:YYC&gt;SFO, SFO&gt;YYC, SFO&gt;YYC:YYC&gt;YXC:YKA&gt;SFO|^([A-Z]{3}>[A-Z]{3}:?)+$||||||





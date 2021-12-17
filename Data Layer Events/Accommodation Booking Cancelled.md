# Accommodation Booking Cancelled

### 

## Javascript Code
```js
window.appEventDataORM = window.appEventDataORM || [];;;
appEventDataORM.push({
  "event": "Accommodation Booking Cancelled",
    "booking": {
        "cancellationID": "<cancellationID>",
        "roomList": [
            {
                "location": {
                    "locationId": "<locationId>"
                },
                "room": {
                    "numAdults": <numAdults>,
                    "numberInMultiRoomReservation": <numberInMultiRoomReservation>,
                    "stayDate": "<stayDate>"
                }
            }
        ],
        "transactionID": "<transactionID>"
    }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|cancellationID|string|Unique identifier of a cancellation of a booking.  Typically not the same as the booking ID.|CN-34456789|||||||
|locationId|string|Unique Identifier of a Location. |155, 65588, 987764448|||||||
|numAdults|integer|Integer number of adults for the booking.|1, 2, 3, 4, 5||||1|||
|numberInMultiRoomReservation|integer|Integer position of a room in a multi-room booking action.|1, 2, 3||||1|||
|stayDate|string|Date of each room night. ISO 8601 form \(YYYY-MM-DD\). Jan 1, 2019 is 2019-01-01|2001-12-22, 2011-01-01|^([0-9]{4})-(1[0-2]|0[1-9])-(3[01]|0[1-9]|[12][0-9])$||||||
|transactionID|string|Unique identifier of the transaction. Max Length 20. Used as a key for upload of post transaction data. ||^[a-zA-Z0-9]{6,20}$|6|20||||

## Attached Notes

<p>Edited&nbsp;</p>
<p>Edited Some more&nbsp;</p>

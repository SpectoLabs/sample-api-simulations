# [Twilio API](https://www.twilio.com/docs/api/rest)

## Send SMS to invalid number
```
curl -X POST 'https://api.twilio.com/2010-04-01/Accounts/AC3d0e9aaf91e037d5f0038248b1234b55/Messages.json' \
--data-urlencode 'To=+15558675309'  \
--data-urlencode 'From=+15017250604'  \
--data-urlencode 'Body=This is the ship that made the Kessel Run in fourteen parsecs?'  \
-d 'MediaUrl=https://c1.staticflickr.com/3/2899/14341091933_1e92e62d12_b.jpg' \
--proxy localhost:8500
```

## Send SMS
```
curl -X POST 'https://api.twilio.com/2010-04-01/Accounts/AC3d0e9aaf91e037d5f0038248b1234b55/Messages.json' \
--data-urlencode 'To=+441122334455'  \
--data-urlencode 'From=+441926803004'  \
--data-urlencode 'Body=This is the ship that made the Kessel Run in fourteen parsecs?'  \
--proxy localhost:8500
```

## Make call to unverified number
```
curl -X POST https://api.twilio.com/2010-04-01/Accounts/AC3d0e9aaf91e037d5f0038248b1234b55/Calls.json     \
--data-urlencode "Url=http://demo.twilio.com/docs/voice.xml"     \
--data-urlencode "To=+1234567890"     \
--data-urlencode "From=+441926803004"    \
--proxy localhost:8500
```

## Make call
```
curl -X POST https://api.twilio.com/2010-04-01/Accounts/AC3d0e9aaf91e037d5f0038248b1234b55/Calls.json     \
--data-urlencode "Url=http://demo.twilio.com/docs/voice.xml"     \
--data-urlencode "To=+441122334455"     \
--data-urlencode "From=+441926803004"  \
--proxy localhost:8500
```

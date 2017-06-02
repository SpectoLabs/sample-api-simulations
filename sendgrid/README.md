
SendGrid (https://sendgrid.com/docs/API_Reference/api_v3.html)

Send email

```
curl --request POST   --url https://api.sendgrid.com/v3/mail/send    --header 'Content-Type: application/json'   --header 'Authorization: Bearer my-key' --data '{"personalizations": [{"to": [{"email": "test@example.com"}]}],"from": {"email": "test@example.com"},"subject": "Sending with SendGrid is Fun","content": [{"type": "text/plain", "value": "and easy to do anywhere, even with cURL"}]}' --proxy localhost:8500
```

Send email with bad request
```
curl --request POST   --url https://api.sendgrid.com/v3/mail/send  --header 'Content-Type: application/json'   --header 'Authorization: Bearer my-key' --data '{"personalizations": [{"to": []}],"from": {"email": "test@example.com"},"subject": "Sending with SendGrid is Fun","content": [{"type": "text/plain", "value": "and easy to do anywhere, even with cURL"}]}' --proxy localhost:8500
```

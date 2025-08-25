# RFC 8693 Token Exchange (نمونه cURL)

```bash
curl -X POST https://idp.example.com/oauth2/token \
  -H "Authorization: Basic BASE64(client_id:client_secret)" \
  -d "grant_type=urn:ietf:params:oauth:grant-type:token-exchange" \
  -d "subject_token=eyJhbGciOi..." \
  -d "subject_token_type=urn:ietf:params:oauth:token-type:access_token" \
  -d "requested_token_type=urn:ietf:params:oauth:token-type:access_token" \
  -d "scope=accounts.read payments.create"
```

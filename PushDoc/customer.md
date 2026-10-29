```bash
curl -X POST "https://accoy.jpin.co.in/receive/customer/" \
  -H "Content-Type: application/json" \
  -H "X-API-Key: " \
  -d '{
    "id": 105,
    "customer_code": 204,
    "name": "Freddy DK",
    "phone": "9037002892",
    "place": "Calicut",
    "address": "Opp. Textile Market, Stadium Road"
  }'
```

Response:
```json
{
  "status": "success",
  "action": "updated",
  "message": "Customer 'Freddy DK' updated successfully.",
  "customer": {
    "id": 105,
    "customer_code": 204,
    "name": "Freddy DK",
    "contact": "9037002892",
    "place": "Calicut",
    "address": "Opp. Textile Market, Stadium Road"
  }
}
```

---

```bash
curl -X POST "https://accoy.jpin.co.in/receive/customer/" \
  -H "Content-Type: application/json" \
  -H "X-API-Key: " \
  -d '{
    "id": 106,
    "customer_code": 206,
    "name": "Akash Satheesh",
    "phone": "9037002892",
    "email": "akash@jpin.co.in",
    "place": "Ernakulam",
    "address": "Ring Road Market, Pune ,MH"
  }'
```

Response:
```json
{
  "status": "success",
  "action": "created",
  "message": "Customer 'Akash Satheesh' created successfully.",
  "customer": {
    "id": 106,
    "customer_code": 206,
    "name": "Akash Satheesh",
    "contact": "9037002892",
    "email": "akash@jpin.co.in",
    "place": "Ernakulam",
    "address": "Ring Road Market, Pune ,MH"
  }
}
```

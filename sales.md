```bash
curl -X POST "https://accoy.jpin.co.in/receive/sales/" \
  -H "Content-Type: application/json" \
  -H "X-API-Key: " \
  -d '{
    "id": 26,
    "username": "rajesh_sales",
    "name": "Rajesh Kumar",
    "email": "rajesh@example.com",
    "phone": "9823456789",
    "is_active": true
  }'
```

Response:
```json
{
  "status": "success",
  "action": "updated",
  "message": "Salesperson 'Rajesh Kumar' updated successfully.",
  "sales_person": {
    "id": 26,
    "username": "rajesh_sales",
    "name": "Rajesh Kumar",
    "email": "rajesh@example.com",
    "role": "sales_person",
    "is_active": true
  }
}
```

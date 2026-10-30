```bash
curl -X POST "https://accoy.jpin.co.in/receive/products/" \
  -H "Content-Type: application/json" \
  -H "X-API-Key: " \
  -d '{
    "category": "Casual Shirts",
    "brand": "Accoy",
    "sortnumber": "CM2701",
    "size": "38",
    "pattern": "Checked",
    "sleeve": "H/S",
    "costprice": "450.00",
    "mrp": "999.00"
  }'
```

Response:
```json
{
  "status": "success",
  "action": "created",
  "message": "Product 'CM2701-38-H/S' created successfully.",
  "product": {
    "id": 400710,
    "barcode": "CM2701-38-H/S",
    "category": "Casual Shirts",
    "brand": "Accoy",
    "sort_number": "CM2701",
    "size": "38",
    "sleeve": "H/S",
    "pattern": "Checked",
    "type": "",
    "cost_price": "450.00",
    "mrp": "999.00",
    "created_at": "2026-10-30T13:07:00.540736+00:00",
    "updated_at": "2026-10-30T13:07:00.540752+00:00"
  }
}
```

---

```bash
curl -X POST "https://accoy.jpin.co.in/receive/products/" \
  -H "Content-Type: application/json" \
  -H "X-API-Key: " \
  -d '{
    "category": "Casual Shirts",
    "brand": "Accoy",
    "sortnumber": "CM2701",
    "size": "40, 42",
    "pattern": "Checked",
    "sleeve": "H/S",
    "costprice": "450.00",
    "mrp": "999.00"
  }'
```

Response:
```json
{
  "status": "success",
  "action": "processed",
  "message": "Processed 2 product variant(s) (2 created, 0 updated).",
  "summary": {
    "total_processed": 2,
    "created": 2,
    "updated": 0,
    "errors": 0
  },
  "products": [
    {
      "id": 400711,
      "barcode": "CM2701-40-H/S",
      "category": "Casual Shirts",
      "brand": "Accoy",
      "sort_number": "CM2701",
      "size": "40",
      "sleeve": "H/S",
      "pattern": "Checked",
      "type": "",
      "cost_price": "450.00",
      "mrp": "999.00",
      "created_at": "2026-10-30T13:07:15.547982+00:00",
      "updated_at": "2026-10-30T13:07:15.547996+00:00"
    },
    {
      "id": 400712,
      "barcode": "CM2701-42-H/S",
      "category": "Casual Shirts",
      "brand": "Accoy",
      "sort_number": "CM2701",
      "size": "42",
      "sleeve": "H/S",
      "pattern": "Checked",
      "type": "",
      "cost_price": "450.00",
      "mrp": "999.00",
      "created_at": "2026-10-30T13:07:15.589904+00:00",
      "updated_at": "2026-10-30T13:07:15.589951+00:00"
    }
  ]
}
```

---

```bash
curl -X POST "https://accoy.jpin.co.in/receive/products/" \
  -H "Content-Type: application/json" \
  -H "X-API-Key: " \
  -d '{
    "category": "Slim Trousers",
    "brand": "Accoy",
    "sortnumber": "TR5001",
    "size": "32",
    "pattern": "Solid",
    "sleeve": "none",
    "costprice": "600.00",
    "mrp": "1499.00"
  }'
```

Response:
```json
{
  "status": "success",
  "action": "created",
  "message": "Product 'TR5001-32' created successfully.",
  "product": {
    "id": 400713,
    "barcode": "TR5001-32",
    "category": "Slim Trousers",
    "brand": "Accoy",
    "sort_number": "TR5001",
    "size": "32",
    "sleeve": "none",
    "pattern": "Solid",
    "type": "",
    "cost_price": "600.00",
    "mrp": "1499.00",
    "created_at": "2026-10-30T13:07:24.694178+00:00",
    "updated_at": "2026-10-30T13:07:24.694184+00:00"
  }
}
```

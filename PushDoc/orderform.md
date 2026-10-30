```bash
curl -X POST "https://accoy.jpin.co.in/receive/order-form/" \
  -H "Content-Type: application/json" \
  -H "X-API-Key: " \
  -d '{
    "external_order_number": "20261029311",
    "customer": 105,
    "sales_person": 26,
    "remarks": "Urgent delivery by Friday",
    "lines": [
      {
        "sort_number": "1301",
        "size": "38",
        "sleeve": "FS",
        "color": "White",
        "mrp": 799.00,
        "quantity": 10
      },
      {
        "sort_number": "1301",
        "size": "40",
        "sleeve": "FS",
        "color": "White",
        "mrp": 799.00,
        "quantity": 15
      },
      {
        "barcode": "1301-42-FS-WHT",
        "quantity": 5
      }
    ]
  }'
```

Response:
```json
{
  "status": "success",
  "message": "Order form 20261029311 created successfully.",
  "order_form": {
    "id": 75069,
    "order_number": "20261029311",
    "external_order_number": "20261029311",
    "status": "planned",
    "dealer_name": "Freddy DK",
    "dealer_place": "Calicut",
    "dealer_contact": "9037002892",
    "remarks": "Urgent delivery by Friday",
    "customer": {
      "id": 105,
      "customer_code": 204,
      "name": "Freddy DK",
      "contact": "9037002892",
      "email": "",
      "place": "Calicut",
      "address": "Opp. Textile Market, Stadium Road"
    },
    "sales_person": {
      "id": 26,
      "username": "rajesh_sales",
      "name": "Rajesh Kumar",
      "email": "rajesh@example.com"
    },
    "total_lines": 3,
    "total_requested_quantity": 30,
    "matched_lines": 0,
    "unmatched_lines": 3,
    "created_at": "2026-10-29T18:10:26.553769+00:00",
    "lines": [
      {
        "id": 150434,
        "source_row": 1,
        "sort_number": "1301",
        "size": "38",
        "sleeve": "FS",
        "color": "White",
        "mrp": "799.0",
        "requested_quantity": 10,
        "match_status": "not_found",
        "variant": null
      },
      {
        "id": 150435,
        "source_row": 2,
        "sort_number": "1301",
        "size": "40",
        "sleeve": "FS",
        "color": "White",
        "mrp": "799.0",
        "requested_quantity": 15,
        "match_status": "not_found",
        "variant": null
      },
      {
        "id": 150436,
        "source_row": 3,
        "sort_number": "",
        "size": "",
        "sleeve": "",
        "color": "",
        "mrp": null,
        "requested_quantity": 5,
        "match_status": "not_found",
        "variant": null
      }
    ],
    "auto_allocated": false
  }
}
```

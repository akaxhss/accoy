# Architecture

Listening endpoints hosted under `https://accoy.jpin.co.in/receive/`

| Endpoint | Method | Primary Action | Payload Type |
|---|---|---|---|
| `https://accoy.jpin.co.in/receive/customer/` | POST / GET | Creates or updates customer/dealer records | Customer JSON (single or array) |
| `https://accoy.jpin.co.in/receive/sales/` | POST / GET | Syncs sales representative accounts | Salesperson JSON (single or array) |
| `https://accoy.jpin.co.in/receive/order-form/` | POST / GET | Auto-creates Order Form & Lines with catalog matching | Order Form JSON with lines array |

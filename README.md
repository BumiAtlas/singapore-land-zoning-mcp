# Singapore Land Lots & Master Plan Zoning MCP

Connect your AI assistant to [BumiAtlas](https://bumiatlas.com) for Singapore land research through the Model Context Protocol.

This listing is a focused entry point for:

- Every cadastral land lot in Singapore (~147k) from the Singapore Land Authority (SLA): lot key, district, area, perimeter and boundary
- Lot lookup as titles write it ("Lot 95333A MK26", "MK26-95333A") or by coordinates
- URA Master Plan 2025 land-use zoning at any point: land use (residential, commercial, business, white, …) and gross plot ratio (GPR)
- The zoning over a lot, with each zone's share of it
- Satellite and street map images of a lot and its neighbours, labelled by lot number

## Connect

```
https://bumiatlas.com/mcp/singapore
```

Add it as a custom connector in any MCP client and sign in with Google. Tools, examples and data notes: [bumiatlas.com/mcp-docs/singapore](https://bumiatlas.com/mcp-docs/singapore).

## Tools

| Tool | Description |
|---|---|
| `SG_lot_search` | Find lots by lot key (MK26-95333A), "Lot 95333A MK26", lot number with district or check letter, or `latitude, longitude` |
| `SG_lot_get` | One lot: district, area, perimeter, last update and the Master Plan zones covering it with their GPR; boundary as GeoJSON |
| `SG_lot_image` | Satellite or street map image of a lot or point, with every lot in view outlined and labelled with its lot number |
| `SG_land_use_get` | Master Plan 2025 zone at a point or by id: land use, GPR or GPR code (landed housing, subject to evaluation), white-use and business-GPR limits |

## Example prompts

- *"What is Lot 95333A MK26? How big is it and what is it zoned for?"*
- *"Which lot is at 1.2834, 103.8607, and what is its gross plot ratio?"*
- *"Is this address in a landed housing area?"*
- *"What does the Master Plan allow on the lots around this point?"*

## Data sources

Contains information from Cadastral Land Parcel (Singapore Land Authority) and Master Plan 2025 Land Use Layer (Urban Redevelopment Authority) accessed on 25 October 2026 from data.gov.sg, which is made available under the terms of the [Singapore Open Data Licence version 1.0](https://data.gov.sg/open-data-licence). Lots have no owner, title or tenure information.

# Mississauga Zoning Lookup Automation

A Make.com (Integromat) automation system that provides instant address validation, geocoding, and zoning resource access for Mississauga, Ontario properties.

## 🎯 Project Overview

This automation was built to streamline property research by providing real-time address-to-coordinates conversion and integration with official City of Mississauga zoning resources.

## ✨ Features

- **Address Validation**: Validates and formats Mississauga property addresses
- **Geocoding**: Converts addresses to precise latitude/longitude coordinates
- **JSON API**: RESTful webhook endpoint with structured responses
- **Official Resources**: Direct links to City of Mississauga zoning tools
- **24/7 Availability**: Reliable Make.com cloud infrastructure
- **Easy Integration**: Simple HTTP GET/POST requests

## 🛠️ Tech Stack

- **Platform**: Make.com (formerly Integromat)
- **APIs**: Google Maps Geocoding API
- **Format**: RESTful JSON API
- **Architecture**: Webhook-based automation

## 📋 How It Works

1. Client sends address via webhook (GET or POST request)
2. Google Maps API geocodes the address
3. System validates location is in Mississauga
4. Returns JSON with coordinates and official zoning resources

## 🔧 API Usage

### Request
```bash
GET https://hook.eu2.make.com/YOUR_WEBHOOK_ID?address=300%20City%20Centre%20Drive,%20Mississauga,%20ON
```

### Response
```json
{
  "status": "success",
  "address": "300 City Centre Dr, Mississauga, ON L5B 3C1, Canada",
  "coordinates": {
    "latitude": 43.5852972,
    "longitude": -79.6446838
  },
  "city": "Mississauga",
  "province": "Ontario",
  "zoning": {
    "message": "Zoning data requires Mississauga GIS API access...",
    "interactive_map": "http://www6.mississauga.ca/missmaps/maps.aspx",
    "note": "Full automated zoning lookup requires official API credentials"
  },
  "timestamp": "2024-11-06T15:30:00Z"
}
```

## 📚 Documentation

Complete technical documentation included:
- Setup instructions
- API endpoint details
- Response format specifications
- Testing guidelines
- Technical limitations
- Future enhancement options

## 🚧 Technical Challenges

### Constraints Addressed:
- **Make.com File Size Limit**: 10MB maximum (Mississauga zoning data is 30MB)
- **No Public API**: City of Mississauga doesn't provide live API access
- **Geospatial Processing**: Point-in-polygon calculations require external infrastructure

### Solution Approach:
Created a practical Phase 1 solution focusing on address validation and geocoding, with clear documentation on infrastructure requirements for full automated zoning lookup.

## 🔮 Future Enhancements

Potential upgrades with additional infrastructure:
- Integration with external geospatial services (Mapbox, PostGIS)
- Cloud-hosted zoning data with custom lookup functions
- Point-in-polygon calculations for automated zone detection
- AWS Lambda/S3 integration for file processing

## 📄 Files Included

- `blueprint.json` - Make.com scenario (importable)
- `documentation.md` - Complete technical documentation
- `README.md` - This file

## 🎓 Skills Demonstrated

- API Integration & Development
- Automation Design (Make.com/Integromat)
- RESTful API Architecture
- JSON Data Formatting
- Problem Solving & Research
- Technical Documentation
- Municipal/Government Data Systems
- Client Communication

## 📞 Official Resources

- [City of Mississauga Zoning Information](https://www.mississauga.ca/services-and-programs/building-and-renovating/zoning-information/)
- [Mississauga Interactive Zoning Map](http://www6.mississauga.ca/missmaps/maps.aspx)
- [Mississauga Open Data Portal](https://data.mississauga.ca/)

## 📝 License

This project was created for a client and is shared for portfolio purposes.

- Fiverr:(https://www.fiverr.com/s/Gz4bBba)
- LinkedIn: www.linkedin.com/in/ademola-gbadamosi-demmy15

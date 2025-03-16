# Razzaq.net
Razzaq provides a suite of APIs to support property listing, search, and marketing for rental properties. It serves users, real estate agents, landlords, and developers. The platform supports advanced search, user authentication, listing management, and analytics.
# Authentication

- API Key: Required for access to any endpoint.
- Endpoint: /api/auth/login
- Method: POST
- Parameters:
   1. username: string
   2. password: string
   
# Endpoints
### 1.	Get Property Listings
- Endpoint: /api/listings
- Method: GET
- Parameters:
  1. location: string (optional)
  2. price_min: integer (optional)
  3. price_max: integer (optional)
  4. property_type: string (optional)
  5. page: integer (optional)
     
### 2.	Add New Property Listing
- Endpoint: /api/listings
- Method: POST
- Parameters:
   1. title: string (required)
   2. description: string (required)
   3. price: integer (required)
   4. address: string (required)
   5. images[]: array of strings (required)
   6. property_type: string (required)
   7. contact_details: object (required)

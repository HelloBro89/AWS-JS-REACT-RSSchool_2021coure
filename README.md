# Online Store

## This repository contains only a frontend part for an online store built on AWS. This app is in the process of being finalized, so some features have not yet been implemented.

# ATTENTION

## If you are trying to add several products to the store at once using the "Choose File" button, you need to create a file with the "CSV" extension. For example

| count | price | title |   description   |
|-------|-------|-------|-----------------|
| 34    | 30    | jeans | jeans blue short|
| 15    | 20000 | car   | Ford sports car |

**!!! Сount, price, title and description fields must be filled in as in the example !!!**

## Also you can add, get by ID or get all a product using post request:
1. Add product (POST)
To url: https://b6sld3tghb.execute-api.eu-west-1.amazonaws.com/dev/products
#### and body:

```javascript
    {
    "price": 1000,
    "title": "TITILE",
    "description": "DESCRIPTION",
    "count": 9999999
    }
```
2. Get ALL (GET)
To url: https://b6sld3tghb.execute-api.eu-west-1.amazonaws.com/dev/products

3. Get by ID (GET)
To url: `https://b6sld3tghb.execute-api.eu-west-1.amazonaws.com/dev/products/{productID}`

### All actual requests for the backend part are located in the file along the relative path:
```bash
cd src\constants\apiPaths.ts
```

## Additional links:
- link to bakend https://github.com/HelloBro89/shop-AWS-js-Backend
- link to cart-api-service https://github.com/HelloBro89/cart-api-backend-shop

## User guide

1. **npm install**
2. **npm run start** 
3. **npm run build** 
4. **npm run build:deploy** - build and deploy in S3 bucket
5. **npm run cloudfront:update:build:deploy** - build, deploy, creat cloudfront and invalidation (with confirm)

## The front-end part of the application used:
- React
- TypeScript
- Redux
- material-ui


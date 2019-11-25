# Market
RestAPI using JpaRepository, which enables to create, read, update and delete products.

To get all Products 

```
http://localhost:8080/products
```

```json
{
  "_embedded": {
    "products": [
      {
        "pname": "Rice",
        "pprice": 2,
        "_links": {
          "self": {
            "href": "http://localhost:8080/products/1"
          },
          "product": {
            "href": "http://localhost:8080/products/1"
          }
        }
      }
    ]
  },
  "_links": {
    "self": {
      "href": "http://localhost:8080/products{?page,size,sort}",
      "templated": true
    },
    "profile": {
      "href": "http://localhost:8080/profile/products"
    }
  },
  "page": {
    "size": 20,
    "totalElements": 1,
    "totalPages": 1,
    "number": 0
  }
}
```


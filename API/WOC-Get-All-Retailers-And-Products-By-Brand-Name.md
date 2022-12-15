Get all Retailers and the products from the retailers from 1 brand
  
* **URL**

  /getallretailersandproductsbybrandname

* **Method:**
 
  `GET`

* **Data Params**

  `{ brand : "Bullit" }`

* **Success Response:**

  * **Code:** 200 <br />
    **Content:** `
    [
  {
    "brand": "Bullit",
    "retailer": "Albert Heijn",
    "products": [
      {
        "name": "Bullit Energy drink",
        "score": 20
      },
      {
        "name": "Bullit Energy drink 6-pack",
        "score": 0
      },
      {
        "name": "Bullit Energy drink 24-pack",
        "score": 0
      },
      {
        "name": "Bullit Energy drink suikervrij",
        "score": 20
      },
      {
        "name": "Bullit Energy drink suikervrij 6-pack",
        "score": 0
      },
      {
        "name": "Bullit Energy drink suikervrij 24-pack",
        "score": 0
      },
      {
        "name": "Bullit Energy drink suikervrij rode bessen",
        "score": 20
      },
      {
        "name": "Bullit Energy drink suikervrij citrus",
        "score": 20
      },
      {
        "name": "Bullit Energy drink suikervrij mango",
        "score": 0
      },
      {
        "name": "Bullit Energy drink suikervrij passievrucht",
        "score": 0
      }
    ]
  },
  {
    "brand": "Bullit",
    "retailer": "Jumbo",
    "products": [
      {
        "name": "Bullit Energy Drink -250ml",
        "score": 0
      },
      {
        "name": "Bullit Energy Drink 6-pack - 6x250ml",
        "score": 0
      },
      {
        "name": "Bullit Energy Drink 24-pack - 24x250ml",
        "score": 0
      },
      {
        "name": "Bullit Energy Drink suikervrij - 250ml",
        "score": 0
      },
      {
        "name": "Bullit Energy Drink suikervrij 6-pack - 6x250ml",
        "score": 0
      },
      {
        "name": "Bullit Energy Drink suikervrij 24-pack - 24x250ml",
        "score": 0
      },
      {
        "name": "Bullit Energy Drink suikervrij rode bessen - 250ml",
        "score": 0
      },
      {
        "name": "Bullit Energy Drink suikervrij citrus - 250ml",
        "score": 0
      },
      {
        "name": "Bullit Energy Drink suikervrij mango - 250ml",
        "score": 0
      },
      {
        "name": "Bullit Energy Drink suikervrij passievrucht - 250ml",
        "score": 0
      }
    ]
  }
]
    `
 
* **Error Response:**

  * **Code:** 403 Forbidden <br />
    **Content:** `{ "message" : "Forbidden" }`
    
  * **Code:** 400 Bad Request <br />
    **Content:** `{ "message" : "brand is not defined!" }`
    

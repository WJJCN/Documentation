**Voorbeeld**
----

/Hier zet je de bescrijving neer
  
* **URL**

  /get_retailers_by_brand

* **Method:**
 
  `GET`

* **Data Params**

  `{ brand : "Red Bull" }`

* **Success Response:**

  * **Code:** 200 <br />
    **Content:** `
    [
      {
        "_id": {
            "$oid": "6347dd4f9af4f90f103778e5"
        },
        "brand": "Red Bull",
        "retailers": "Jumbo",
        "products": [
            {
                "name": "Red Bull Energy Drink - 250ml",
                "score": "100%"
            },
            {
                "name": "Red Bull Energy Drink 4-pack - 4x250ml",
                "score": "100%"
            },
            {
                "name": "Red Bull Energy Drink 6-pack - 6x250ml",
                "score": "100%"
            },
            {
                "name": "Red Bull Energy Drink 24-pack - 24x250ml",
                "score": "100%"
            },
            {
                "name": "Red Bull Energy Drink 12-pack - 12x250ml",
                "score": "100%"
            }
          ]
        }
      }
    ]
    `
 
* **Error Response:**

  * **Code:** 403 Forbidden <br />
    **Content:** `{ "message" : "Forbidden" }`
    
  * **Code:** 400 Bad Request <br />
    **Content:** `{ "message" : "brand is not defined!" }`
    

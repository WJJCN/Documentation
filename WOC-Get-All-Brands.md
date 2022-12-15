Get all Brands
  
* **URL**

  /brand

* **Method:**
 
  `GET`

* **Success Response:**

  * **Code:** 200 <br />
    **Content:** `
[
  {
    "_id": {
      "$oid": "63762d38f2c01e731408394d"
    },
    "name": "Red Bull",
    "retailers": [
      {
        "$oid": "637629daf2c01e7314083933"
      },
      {
        "$oid": "63762a7bf2c01e7314083935"
      }
    ]
  },
  {
    "_id": {
      "$oid": "63762d52f2c01e731408394f"
    },
    "name": "Bullit",
    "retailers": [
      {
        "$oid": "637629daf2c01e7314083933"
      },
      {
        "$oid": "63762a7bf2c01e7314083935"
      }
    ]
  }
]
    `
 
* **Error Response:**

  * **Code:** 403 Forbidden <br />
    **Content:** `{ "message" : "Forbidden" }`

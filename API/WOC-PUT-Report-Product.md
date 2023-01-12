Update product to be reported
  
* **URL**

  /reportproduct

* **Method:**
 
  `PUT`

* **Data Params**

`{ product : {
    "_id": {
      "$oid": "6389c6fdee8041d6f23282eb"
    }
  } }`


* **Success Response:**

  * **Code:** 200 <br />
    **Content:** `
{
  "statuscode": 200,
  "body": "\"Product reported!\""
}
    `
 
* **Error Response:**
  * **Code:** 400 Bad Request <br />
    **Content:** `{ "message" : "product is not defined!" }`
    
  * **Code:** 403 Forbidden <br />
    **Content:** `{ "message" : "Forbidden" }`

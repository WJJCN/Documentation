Update brands
  
* **URL**

  /brand

* **Method:**
 
  `PUT`

* **Data Params**

  `{ token : "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjEiLCJkYXRlIjoiMDEtMTItMjAyMyIsImhhc2hlZF9wYXNzd29yZCI6ImViMzE3MjY3NGI3ZWFkNDc2NGM4ZDVhODExODc0YWQ1OTRjY2U2OWMxYzc2MzIzYmZiYTE3OWY5ZGM4MGZlYzcifQ.-WZ-0nIyWOY8F2KuLTEAmrfGw5vG3xNL3YA59Z2WmXQ" }`
  `{ brands : {
    "_id": {
      "$oid": "6388a8ff2f39bd02dcb65bf5"
    },
    "name": "Testbrand",
    "retailers": [
      "637629daf2c01e7314083933",
      "63762a7bf2c01e7314083935"
    ]
  } }`


* **Success Response:**

  * **Code:** 200 <br />
    **Content:** `
{
  "statuscode": 200,
  "body": "\"All values changend!\""
}
    `
 
* **Error Response:**
  * **Code:** 400 Bad Request <br />
    **Content:** `{ "message" : "token is not defined!" }`
    
  * **Code:** 400 Bad Request <br />
    **Content:** `{ "message" : "brands is not defined!" }`
    
  * **Code:** 401 Unauthorized <br />
    **Content:** `{ "message" : "Token incorrect!" }`
    
  * **Code:** 403 Forbidden <br />
    **Content:** `{ "message" : "Forbidden" }`

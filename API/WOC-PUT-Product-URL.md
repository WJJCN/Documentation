Update product url
  
* **URL**

  /reportedproduct

* **Method:**
 
  `PUT`

* **Data Params**

  `{ token : "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjEiLCJkYXRlIjoiMDEtMTItMjAyMyIsImhhc2hlZF9wYXNzd29yZCI6ImViMzE3MjY3NGI3ZWFkNDc2NGM4ZDVhODExODc0YWQ1OTRjY2U2OWMxYzc2MzIzYmZiYTE3OWY5ZGM4MGZlYzcifQ.-WZ-0nIyWOY8F2KuLTEAmrfGw5vG3xNL3YA59Z2WmXQ" }`
  `{ product : {
    "_id": {
      "$oid": "639af2d8832a17b024fdcc15"
    },
    "product_url": "test.nl"
  } }`


* **Success Response:**

  * **Code:** 200 <br />
    **Content:** `
{
  "statuscode": 200,
  "body": "\"Password changed!\""
}
    `
 
* **Error Response:**
  * **Code:** 400 Bad Request <br />
    **Content:** `{ "message" : "token is not defined!" }`
    
  * **Code:** 400 Bad Request <br />
    **Content:** `{ "message" : "product is not defined!" }`
    
  * **Code:** 401 Unauthorized <br />
    **Content:** `{ "message" : "Token incorrect!" }`
    
  * **Code:** 403 Forbidden <br />
    **Content:** `{ "message" : "Forbidden" }`

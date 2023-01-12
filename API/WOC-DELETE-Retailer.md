Delete a retailer
  
* **URL**

  /retailer

* **Method:**
 
  `DELETE`

* **Data Params**

  `{ token : "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjEiLCJkYXRlIjoiMDEtMTItMjAyMyIsImhhc2hlZF9wYXNzd29yZCI6ImViMzE3MjY3NGI3ZWFkNDc2NGM4ZDVhODExODc0YWQ1OTRjY2U2OWMxYzc2MzIzYmZiYTE3OWY5ZGM4MGZlYzcifQ.-WZ-0nIyWOY8F2KuLTEAmrfGw5vG3xNL3YA59Z2WmXQ" }`
  `{ id : "63bfc4c2e39fcd01114b9f8a" }`

* **Success Response:**

  * **Code:** 200 <br />
    **Content:** `
{
  "statuscode": 200,
  "body": "\"Retailer deleted!\""
}
    `
 
* **Error Response:**
  * **Code:** 400 Bad Request <br />
    **Content:** `{ "message" : "token is not defined!" }`
    
  * **Code:** 400 Bad Request <br />
    **Content:** `{ "message" : "id is not defined!" }`
    
  * **Code:** 401 Unauthorized <br />
    **Content:** `{ "message" : "Token incorrect!" }`
    
  * **Code:** 403 Forbidden <br />
    **Content:** `{ "message" : "Forbidden" }`

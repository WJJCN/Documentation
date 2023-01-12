Add a brand
  
* **URL**

  /brand

* **Method:**
 
  `POST`

* **Data Params**

  `{ token : "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjEiLCJkYXRlIjoiMDEtMTItMjAyMyIsImhhc2hlZF9wYXNzd29yZCI6ImViMzE3MjY3NGI3ZWFkNDc2NGM4ZDVhODExODc0YWQ1OTRjY2U2OWMxYzc2MzIzYmZiYTE3OWY5ZGM4MGZlYzcifQ.-WZ-0nIyWOY8F2KuLTEAmrfGw5vG3xNL3YA59Z2WmXQ" }`
  `{ name : "Jumbo" }`
  `{ retailers : "[
		"637629daf2c01e7314083933",
		"63762a7bf2c01e7314083935"
	]" }`

* **Success Response:**

  * **Code:** 200 <br />
    **Content:** `
{
  "$oid": "63bfc8c5b4955272cf451724"
}
    `
 
* **Error Response:**
  * **Code:** 400 Bad Request <br />
    **Content:** `{ "message" : "token is not defined!" }`
    
  * **Code:** 400 Bad Request <br />
    **Content:** `{ "message" : "name is not defined!" }`
    
  * **Code:** 400 Bad Request <br />
    **Content:** `{ "message" : "retailers is not defined!" }`
    
  * **Code:** 401 Unauthorized <br />
    **Content:** `{ "message" : "Token incorrect!" }`
    
  * **Code:** 403 Forbidden <br />
    **Content:** `{ "message" : "Forbidden" }`

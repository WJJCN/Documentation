Add a retailer
  
* **URL**

  /retailer

* **Method:**
 
  `POST`

* **Data Params**

  `{ token : "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjEiLCJkYXRlIjoiMDEtMTItMjAyMyIsImhhc2hlZF9wYXNzd29yZCI6ImViMzE3MjY3NGI3ZWFkNDc2NGM4ZDVhODExODc0YWQ1OTRjY2U2OWMxYzc2MzIzYmZiYTE3OWY5ZGM4MGZlYzcifQ.-WZ-0nIyWOY8F2KuLTEAmrfGw5vG3xNL3YA59Z2WmXQ" }`
  `{ name: "test" }`
  `{ base_url: "test.nl" }`
  `{ scrape: "false" }`
  `{ url_to_scrape: "test.nl/producten" }`
  

* **Success Response:**

  * **Code:** 200 <br />
    **Content:** `
{
  "$oid": "63bfc97945005a7b4279bf82"
}
    `
 
* **Error Response:**
  * **Code:** 400 Bad Request <br />
    **Content:** `{ "message" : "token is not defined!" }`
    
  * **Code:** 400 Bad Request <br />
    **Content:** `{ "message" : "name is not defined!" }`
    
  * **Code:** 400 Bad Request <br />
    **Content:** `{ "message" : "base_url is not defined!" }`
    
  * **Code:** 400 Bad Request <br />
    **Content:** `{ "message" : "scrape is not defined!" }`
    
  * **Code:** 400 Bad Request <br />
    **Content:** `{ "message" : "url_to_scrape is not defined!" }`
    
  * **Code:** 401 Unauthorized <br />
    **Content:** `{ "message" : "Token incorrect!" }`
    
  * **Code:** 403 Forbidden <br />
    **Content:** `{ "message" : "Forbidden" }`

Delete a brand
  
* **URL**

  /brand

* **Method:**
 
  `DELETE`

* **Success Response:**

  * **Code:** 200 <br />
    **Content:** `
{
  "statuscode": 200,
  "body": "\"Brand deleted!\""
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

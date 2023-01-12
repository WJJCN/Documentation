Get JWT token to login
  
* **URL**

  /login

* **Method:**
 
  `GET`
  
* **Data Params**

  `{  password: "admin" }`

* **Success Response:**

  * **Code:** 200 <br />
    **Content:** `
{
  "statuscode": 200,
  "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjEiLCJkYXRlIjoiMTItMTYtMjAyMiIsImhhc2hlZF9wYXNzd29yZCI6IjcyNDJjZDg0NWE1NTE4ZmJhMTFjMDdmYTI5NWI0NThkNTAwZjY3OGNhYjYyOGFiYzg5ZDY3ZGQ1ZGZiNjYxOWIifQ.NEsKeY0T0Eus3FS5K_AUy8OlOJb7WcGM5gU7OhJbtVE"
}
    `
 
* **Error Response:**
  * **Code:** 400 Bad Request <br />
    **Content:** `{ "message" : "password is not defined!" }`
    
  * **Code:** 401 Unauthorized <br />
    **Content:** `{ "message" : "Password is not correct!" }`
    
  * **Code:** 403 Forbidden <br />
    **Content:** `{ "message" : "Forbidden" }`

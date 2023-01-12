Get reported products for admin page
  
* **URL**

  /reportedproduct

* **Method:**
 
  `GET`
  
* **Data Params**

  `{ token : "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjEiLCJkYXRlIjoiMDEtMTItMjAyMyIsImhhc2hlZF9wYXNzd29yZCI6ImViMzE3MjY3NGI3ZWFkNDc2NGM4ZDVhODExODc0YWQ1OTRjY2U2OWMxYzc2MzIzYmZiYTE3OWY5ZGM4MGZlYzcifQ.-WZ-0nIyWOY8F2KuLTEAmrfGw5vG3xNL3YA59Z2WmXQ" }`

* **Success Response:**

  * **Code:** 200 <br />
    **Content:** `
{
    "_id": {
      "$oid": "639af2d8832a17b024fdcc1b"
    },
    "brand": {
      "$oid": "63762d52f2c01e731408394f"
    },
    "retailer": {
      "$oid": "637629daf2c01e7314083933"
    },
    "name": "Bullit Energy drink 6-pack",
    "reported": true,
    "product_url": "https://www.ah.nl/producten/product/wi229612/bullit-energy-drink-6-pack/",
    "product_brand": {
      "productomschrijving": "Energy drink 6-pack",
      "inhoud": "6 x",
      "Opco": "Bullit",
      "omschrijving": "Bullit Energy Drink geeft je de energie die je nodig hebt in vele dagelijkse situaties.",
      "USP": [
        "Ijskoud het lekkerst",
        "Bevat water, suiker, taurine, cafeïne en vitamine B",
        "De hoeveelheid suiker is vergelijkbaar met frisdrank: circa 11g/100ml",
        "De hoeveelheid cafeïne is vergelijkbaar met een kop koffie: 32mg/100ml"
      ]
    },
    "history": [
      {
        "scrape_date": "2022-12-15",
        "score": 0,
        "product_brand": {
          "productomschrijving": "Energy drink 6-pack",
          "inhoud": "6 x",
          "Opco": "Bullit",
          "omschrijving": "Bullit Energy Drink geeft je de energie die je nodig hebt in vele dagelijkse situaties.",
          "USP": [
            "Ijskoud het lekkerst",
            "Bevat water, suiker, taurine, cafeïne en vitamine B",
            "De hoeveelheid suiker is vergelijkbaar met frisdrank: circa 11g/100ml",
            "De hoeveelheid cafeïne is vergelijkbaar met een kop koffie: 32mg/100ml"
          ]
        },
        "product_scraped": {
          "productomschrijving": {
            "text": "Bullit Energy drink 6 -pack",
            "equal_to_scraped": false
          },
          "inhoud": {
            "text": "6 x 0,25 l",
            "equal_to_scraped": false
          },
          "Opco": {
            "text": "Bullit Energy drink 6 -pack",
            "equal_to_scraped": false
          },
          "omschrijving": {
            "text": "Bullit energy drink geeft je de energie die je nodig hebt in vele dagelijkse situaties.",
            "equal_to_scraped": false
          },
          "USP": {
            "text": [
              "Ijskoud het lekkerst",
              "Not found",
              "De hoeveelheid suiker is vergelijkbaar met frisdrank: circa 11g/100ml",
              "Not found"
            ],
            "equal_to_scraped": false
          }
        }
      }
    ]
  }
    `
 
* **Error Response:**
  * **Code:** 400 Bad Request <br />
    **Content:** `{ "message" : "token is not defined!" }`
    
  * **Code:** 401 Unauthorized <br />
    **Content:** `{ "message" : "Token incorrect!" }`
    
  * **Code:** 403 Forbidden <br />
    **Content:** `{ "message" : "Forbidden" }`

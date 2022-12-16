Get all products by 1 brand name
  
* **URL**

  /getallproductsbybrand

* **Method:**
 
  `GET`

* **Success Response:**

  * **Code:** 200 <br />
    **Content:** `
[
  {
    "_id": {
      "$oid": "639af2d8832a17b024fdcc1a"
    },
    "brand": "Bullit",
    "retailer": "Albert Heijn",
    "product": "Bullit Energy drink",
    "product_url": "https://www.ah.nl/producten/product/wi141083/bullit-energy-drink/",
    "history": [
      {
        "scrape_date": "2022-12-15",
        "score": 20,
        "product_brand": {
          "productomschrijving": "Energy drink",
          "inhoud": "250 ml",
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
            "text": "Bullit Energy drink",
            "equal_to_scraped": false
          },
          "inhoud": {
            "text": "250 ml",
            "equal_to_scraped": true
          },
          "Opco": {
            "text": "Bullit Energy drink",
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
      },
    ]
  }
]
    `
 
* **Error Response:**
  * **Code:** 400 Bad Request <br />
    **Content:** `{ "message" : "brand is not defined!" }`
    
  * **Code:** 403 Forbidden <br />
    **Content:** `{ "message" : "Forbidden" }`

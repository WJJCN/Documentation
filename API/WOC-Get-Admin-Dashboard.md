Get full admin dashboard with brands, products, retailers, logs, and admin settings
  
* **URL**

  /getadmindashboard

* **Method:**
 
  `GET`

* **Data Params**

  `{ token : "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjEiLCJkYXRlIjoiMDEtMTItMjAyMyIsImhhc2hlZF9wYXNzd29yZCI6ImViMzE3MjY3NGI3ZWFkNDc2NGM4ZDVhODExODc0YWQ1OTRjY2U2OWMxYzc2MzIzYmZiYTE3OWY5ZGM4MGZlYzcifQ.-WZ-0nIyWOY8F2KuLTEAmrfGw5vG3xNL3YA59Z2WmXQ" }`

* **Success Response:**

  * **Code:** 200 <br />
    **Content:** `
    {
  "allBrands": [
    {
      "_id": {
        "$oid": "63762d38f2c01e731408394d"
      },
      "name": "Red Bull",
      "retailers": [
        {
          "name": "Albert Heijn"
        },
        {
          "name": "Jumbo"
        }
      ]
    },
    {
      "_id": {
        "$oid": "63762d52f2c01e731408394f"
      },
      "name": "Bullit",
      "retailers": [
        {
          "name": "Albert Heijn"
        },
        {
          "name": "Jumbo"
        }
      ]
    }
  ],
  "allProductsArray": [
    {
      "_id": {
        "$oid": "639af2d8832a17b024fdcc15"
      },
      "brand": "Red Bull",
      "retailer": "Albert Heijn",
      "product": "Red Bull Energy drink",
      "product_url": "teeeeeeeest.nl",
      "history": [
        {
          "scrape_date": "2022-12-15",
          "score": 0,
          "product_brand": {
            "productomschrijving": "Energy drink",
            "inhoud": "250 ml",
            "Opco": "Red Bull",
            "omschrijving": "Red Bull Energy Drink wordt wereldwijd gewaardeerd door topsporters.",
            "USP": [
              "Stimuleert Lichaam en Geest®",
              "Bevat cafeïne, taurine, vitamine B, suiker en water",
              "Het suikergehalte van een blikje is gelijk aan frisdrank: 11g/100ml",
              "Het cafeïnegehalte van een blikje is gelijk aan een kop koffie: 32mg/100ml"
            ]
          },
          "product_scraped": {
            "productomschrijving": {
              "text": "Red Bull Energy drink",
              "equal_to_scraped": false
            },
            "inhoud": {
              "text": "0,25 l",
              "equal_to_scraped": false
            },
            "Opco": {
              "text": "Red Bull Energy drink",
              "equal_to_scraped": false
            },
            "omschrijving": {
              "text": "Red bull energy drink is speciaal ontwikkeld voor momenten waarop je meer wilt presteren.",
              "equal_to_scraped": false
            },
            "USP": {
              "text": [
                "Stimuleert lichaam en geest",
                "Frisdrank, sappen, koffie, thee",
                "De hoeveelheid cafeine is vergelijkaar met een kopje koffie: 32mg/100ml",
                "De hoeveelheid cafeine is vergelijkaar met een kopje koffie: 32mg/100ml"
              ],
              "equal_to_scraped": false
            }
          }
        },
      ]
    },
  "allRetailers": [   
    {
      "_id": {
        "$oid": "637629daf2c01e7314083933"
      },
      "name": "Albert Heijn",
      "base_url": "https://www.ah.nl/",
      "scrape": "false",
      "url_to_scrape": "https://www.ah.nl/producten/frisdrank-sappen-koffie-thee/frisdrank/energy-drinks"
    },
    {
      "_id": {
        "$oid": "63762a7bf2c01e7314083935"
      },
      "name": "Jumbo",
      "base_url": "https://www.jumbo.com",
      "scrape": "true",
      "url_to_scrape": "https://www.jumbo.com/producten/fris,-sap,-koffie,-thee/energiedranken"
    }
  ],
  "allLogs": [
    {
      "_id": {
        "$oid": "639af3f3c94436ba9764e399"
      },
      "date_run": "2022-12-15",
      "steps": {
        "link_crawling": {
          "status": true,
          "error": ""
        },
        "link_check": {
          "status": true,
          "error": ""
        },
        "product_fetch_compare": {
          "status": true,
          "error": ""
        },
        "save_to_database": {
          "status": true,
          "error": ""
        }
      },
      "retailer": "Albert Heijn"
    },
    {
      "_id": {
        "$oid": "639af409c94436ba9764e3b5"
      },
      "date_run": "2022-12-15",
      "steps": {
        "link_crawling": {
          "status": false,
          "error": "[ERROR] Could not crawl the given URL."
        },
        "link_check": {
          "status": true,
          "error": ""
        },
        "product_fetch_compare": {
          "status": true,
          "error": ""
        },
        "save_to_database": {
          "status": true,
          "error": ""
        }
      },
      "retailer": "Jumbo"
    },
    {
      "_id": {
        "$oid": "639c31a306d42ada98b6a084"
      },
      "date_run": "2022-12-16",
      "steps": {
        "link_crawling": {
          "status": true,
          "error": ""
        },
        "link_check": {
          "status": true,
          "error": ""
        },
        "product_fetch_compare": {
          "status": true,
          "error": ""
        },
        "save_to_database": {
          "status": true,
          "error": ""
        }
      },
      "retailer": "Albert Heijn"
    },
    {
      "_id": {
        "$oid": "639c31be06d42ada98b6a094"
      },
      "date_run": "2022-12-16",
      "steps": {
        "link_crawling": {
          "status": false,
          "error": "[ERROR] Could not crawl the given URL."
        },
        "link_check": {
          "status": true,
          "error": ""
        },
        "product_fetch_compare": {
          "status": true,
          "error": ""
        },
        "save_to_database": {
          "status": true,
          "error": ""
        }
      },
      "retailer": "Jumbo"
    },
    {
      "_id": {
        "$oid": "639c33953990e1cff61951a4"
      },
      "date_run": "2022-12-16",
      "steps": {
        "link_crawling": {
          "status": true,
          "error": ""
        },
        "link_check": {
          "status": true,
          "error": ""
        },
        "product_fetch_compare": {
          "status": true,
          "error": ""
        },
        "save_to_database": {
          "status": true,
          "error": ""
        }
      },
      "retailer": "Albert Heijn"
    },
    {
      "_id": {
        "$oid": "639c33bc3990e1cff61951b4"
      },
      "date_run": "2022-12-16",
      "steps": {
        "link_crawling": {
          "status": true,
          "error": ""
        },
        "link_check": {
          "status": true,
          "error": ""
        },
        "product_fetch_compare": {
          "status": true,
          "error": ""
        },
        "save_to_database": {
          "status": true,
          "error": ""
        }
      },
      "retailer": "Jumbo"
    },
    {
      "_id": {
        "$oid": "639c38626a9db0971716e0e1"
      },
      "date_run": "2022-12-16",
      "steps": {
        "link_crawling": {
          "status": true,
          "error": ""
        },
        "link_check": {
          "status": true,
          "error": ""
        },
        "product_fetch_compare": {
          "status": true,
          "error": ""
        },
        "save_to_database": {
          "status": true,
          "error": ""
        }
      },
      "retailer": "Jumbo"
    },
    {
      "_id": {
        "$oid": "639c396ed362236e51f8804e"
      },
      "date_run": "2022-12-16",
      "steps": {
        "link_crawling": {
          "status": true,
          "error": ""
        },
        "link_check": {
          "status": true,
          "error": ""
        },
        "product_fetch_compare": {
          "status": true,
          "error": ""
        },
        "save_to_database": {
          "status": true,
          "error": ""
        }
      },
      "retailer": "Albert Heijn"
    },
    {
      "_id": {
        "$oid": "639c39f77c37bff4242d4d9c"
      },
      "date_run": "2022-12-16",
      "steps": {
        "link_crawling": {
          "status": false,
          "error": "[ERROR] Could not crawl the given URL."
        },
        "link_check": {
          "status": true,
          "error": ""
        },
        "product_fetch_compare": {
          "status": true,
          "error": ""
        },
        "save_to_database": {
          "status": true,
          "error": ""
        }
      },
      "retailer": "Jumbo"
    }
  ],
  "allAdminSettings": [
    {
      "_id": {
        "$oid": "63760b736a6fa0bae61e4e85"
      },
      "day_to_scrape": "Friday",
      "time_to_scrape": "04:02"
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

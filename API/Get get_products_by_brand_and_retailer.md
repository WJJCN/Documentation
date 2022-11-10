**Voorbeeld**
----

/Hier zet je de bescrijving neer
  
* **URL**

  /get_products_by_brand_and_retailer

* **Method:**
 
  `GET`

* **Data Params**

  `{ brand : "Red Bull" }`
  `{ retailer : "Jumbo" }`

* **Success Response:**

  * **Code:** 200 <br />
    **Content:** `
    [
      {
        "_id": {
          "$oid": "6347e22f9d8358b9628b62e0"
        },
        "brand": "Red Bull",
        "retailer": "Jumbo",
        "product": "Red Bull Energy Drink - 250ml",
        "product_brand": {
            "brand": "Red Bull",
            "title": "Red Bull Energy Drink - 250ml",
            "short description 1": "Red Bull Energy Drink wordt wereldwijd gewaardeerd door topsporters.\r\n\r\n• Stimuleert Lichaam en Geest\r\n\r\n• Bevat cafeïne, taurine, vitamine B, suiker en water\r\n\r\n• De hoeveelheid suiker in een blikje van 250ml is vergelijkbaar met frisdrank: 11g/100ml\r\n\r\n• De hoeveelheid cafeïne in een blikje van 250ml is vergelijkbaar met een kopje koffie: 32mg/100ml\r\n\r\nEnergiedranken van Red Bull zijn te drinken als je onderweg bent, tijdens colleges en studiesessies, op het werk, tijdens het sporten, het spelen van videospelletjes, of tijdens het uitgaan, dag en nacht. Aluminium blik is oneindig recyclebaar na verzameling. Gooi je blikje daarom in de prullenbak en help zo het milieu.\r\n",
            "short description 2": "Stimuleert Lichaam en Geest. Red Bull Energy Drink wordt wereldwijd gewaardeerd door topatleten en studenten. Red Bull houdt je scherp, niet alleen tijdens het sporten of studeren maar ook bij prestatiegericht werk en lange autoritten. Het is een functionele drank die je vleugels geeft wanneer je ze nodig hebt.\r\n",
            "SEO": [
                "Energy",
                "Energydrink",
                "Energydrinks",
                "Energie"
            ],
            "bullit points": [
                "Stimuleert Lichaam en Geest®",
                "Een blikje bestaat uit 250ml en bevat cafeïne, taurine, vitamine B, suiker en water",
                "De hoeveelheid suiker is vergelijkbaar met frisdrank: 11g/100ml",
                "De hoeveelheid cafeïne is vergelijkbaar met een kopje koffie: 32mg/100ml"
            ]
        },
        "product_scraped": {
            "brand": "Red Bull",
            "title": "Red Bull Energy Drink - 250ml",
            "short description 1": "Red Bull Energy Drink wordt wereldwijd gewaardeerd door topsporters.\r\n\r\n• Stimuleert Lichaam en Geest\r\n\r\n• Bevat cafeïne, taurine, vitamine B, suiker en water\r\n\r\n• De hoeveelheid suiker in een blikje van 250ml is vergelijkbaar met frisdrank: 11g/100ml\r\n\r\n• De hoeveelheid cafeïne in een blikje van 250ml is vergelijkbaar met een kopje koffie: 32mg/100ml\r\n\r\nEnergiedranken van Red Bull zijn te drinken als je onderweg bent, tijdens colleges en studiesessies, op het werk, tijdens het sporten, het spelen van videospelletjes, of tijdens het uitgaan, dag en nacht. Aluminium blik is oneindig recyclebaar na verzameling. Gooi je blikje daarom in de prullenbak en help zo het milieu.\r\n",
            "short description 2": "Stimuleert Lichaam en Geest. Red Bull Energy Drink wordt wereldwijd gewaardeerd door topatleten en studenten. Red Bull houdt je scherp, niet alleen tijdens het sporten of studeren maar ook bij prestatiegericht werk en lange autoritten. Het is een functionele drank die je vleugels geeft wanneer je ze nodig hebt.\r\n",
            "SEO": [
                "Energy",
                "Energydrink",
                "Energydrinks",
                "Energie"
            ],
            "bullit points": [
                "Stimuleert Lichaam en Geest®",
                "Een blikje bestaat uit 250ml en bevat cafeïne, taurine, vitamine B, suiker en water",
                "De hoeveelheid suiker is vergelijkbaar met frisdrank: 11g/100ml",
                "De hoeveelheid cafeïne is vergelijkbaar met een kopje koffie: 32mg/100ml"
            ]
          }
        }
      }
    ]
    `
 
* **Error Response:**

  * **Code:** 403 Forbidden <br />
    **Content:** `{ "message" : "Forbidden" }`
    
  * **Code:** 400 Bad Request <br />
    **Content:** `{ "message" : "brand is not defined!" }`
    
  * **Code:** 400 Bad Request <br />
    **Content:** `{ "message" : "retailer is not defined!" }`

# quick-mongo-atlas-datasets

Quick way to load all sample MongoDB Atlas datasets

For available sample datasets in Atlas, please see [here](https://docs.atlas.mongodb.com/sample-data/available-sample-datasets/) for detail.

Table of contents:

- [quick-mongo-atlas-datasets](#quick-mongo-atlas-datasets)
  - [Quickstart](#quickstart)
  - [Available datasets](#available-datasets)
    - [Sample AirBnB Listings Dataset](#sample-airbnb-listings-dataset)
      - [Collections](#collections)
        - [`listingsAndReviews`](#listingsandreviews)
    - [Sample Geospatial Dataset](#sample-geospatial-dataset)
      - [Collections](#collections-1)
        - [`shipwrecks`](#shipwrecks)
    - [Sample Mflix Dataset](#sample-mflix-dataset)
      - [Collections](#collections-2)
        - [`comments`](#comments)
        - [`movies`](#movies)
        - [`sessions`](#sessions)
        - [`theaters`](#theaters)
        - [`users`](#users)
    - [Sample Supply Store Dataset](#sample-supply-store-dataset)
      - [Collections](#collections-3)
        - [`sales`](#sales)
    - [Sample Weather Dataset](#sample-weather-dataset)
      - [Collections](#collections-4)
        - [`data`](#data)
    - [Sample Training Dataset](#sample-training-dataset)
      - [Collections](#collections-5)
        - [`companies`](#companies)
        - [`grades`](#grades)
        - [`inspections`](#inspections)
        - [`posts`](#posts)
        - [`routes`](#routes)
        - [`stories`](#stories)
        - [`trips`](#trips)
        - [`tweets`](#tweets)
        - [`zips`](#zips)

## Quickstart

Clone this repository to download all dumped database files:

```bash
git clone https://github.com/huynhsamha/quick-mongo-atlas-datasets.git
cd quick-mongo-atlas-datasets
```

Start MongoDB on your localhost or server

Import database `sample_airbnb` to localhost:27017 with db name `airbnb`

```bash
mongorestore --host localhost --port 27017 --db airbnb --dir ./dump/sample_airbnb
```

Available datasets:

+ sample_airbnb
+ sample_geospatial
+ sample_mflix
+ sample_supplies
+ sample_training
+ sample_weatherdata

## Available datasets

### Sample AirBnB Listings Dataset

Directory: `./dump/sample_airbnb`

The `sample_airbnb` database is a compilation of vacation home listings and reviews

#### Collections

This database contains a single collection called `listingsAndReviews`.

##### `listingsAndReviews`

Sample Document

```json
{
  "_id": "10006546",
  "listing_url": "https://www.airbnb.com/rooms/10006546",
  "name": "Ribeira Charming Duplex",
  "summary": "Fantastic duplex apartment with three bedrooms, located in the historic area of Porto, Ribeira (Cube)...",
  "interaction": "Cot - 10 € / night Dog - € 7,5 / night",
  "house_rules": "Make the house your home...",
  "property_type": "House",
  "room_type": "Entire home/apt",
  "bed_type": "Real Bed",
  "minimum_nights": "2",
  "maximum_nights": "30",
  "cancellation_policy": "moderate",
  "last_scraped": {
    "$date": {
      "$numberLong": "1550293200000"
    }
  },
  "calendar_last_scraped": {
    "$date": {
      "$numberLong": "1550293200000"
    }
  },
  "first_review": {
    "$date": {
      "$numberLong": "1451797200000"
    }
  },
  "last_review": {
    "$date": {
      "$numberLong": "1547960400000"
    }
  },
  "accommodates": {
    "$numberInt": "8"
  },
  "bedrooms": {
    "$numberInt": "3"
  },
  "beds": {
    "$numberInt": "5"
  },
  "number_of_reviews": {
    "$numberInt": "51"
  },
  "bathrooms": {
    "$numberDecimal": "1.0"
  },
  "amenities": [
    "TV",
    "Cable TV",
    ...
    "Cleaning before checkout",
    "Waterfront"
  ],
  "price": {
    "$numberDecimal": "80.00"
  },
  "security_deposit": {
    "$numberDecimal": "200.00"
  },
  "cleaning_fee": {
    "$numberDecimal": "35.00"
  },
  "extra_people": {
    "$numberDecimal": "15.00"
  },
  "guests_included": {
    "$numberDecimal": "6"
  },
  "images": {
    "thumbnail_url": "",
    "medium_url": "",
    "picture_url": "https://a0.muscache.com/im/pictures/e83e702f-ef49-40fb-8fa0-6512d7e26e9b.jpg?aki_policy=large",
    "xl_picture_url": ""
  },
  "host": {
    "host_id": "51399391",
    "host_url": "https://www.airbnb.com/users/show/51399391",
    "host_name": "Ana&Gonçalo",
    "host_location": "Porto, Porto District, Portugal",
    "host_about": "Gostamos de passear, de viajar, de conhecer pessoas e locais novos, gostamos de desporto e animais! Vivemos na cidade mais linda do mundo!!!",
    "host_response_time": "within an hour",
    "host_thumbnail_url": "https://a0.muscache.com/im/pictures/fab79f25-2e10-4f0f-9711-663cb69dc7d8.jpg?aki_policy=profile_small",
    "host_picture_url": "https://a0.muscache.com/im/pictures/fab79f25-2e10-4f0f-9711-663cb69dc7d8.jpg?aki_policy=profile_x_medium",
    "host_neighbourhood": "",
    "host_response_rate": {
      "$numberInt": "100"
    },
    "host_is_superhost": false,
    "host_has_profile_pic": true,
    "host_identity_verified": true,
    "host_listings_count": {
      "$numberInt": "3"
    },
    "host_total_listings_count": {
      "$numberInt": "3"
    },
    "host_verifications": [
      "email",
      "phone",
      "reviews",
      "jumio",
      "offline_government_id",
      "government_id"
    ]
  },
  "address": {
    "street": "Porto, Porto, Portugal",
    "suburb": "",
    "government_area": "Cedofeita, Ildefonso, Sé, Miragaia, Nicolau, Vitória",
    "market": "Porto",
    "country": "Portugal",
    "country_code": "PT",
    "location": {
      "type": "Point",
      "coordinates": [
        {
          "$numberDouble": "-8.61308"
        },
        {
          "$numberDouble": "41.1413"
        }
      ],
      "is_location_exact": false
    }
  },
  "availability": {
    "availability_30": {
      "$numberInt": "28"
    },
    "availability_60": {
      "$numberInt": "47"
    },
    "availability_90": {
      "$numberInt": "74"
    },
    "availability_365": {
      "$numberInt": "239"
    }
  },
  "review_scores": {
    "review_scores_accuracy": {
      "$numberInt": "9"
    },
    "review_scores_cleanliness": {
      "$numberInt": "9"
    },
    "review_scores_checkin": {
      "$numberInt": "10"
    },
    "review_scores_communication": {
      "$numberInt": "10"
    },
    "review_scores_location": {
      "$numberInt": "10"
    },
    "review_scores_value": {
      "$numberInt": "9"
    },
    "review_scores_rating": {
      "$numberInt": "89"
    }
  },
  "reviews": [
    {
      "_id": "362865132",
      "date": {
        "$date": {
          "$numberLong": "1545886800000"
        }
      },
      "listing_id": "10006546",
      "reviewer_id": "208880077",
      "reviewer_name": "Thomas",
      "comments": "Very helpful hosts. Cooked traditional..."
    },
    {
      "_id": "364728730",
      "date": {
        "$date": {
          "$numberLong": "1546232400000"
        }
      },
      "listing_id": "10006546",
      "reviewer_id": "91827533",
      "reviewer_name": "Mr",
      "comments": "Ana & Goncalo were great on communication..."
    },
    {
      "_id": "403055315",
      "date": {
        "$date": {
          "$numberLong": "1547960400000"
        }
      },
      "listing_id": "10006546",
      "reviewer_id": "15138940",
      "reviewer_name": "Milo",
      "comments": "The house was extremely well located..."
    }
  ]
}
```

### Sample Geospatial Dataset

Directory: `./dump/sample_geospatial`

The `sample_geospatial` database contains data specifically designed to help familiarize you with GeoJSON data.

#### Collections

This database contains a single collection called `shipwrecks`.

##### `shipwrecks`

Sample Document

```json
{
  "_id": {
    "$oid": "578f6fa2df35c7fbdbaed8c6"
  },
  "recrd": "",
  "vesslterms": "",
  "feature_type": "Wrecks - Submerged, dangerous",
  "chart": "US,U1,graph,DNC H1409860",
  "latdec": {
    "$numberDouble": "9.3560572"
  },
  "londec": {
    "$numberDouble": "-79.9074173"
  },
  "gp_quality": "",
  "depth": "",
  "sounding_type": "",
  "history": "",
  "quasou": "depth unknown",
  "watlev": "always under water/submerged",
  "coordinates": [
    {
      "$numberDouble": "-79.9074173"
    },
    {
      "$numberDouble": "9.3560572"
    }
  ]
}
```

### Sample Mflix Dataset

Directory: `./dump/sample_mflix`

The `sample_mflix` database contains data on movies and movie theaters. The database also contains collections for certain metadata, including users and comments on specific movies.

#### Collections

The sample_mflix database contains the following collections:

| Collection Name | Description                                                                |
| --------------- | -------------------------------------------------------------------------- |
| **comments**    | Contains comments associated with specific movies.                         |
| **movies**      | Contains movie information, including release year, director, and reviews. |
| **sessions**    | Metadata field. Contains users’ JSON Web Tokens.                           |
| **theaters**    | Contains locations of movie theaters.                                      |
| **users**       | Contains user information.                                                 |

##### `comments`

Sample Document

```json
{
  "_id": {
    "$oid": "5a9427648b0beebeb69579cc"
  },
  "name": "Andrea Le",
  "email": "andrea_le@fakegmail.com",
  "movie_id": {
    "$oid": "573a1390f29313caabcd418c"
  },
  "text": "Rem officiis eaque repellendus amet eos doloribus. Porro
    dolor voluptatum voluptates neque culpa molestias. Voluptate unde
    nulla temporibus ullam.",
  "date": {
    "$date": {
      "$numberLong": "1332804016000"
    }
  }
}
```

##### `movies`

Sample Document

```json
{
  "_id": {
    "$oid": "573a1390f29313caabcd413b"
  },
  "title": "The Arrival of a Train",
  "year": {
    "$numberInt": "1896"
  },
  "runtime": {
    "$numberInt": "1"
  },
  "released": {
    "$date": {
      "$numberLong": "-2335219200000"
    }
  },
  "poster": "http://ia.media-imdb.com/images/M/MV5BMjEyNDk5MDYzOV5BMl5BanBnXkFtZTgwNjIxMTEwMzE@._V1_SX300.jpg",
  "plot": "A group of people are standing in a straight line along the
    platform of a railway station, waiting for a train, which is seen
    coming at some distance. When the train stops at the platform, ...",
  "fullplot": "A group of people are standing in a straight line along
    the platform of a railway station, waiting for a train, which is
    seen coming at some distance. When the train stops at the platform,
    the line dissolves. The doors of the railway-cars open, and people
    on the platform help passengers to get off.",
  "lastupdated": "2015-08-15 00:02:53.443000000",
  "type": "movie",
  "directors": [
    "Auguste Lumière",
    "Louis Lumière"
  ],
  "imdb": {
    "rating": {
      "$numberDouble": "7.3"
    },
    "votes": {
      "$numberInt": "5043"
    },
    "id": {
      "$numberInt": "12"
    }
  },
  "countries": [
    "France"
  ],
  "genres": [
    "Documentary",
    "Short"
  ],
  "tomatoes": {
    "viewer": {
      "rating": {
        "$numberDouble": "3.7"
      },
      "numReviews": {
        "$numberInt": "59"
      }
    },
    "lastUpdated": {
      "$date": {
        "$numberLong": "1441993589000"
      }
    }
  },
  "num_mflix_comments": {
    "$numberInt": "1"
  }
}
```

##### `sessions`

Sample Document

```json
{
  "_id": {
    "$oid": "5a98348755593fdf68350932"
  },
  "user_id": "bfb9vc1zz@xhasq.5h9",
  "jwt": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9..."
}
```

##### `theaters`

Sample Document

```json
{
  "_id": {
    "$oid": "59a47286cfa9a3a73e51e72c"
  },
  "theaterId": {
    "$numberInt": "1000"
  },
  "location": {
    "address": {
      "street1": "340 W Market",
      "city": "Bloomington",
      "state": "MN",
      "zipcode": "55425"
    },
    "geo": {
      "type": "Point",
      "coordinates": [
        {
          "$numberDouble": "-93.24565"
        },
        {
          "$numberDouble": "44.85466"
        }
      ]
    }
  }
}
```

##### `users`

Sample Document

```json
{
  "_id": {
    "$oid": "59b99db4cfa9a34dcd7885b6"
  },
  "name": "Ned Stark",
  "email": "sean_bean@gameofthron.es",
  "password": "$2b$12$UREFwsRUoyF0CRqGNK0LzO0HM/jLhgUCNNIJ9RJAqMUQ74crlJ1Vu"
}
```

### Sample Supply Store Dataset

Directory: `./dump/sample_supplies`

The `sample_supplies` database contains data from a mock office supply company. The company tracks customer information and sales data, and has several store locations throughout the world.

#### Collections

This database contains a single collection called `sales`.

##### `sales`

Sample Document

```json
{
  "_id": {
    "$oid": "5bd761dcae323e45a93ccfe8"
  },
  "saleDate": {
    "$date": {
      "$numberLong": "1427144809506"
    }
  },
  "items": [
    {
      "name": "notepad",
      "tags": [
        "office",
        "writing",
        "school"
      ],
      "price": {
        "$numberDecimal": "35.29"
      },
      "quantity": {
        "$numberInt": "2"
      }
    },
    {
      "name": "pens",
      "tags": [
        "writing",
        "office",
        "school",
        "stationary"
      ],
      "price": {
        "$numberDecimal": "56.12"
      },
      "quantity": {
        "$numberInt": "5"
      }
    },
    {
      "name": "envelopes",
      "tags": [
        "stationary",
        "office",
        "general"
      ],
      "price": {
        "$numberDecimal": "19.95"
      },
      "quantity": {
        "$numberInt": "8"
      }
    },
    {
      "name": "binder",
      "tags": [
        "school",
        "general",
        "organization"
      ],
      "price": {
        "$numberDecimal": "14.16"
      },
      "quantity": {
        "$numberInt": "3"
      }
    }
  ],
  "storeLocation": "Denver",
  "customer": {
    "gender": "M",
    "age": {
      "$numberInt": "42"
    },
    "email": "cauho@witwuta.sv",
    "satisfaction": {
      "$numberInt": "4"
    }
  },
  "couponUsed": true,
  "purchaseMethod": "Online"
}
```

### Sample Weather Dataset

Directory: `./dump/sample_weatherdata`

The `sample_weatherdata` database contains detailed weather reports from various locations. Each report contains readings such as airTemperature, wind, and visibility. Each report contains a location which is stored as GeoJSON.

#### Collections

This database contains a single collection called `data`.

##### `data`

Sample Document

```json
{
  "_id": {
    "$oid": "5553a998e4b02cf7151190c9"
  },
  "st": "x+51900+003200",
  "ts": {
    "$date": {
      "$numberLong": "447354000000"
    }
  },
  "position": {
    "type": "Point",
    "coordinates": [
      {
        "$numberDouble": "3.2"
      },
      {
        "$numberDouble": "51.9"
      }
    ]
  },
  "elevation": {
    "$numberInt": "9999"
  },
  "callLetters": "PLAT",
  "qualityControlProcess": "V020",
  "dataSource": "4",
  "type": "FM-13",
  "airTemperature": {
    "value": {
      "$numberDouble": "4.8"
    },
    "quality": "1"
  },
  "dewPoint": {
    "value": {
      "$numberDouble": "4.6"
    },
    "quality": "1"
  },
  "pressure": {
    "value": {
      "$numberDouble": "1032.6"
    },
    "quality": "1"
  },
  "wind": {
    "direction": {
      "angle": {
        "$numberInt": "170"
      },
      "quality": "1"
    },
    "type": "N",
    "speed": {
      "rate": {
        "$numberDouble": "0.5"
      },
      "quality": "1"
    }
  },
  "visibility": {
    "distance": {
      "value": {
        "$numberInt": "999999"
      },
      "quality": "9"
    },
    "variability": {
      "value": "N",
      "quality": "9"
    }
  },
  "skyCondition": {
    "ceilingHeight": {
      "value": {
        "$numberInt": "99999"
      },
      "quality": "9",
      "determination": "9"
    },
    "cavok": "N"
  },
  "sections": [
    "AG1",
    "MD1",
    "OA1",
    "SA1"
  ],
  "precipitationEstimatedObservation": {
    "discrepancy": "2",
    "estimatedWaterDepth": {
      "$numberInt": "999"
    }
  },
  "atmosphericPressureChange": {
    "tendency": {
      "code": "2",
      "quality": "1"
    },
    "quantity3Hours": {
      "value": {
        "$numberDouble": "1.2"
      },
      "quality": "1"
    },
    "quantity24Hours": {
      "value": {
        "$numberDouble": "99.9"
      },
      "quality": "9"
    }
  },
  "seaSurfaceTemperature": {
    "value": {
      "$numberDouble": "5.5"
    },
    "quality": "9"
  }
}
```

### Sample Training Dataset

Directory: `./dump/sample_training`

The `sample_training` database contains a set of realistic data.

#### Collections

The `sample_training` database contains the following collections:

| Collection Name | Description                                                                                                                                                                                                  |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| companies       | Contains a list of Crunchbase Data company information.                                                                                                                                                      |
| grades          | Contains student grade information on a given class, including scores on different assessments.                                                                                                              |
| inspections     | Contains a list of New York City business inspections, including whether the business failed or passed the inspection.                                                                                       |
| posts           | Contains randomized US Senate speeches organized as blog posts with randomly generated comments.                                                                                                             |
| routes          | Contains information of airline routes, with source and destination airports, the service airline and the type of airplane. This collection is used in labs that explore the $graphLookup aggregation stage. |
| stories         | Contains Digg stories, a website for sharing and commenting on online content.                                                                                                                               |
| trips           | Contains New York City Citibike Data trips data. This data is useful to explore the $graphLookup aggregation stage and showcase Geospatial Queries.                                                          |
| tweets          | Contains tweet data from Twitter Decahose stream service.                                                                                                                                                    |
| zips            | Contains United States general cities postal/zip code data.                                                                                                                                                  |

##### `companies`

Sample Document

```json
{
  "_id": {
      "$oid": "52cdef7c4bab8bd675298291"
  },
  "acquisition": null,
  "acquisitions": [],
  "alias_list": null,
  "blog_feed_url": "http://mobiance.wordpress.com/feed/",
  "blog_url": "http://mobiance.wordpress.com/",
  "category_code": "web",
  "competitions": [],
  "created_at": "Tue Feb 12 17:31:58 UTC 2008",
  "crunchbase_url": "http://www.crunchbase.com/company/mobiance",
  "deadpooled_day": null,
  "deadpooled_month": null,
  "deadpooled_url": null,
  "deadpooled_year": null,
  "description": null,
  "email_address": "info@mobiance.com",
  "external_links": [],
  "founded_day": {
      "$numberInt": "1"
  },
  "founded_month": {
      "$numberInt": "10"
  },
  "founded_year": {
      "$numberInt": "2004"
  },
  "funding_rounds": [],
  "homepage_url": "http://www.mobiance.com",
  "image": {
      "attribution": null,
      "available_sizes": [
          [
              [
                  {
                      "$numberInt": "150"
                  },
                  {
                      "$numberInt": "43"
                  }
              ],
              "assets/images/resized/0001/1859/11859v1-max-150x150.png"
          ],
          [
              [
                  {
                      "$numberInt": "208"
                  },
                  {
                      "$numberInt": "60"
                  }
              ],
              "assets/images/resized/0001/1859/11859v1-max-250x250.png"
          ],
          [
              [
                  {
                      "$numberInt": "208"
                  },
                  {
                      "$numberInt": "60"
                  }
              ],
              "assets/images/resized/0001/1859/11859v1-max-450x450.png"
          ]
      ]
  },
  "investments": [],
  "ipo": null,
  "milestones": [],
  "name": "Mobiance",
  "number_of_employees": {
      "$numberInt": "5"
  },
  "offices": [
      {
          "address1": "BC-3, Atrium Business Center,",
          "address2": "Coles Road, Frazer Town,",
          "city": "Bangalore",
          "country_code": "IND",
          "description": null,
          "latitude": null,
          "longitude": null,
          "state_code": null,
          "zip_code": "560005"
      }
  ],
  "overview": "<p>Mobiance provides the technology to track cell phones ...",
  "partners": [],
  "permalink": "mobiance",
  "phone_number": "+91-80- 41264756",
  "products": [],
  "providerships": [],
  "relationships": [
      {
          "is_past": true,
          "person": {
              "first_name": "Ritesh",
              "last_name": "Ambastha",
              "permalink": "ritesh-ambastha"
          },
          "title": "Product Manager"
      }
  ],
  "screenshots": [],
  "tag_list": null,
  "total_money_raised": "$0",
  "twitter_username": null,
  "updated_at": "Thu Dec 01 07:37:10 UTC 2011",
  "video_embeds": []
}
```

##### `grades`

Sample Document

```json
{
    "_id": {
        "$oid": "56d5f7eb604eb380b0d8d8fa"
    },
    "class_id": {
        "$numberDouble": "173"
    },
    "scores": [
        {
            "score": {
                "$numberDouble": "19.81430597438296"
            },
            "type": "exam"
        },
        {
            "score": {
                "$numberDouble": "16.851404299968642"
            },
            "type": "quiz"
        },
        {
            "score": {
                "$numberDouble": "60.108751761488186"
            },
            "type": "homework"
        },
        {
            "score": {
                "$numberDouble": "22.886167083915776"
            },
            "type": "homework"
        }
    ],
    "student_id": {
        "$numberDouble": "4"
    }
}
```

##### `inspections`

Sample Document

```json
{
   "_id": {
     "$oid": "56d61033a378eccde8a8357e"
   },
   "address": {
       "city": "LAWRENCE",
       "number": 1,
       "street": "BAY BLVD",
       "zip": 11559
   },
   "business_name": "SPRAGUE OPERATING RESOURCES LLC.",
   "certificate_number": 3019422,
   "date": "Mar  3 2015",
   "id": "11247-2015-ENFO",
   "result": "Fail",
   "sector": "Fuel Oil Dealer - 814"
}
```

##### `posts`

Sample Document

```json
{
    "_id": {
      "$oid": "50ab0f8bbcf1bfe2536dc3f9"
    },
    "author": "machine",
    "body": "Amendment I\n<p>Congress shall make no law respecting ...  ",
    "comments": [
        {
            "author": "Santiago Dollins",
            "body": "Lorem ipsum dolor sit amet, consectetur adipisicing...",
            "email": "HvizfYVx@pKvLaagH.com"
        },
        {
            "author": "Jaclyn Morado",
            "body": "Lorem ipsum dolor sit amet, consectetur adipisicing...",
            "email": "WpOUCpdD@hccdxJvT.com"
        }
        ...
    ],
    "date": {
      "$date": {
        "$numberLong": "1332804016000"
      }
    },
    "permalink": "aRjNnLZkJkTyspAIoRGe",
    "tags": [
        "watchmaker",
        "santa",
        "xylophone",
        "math",
        "handsaw",
        "dream",
        "undershirt",
        "dolphin",
        "tanker",
        "action"
    ],
    "title": "Bill of Rights"
}
```

##### `routes`

Sample Document

```json
{
     "_id": {
       "$oid": "56e9b39b732b6122f877fa5c"
     },
     "airline": {
         "alias": "2G",
         "iata": "CRG",
         "id": 1654,
         "name": "Cargoitalia"
     },
     "airplane": "A81",
     "codeshare": "",
     "dst_airport": "OVB",
     "src_airport": "BTK",
     "stops": 0
 }
```

##### `stories`

Sample Document

```json
{
    "_id": {
      "$oid": "4ba2681f238d3ba3ca000065"
    },
    "comments": 79,
    "container": {
        "name": "Science",
        "short_name": "science"
    },
    "description": "Today's youth are generally not the self-centered,...",
    "diggs": 493,
    "href": "http://digg.com/general_sciences/Study_Today_s_youth_a...",
    "id": "19955283",
    "link": "http://www.brainmysteries.com/research/Study_Todays_yo...",
    "media": "news",
    "promote_date": 1268866803,
    "shorturl": [
        {
            "short_url": "http://digg.com/d31LjHP",
            "view_count": 2109
        }
    ],
    "status": "popular",
    "submit_date": 1268725903,
    "thumbnail": {
        "contentType": "image/jpeg",
        "height": 80,
        "originalheight": 232,
        "originalwidth": 350,
        "src": "http://digg.com/general_sciences/Study_Today_s_youth_...",
        "width": 80
    },
    "title": "Study: Today's youth aren't ego-driven slackers after all ",
    "topic": {
        "name": "General Sciences",
        "short_name": "general_sciences"
    },
    "user": {
        "icon": "http://digg.com/users/lekahe/l.png",
        "name": "lekahe",
        "profileviews": 63011,
        "registered": 1187263066
    }
}
```

##### `trips`

Sample Document

```json
{
    "_id": {
      "$oid": "572bb8222b288919b68abf82"
    },
    "bikeid": 14785,
    "birth year": 1977,
    "end station id": 433,
    "end station location": {
        "coordinates": [
            -73.98057249,
            40.72955361
        ],
        "type": "Point"
    },
    "end station name": "E 13 St & Avenue A",
    "gender": 1,
    "start station id": 518,
    "start station location": {
        "coordinates": [
            -73.9734419,
            40.74780373
        ],
        "type": "Point"
    },
    "start station name": "E 39 St & 2 Ave",
    "start time": {
      "$date": {
        "$numberLong": "1332804016000"
      }
    },
    "stop time": {
      "$date": {
        "$numberLong": "1352114016000"
      }
    },
    "tripduration": 812,
    "usertype": "Subscriber"
}
```

##### `tweets`

Sample Document

```json
{
  "_id": {
    "$oid": "5c8eccb0caa187d17ca62433"
  },
  "contributors": null,
  "coordinates": null,
  "created_at": "Thu Sep 02 18:11:30 +0000 2010",
  "entities": {
      "hashtags": [
          {
              "indices": [
                  0,
                  16
              ],
              "text": "IEGreekStepShow"
          }
      ],
      "urls": [],
      "user_mentions": []
  },
  "favorited": false,
  "geo": null,
  "id": "22819404700",
  "in_reply_to_screen_name": null,
  "in_reply_to_status_id": null,
  "in_reply_to_user_id": null,
  "place": null,
  "retweet_count": null,
  "retweeted": false,
  "source": "<a href=\"http://blackberry.com/twitter\" ...",
  "text": "#IEGreekStepShow I'm there.. Are you?",
  "truncated": false,
  "user": {
      "contributors_enabled": false,
      "created_at": "Mon Apr 13 23:24:53 +0000 2009",
      "description": "We are a team of people who specialize in: ...",
      "favourites_count": 11,
      "follow_request_sent": null,
      "followers_count": 988,
      "following": null,
      "friends_count": 1371,
      "geo_enabled": false,
      "id": 30990697,
      "lang": "en",
      "listed_count": 29,
      "location": "ANYWHERE We are NEEDED!!!",
      "name": "Juan Young II",
      "notifications": null,
      "profile_background_color": "000000",
      "profile_background_image_url": "http://a1.twimg.com/profile_backg...",
      "profile_background_tile": true,
      "profile_image_url": "http://a2.twimg.com/profile_images/110364584...",
      "profile_link_color": "CC3300",
      "profile_sidebar_border_color": "FFFFFF",
      "profile_sidebar_fill_color": "F7DA93",
      "profile_text_color": "000000",
      "profile_use_background_image": true,
      "protected": false,
      "screen_name": "juanyoungonline",
      "show_all_inline_media": false,
      "statuses_count": 14804,
      "time_zone": "Pacific Time (US & Canada)",
      "url": "http://www.hard2please-ent.com",
      "utc_offset": -28800,
      "verified": false
  }
}
```

##### `zips`

Sample Document

```json
{
  "_id": {
    "$oid": "5c8eccc1caa187d17ca6ed29"
  },
  "city": "CLEVELAND",
  "loc": {
      "x": 86.559355,
      "y": 33.992106
  },
  "pop": 2369,
  "state": "AL",
  "zip": "35049"
}
```

# E-Commerce Sample Set

I had a hard time finding a sample set of e-commerce items that was sufficiently large enough to test out anything of scale. Hope this helps in your testing!

This sample set was built with data from [Faker.js](https://github.com/marak/Faker.js/) and images from the free [Re:splashed](http://www.resplashed.com/) collection (individual artists noted in the JSON file). I wrote a compositing script with GraphicsMagick to combine the Re:splashed images with a couple of line-art vectors (mugs and shirts).

The mug vector was adapted from [Arnaud.ramey work on wikipedia](https://en.wikipedia.org/wiki/File:Mug.svg) (Creative Commons  Attribution-Share Alike 3.0 Unported)

The shirt vector was adapted from [IKorteXI](http://ikortexi.deviantart.com/art/Shirt-Template-67136327?) (no formal license, but assumed public domain by the line "Shirt template i made that anyone can use. Credit appreciated.")

## JSON Structure
```
  {
    //information from resplashed
    "imageCredit": {
      "artist": "Edoardo Loru",
      "link": "http://www.resplashed.com/photographer/edoardo_loru/"
    },
    //Tags from resplashed
    "tags": [
      "Sunset"
    ],
    //The original image from resplashed
    "imageUrl": "http://www.resplashed.com/img/400_be82688cef75.jpg",
    //the original filename from resplashed
    "filename": "400_be82688cef75.jpg",
    //Unique MD5 hash based on the filename
    "imageHash": "e3d9f0a1cd0fa5c4ee6b29fb190ff5b3",
    //randomly generated price
    "price": 12.99,
    //name generated from the item type, a random tag, and a random adjective
    "name": "Rustic Sunset Mug",
    //Random lorem ipsum description
    "description": "similique doloremque magni deserunt omnis quae praesentium adipisci voluptate fuga voluptatem",
    //Unique "slug" based on the name
    "slug": "Rustic-Sunset-Mug-1",
    //Date added (Feb 2017) in javascript timestamp format
    "added": 1485373038397,
    //links to the manufacturer.json file, which has a handful of random fake companies
    "manufacturer": "Lowe-Wunsch-and-Stoltenberg",
    //will either be 'mug' or 'shirt'
    "itemType": "mug",
    //The composited image - made up of the item type and original filename
    "productImg": "mug-400_be82688cef75.jpg"
  },
```


## Liscense
Creative Commons Attribution-Share Alike 3.0 Unported
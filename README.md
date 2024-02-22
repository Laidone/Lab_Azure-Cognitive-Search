# Lab_Azure-Cognitive-Search
Para se configurar uma pesquisa, precisamos fornecer o que queremos no formato JSON

Terminado de fazer toda a configuração do Azure Cognitive Search fiz um teste para sentimentos positivos usando o JSON que criei

{
 "search": "sentiment:'positive'",
 "count": true
}

O resultado foi 7 dados de conotação positiva.
As frases especificas são encontradas na chave com o nome "merged_content".
Essa ferramenta é muito útil para uma companhia como um grande volume de documentos e precisa fazer análises desses documentos

Segue o resultado completo do JSON



{
  "@odata.context": "https://labsearchhhh.search.windows.net/indexes('coffee-index')/$metadata#docs(*)",
  "@odata.count": 7,
  "value": [
    {
      "@search.score": 0.6931472,
      "content": "\n\nReview: I love the coffee drinks here, but my favorite part is the local art they sell. There are many kinds of paintings and watercolors they showcase each week. I love checking out the new prints that they have and buying cards for friends. Also did I mention that the wi-fi is excellent? \nDate: September 3, 2018\nLocation: Seattle, Washington  \nimage1.png\n\n\n\nimage2.png\n\n\n\n",
      "metadata_storage_path": "aHR0cHM6Ly9zdG9hZ2VpYWNvbnQuYmxvYi5jb3JlLndpbmRvd3MubmV0L2NvZmZlZXJldmlld3MvcmV2aWV3LTEuZG9jeA2",
      "locations": [
        "Seattle",
        "Washington"
      ],
      "keyphrases": [
        "coffee drinks",
        "favorite part",
        "local art",
        "many kinds",
        "new prints",
        "Review",
        "paintings",
        "watercolors",
        "cards",
        "friends",
        "wi-fi",
        "Date",
        "September",
        "Location",
        "Seattle",
        "Washington"
      ],
      "sentiment": "[\"positive\"]",
      "merged_content": "\n\nReview: I love the coffee drinks here, but my favorite part is the local art they sell. There are many kinds of paintings and watercolors they showcase each week. I love checking out the new prints that they have and buying cards for friends. Also did I mention that the wi-fi is excellent? \nDate: September 3, 2018\nLocation: Seattle, Washington  \nimage1.png\n  \n\n\nimage2.png\n  \n\n\n",
      "text": [
        "",
        ""
      ],
      "layoutText": [
        "{\"language\":\"en\",\"text\":\"\",\"lines\":[],\"words\":[]}",
        "{\"language\":\"en\",\"text\":\"\",\"lines\":[],\"words\":[]}"
      ],
      "imageTags": [
        "person",
        "human face",
        "clothing",
        "laptop",
        "table",
        "computer",
        "sitting",
        "outdoor",
        "indoor",
        "paint",
        "painting",
        "art",
        "child art",
        "indoor",
        "wall"
      ],
      "imageCaption": [
        "{\"tags\":[\"person\",\"laptop\",\"boy\"],\"captions\":[{\"text\":\"a person sitting at a table\",\"confidence\":0.46376612782478333}]}",
        "{\"tags\":[],\"captions\":[{\"text\":\"a wall with a painting on it\",\"confidence\":0.35804325342178345}]}"
      ]
    },
    {
      "@search.score": 0.2876821,
      "content": "\nReview: What I really like about this location is that there are also art classes offered for children! My family loves to come to Fourth Coffee on weekends for the live music and paint events! Some of the best events my kids have been to are at Fourth Coffee on a rainy Saturday. Hopefully they will bring back the Melodies & Collage Memories event, that was a great time for our whole family. \nDate: October 14, 2018\nLocation: Seattle, Washington  \nimage1.png\n\n\n\nimage2.png\n\n\n\n",
      "metadata_storage_path": "aHR0cHM6Ly9zdG9hZ2VpYWNvbnQuYmxvYi5jb3JlLndpbmRvd3MubmV0L2NvZmZlZXJldmlld3MvcmV2aWV3LTYuZG9jeA2",
      "locations": [
        "Fourth Coffee",
        "Seattle",
        "Washington"
      ],
      "keyphrases": [
        "Collage Memories event",
        "art classes",
        "Fourth Coffee",
        "live music",
        "paint events",
        "best events",
        "rainy Saturday",
        "great time",
        "Review",
        "location",
        "children",
        "family",
        "weekends",
        "kids",
        "Melodies",
        "Date",
        "October",
        "Seattle",
        "Washington"
      ],
      "sentiment": "[\"positive\"]",
      "merged_content": "\nReview: What I really like about this location is that there are also art classes offered for children! My family loves to come to Fourth Coffee on weekends for the live music and paint events! Some of the best events my kids have been to are at Fourth Coffee on a rainy Saturday. Hopefully they will bring back the Melodies & Collage Memories event, that was a great time for our whole family. \nDate: October 14, 2018\nLocation: Seattle, Washington  \nimage1.png\n 3 \n\n\nimage2.png\n  \n\n\n",
      "text": [
        "3",
        ""
      ],
      "layoutText": [
        "{\"language\":\"en\",\"text\":\"3\",\"lines\":[{\"boundingBox\":[{\"x\":434,\"y\":295},{\"x\":450,\"y\":294},{\"x\":451,\"y\":315},{\"x\":436,\"y\":316}],\"text\":\"3\"}],\"words\":[{\"boundingBox\":[{\"x\":434,\"y\":295},{\"x\":448,\"y\":294},{\"x\":449,\"y\":315},{\"x\":435,\"y\":316}],\"text\":\"3\"}]}",
        "{\"language\":\"en\",\"text\":\"\",\"lines\":[],\"words\":[]}"
      ],
      "imageTags": [
        "human face",
        "clothing",
        "person",
        "smile",
        "girl",
        "indoor",
        "toddler",
        "woman",
        "boy",
        "floor",
        "clothing",
        "person",
        "human face",
        "microphone",
        "bottle",
        "woman"
      ],
      "imageCaption": [
        "{\"tags\":[\"text\",\"person\",\"indoor\"],\"captions\":[{\"text\":\"a couple of girls holding a book\",\"confidence\":0.38007557392120361}]}",
        "{\"tags\":[\"person\"],\"captions\":[{\"text\":\"a person playing guitar\",\"confidence\":0.47499334812164307}]}"
      ]
    },
    {
      "@search.score": 0.2876821,
      "content": "\n\nReview: The great thing about this Fourth Coffee location is that there’s an event space for talks. I went to one the other day that focused on giving students a place to present their latest research. The event room is also perfect for larger groups or clubs to meet up. Just be aware that weekends it can get really crowded, which I don’t like. \nDate: October 11, 2018\nLocation: Los Angeles, California\t\nimage1.png\n\n\n\nimage2.png\n\n\n\n",
      "metadata_storage_path": "aHR0cHM6Ly9zdG9hZ2VpYWNvbnQuYmxvYi5jb3JlLndpbmRvd3MubmV0L2NvZmZlZXJldmlld3MvcmV2aWV3LTcuZG9jeA2",
      "locations": [
        "Fourth Coffee location",
        "event room",
        "Los Angeles",
        "California"
      ],
      "keyphrases": [
        "Fourth Coffee location",
        "great thing",
        "event space",
        "latest research",
        "event room",
        "larger groups",
        "Los Angeles",
        "Review",
        "talks",
        "students",
        "place",
        "clubs",
        "weekends",
        "Date",
        "October",
        "California"
      ],
      "sentiment": "[\"positive\"]",
      "merged_content": "\n\nReview: The great thing about this Fourth Coffee location is that there’s an event space for talks. I went to one the other day that focused on giving students a place to present their latest research. The event room is also perfect for larger groups or clubs to meet up. Just be aware that weekends it can get really crowded, which I don’t like. \nDate: October 11, 2018\nLocation: Los Angeles, California\t\nimage1.png\n  \n\n\nimage2.png\n . .. ..... \n\n\n",
      "text": [
        "",
        ". .. ....."
      ],
      "layoutText": [
        "{\"language\":\"en\",\"text\":\"\",\"lines\":[],\"words\":[]}",
        "{\"language\":\"en\",\"text\":\". .. .....\",\"lines\":[{\"boundingBox\":[{\"x\":371,\"y\":289},{\"x\":415,\"y\":282},{\"x\":417,\"y\":292},{\"x\":373,\"y\":298}],\"text\":\". ..\"},{\"boundingBox\":[{\"x\":366,\"y\":303},{\"x\":428,\"y\":294},{\"x\":429,\"y\":303},{\"x\":367,\"y\":312}],\"text\":\".....\"}],\"words\":[{\"boundingBox\":[{\"x\":377,\"y\":290},{\"x\":382,\"y\":289},{\"x\":383,\"y\":297},{\"x\":378,\"y\":298}],\"text\":\".\"},{\"boundingBox\":[{\"x\":391,\"y\":287},{\"x\":410,\"y\":284},{\"x\":411,\"y\":293},{\"x\":393,\"y\":296}],\"text\":\"..\"},{\"boundingBox\":[{\"x\":366,\"y\":304},{\"x\":424,\"y\":295},{\"x\":426,\"y\":304},{\"x\":368,\"y\":313}],\"text\":\".....\"}]}"
      ],
      "imageTags": [
        "clothing",
        "person",
        "indoor",
        "man",
        "footwear",
        "human face",
        "woman",
        "wall",
        "jeans",
        "people",
        "sitting",
        "group",
        "laptop",
        "indoor",
        "computer",
        "furniture",
        "wall",
        "desk",
        "table",
        "personal computer",
        "space bar",
        "output device",
        "netbook",
        "wooden",
        "touchpad",
        "coffee",
        "mac",
        "sitting",
        "floor"
      ],
      "imageCaption": [
        "{\"tags\":[\"person\",\"group\",\"people\"],\"captions\":[{\"text\":\"a person teaching a class\",\"confidence\":0.46982324123382568}]}",
        "{\"tags\":[\"text\",\"floor\",\"indoor\",\"wooden\",\"electronics\",\"wood\",\"computer\"],\"captions\":[{\"text\":\"a laptop on a table\",\"confidence\":0.49744489789009094}]}"
      ]
    },
    {
      "@search.score": 0.18232156,
      "content": "\n\nReview: The coffee tastings every Wednesday afternoon are so fun. Each month there is a new drink theme. You do need to book a spot in advance to attend. It is very worth it! I also love their local music. Fourth Coffee brings in rising artists every weekend. I like to head over there mid-afternoon on weekdays when it’s not too busy and get a slice of pie or their seasonal baked goods.  \nDate: August 13, 2018\nLocation: Chicago, Illinois  \n\nimage1.png\n\n\n\nimage2.png\n\n\n\n",
      "metadata_storage_path": "aHR0cHM6Ly9zdG9hZ2VpYWNvbnQuYmxvYi5jb3JlLndpbmRvd3MubmV0L2NvZmZlZXJldmlld3MvcmV2aWV3LTQuZG9jeA2",
      "locations": [
        "Fourth Coffee",
        "Chicago",
        "Illinois"
      ],
      "keyphrases": [
        "new drink theme",
        "seasonal baked goods",
        "coffee tastings",
        "local music",
        "Fourth Coffee",
        "rising artists",
        "ierican Coffee",
        "Review",
        "afternoon",
        "spot",
        "advance",
        "weekdays",
        "slice",
        "pie",
        "Date",
        "August",
        "Location",
        "Chicago",
        "Illinois"
      ],
      "sentiment": "[\"positive\"]",
      "merged_content": "\n\nReview: The coffee tastings every Wednesday afternoon are so fun. Each month there is a new drink theme. You do need to book a spot in advance to attend. It is very worth it! I also love their local music. Fourth Coffee brings in rising artists every weekend. I like to head over there mid-afternoon on weekdays when it’s not too busy and get a slice of pie or their seasonal baked goods.  \nDate: August 13, 2018\nLocation: Chicago, Illinois  \n\nimage1.png\n ierican Coffee 114 10148/0034 \n\n\nimage2.png\n  \n\n\n",
      "text": [
        "ierican Coffee 114 10148/0034",
        ""
      ],
      "layoutText": [
        "{\"language\":\"en\",\"text\":\"ierican Coffee 114 10148/0034\",\"lines\":[{\"boundingBox\":[{\"x\":701,\"y\":284},{\"x\":649,\"y\":303},{\"x\":647,\"y\":297},{\"x\":699,\"y\":279}],\"text\":\"ierican Coffee\"},{\"boundingBox\":[{\"x\":682,\"y\":241},{\"x\":614,\"y\":263},{\"x\":611,\"y\":251},{\"x\":678,\"y\":228}],\"text\":\"114 10148/0034\"}],\"words\":[{\"boundingBox\":[{\"x\":701,\"y\":285},{\"x\":679,\"y\":293},{\"x\":676,\"y\":287},{\"x\":699,\"y\":279}],\"text\":\"ierican\"},{\"boundingBox\":[{\"x\":676,\"y\":294},{\"x\":652,\"y\":303},{\"x\":650,\"y\":297},{\"x\":674,\"y\":288}],\"text\":\"Coffee\"},{\"boundingBox\":[{\"x\":682,\"y\":242},{\"x\":672,\"y\":245},{\"x\":668,\"y\":232},{\"x\":678,\"y\":229}],\"text\":\"114\"},{\"boundingBox\":[{\"x\":669,\"y\":245},{\"x\":618,\"y\":262},{\"x\":615,\"y\":251},{\"x\":666,\"y\":233}],\"text\":\"10148/0034\"}]}",
        "{\"language\":\"en\",\"text\":\"\",\"lines\":[],\"words\":[]}"
      ],
      "imageTags": [
        "food",
        "chocolate",
        "table",
        "cup",
        "serveware",
        "indoor",
        "cocoa solids",
        "caffeine",
        "tableware",
        "sitting",
        "coffee",
        "dessert",
        "musical instrument",
        "music",
        "concert",
        "clothing",
        "person",
        "string instrument",
        "human face",
        "microphone",
        "plucked string instruments",
        "acoustic guitar",
        "guitar",
        "indoor",
        "woman"
      ],
      "imageCaption": [
        "{\"tags\":[\"cup\",\"coffee\",\"table\",\"indoor\",\"pastry\",\"beverage\",\"breakfast\",\"close\"],\"captions\":[{\"text\":\"a group of small cups with brown liquid in them\",\"confidence\":0.39556050300598145}]}",
        "{\"tags\":[\"person\",\"music\",\"guitar\",\"bowed instrument\",\"bass\"],\"captions\":[{\"text\":\"a person playing a guitar\",\"confidence\":0.54444891214370728}]}"
      ]
    },
    {
      "@search.score": 0.18232156,
      "content": "\nReview: I often make Fourth Coffee my meeting spot for my client meetings weekday mornings. I own a small business and the folks who work at Fourth Coffee are always very friendly. It leaves a good impression on my clients. There are also plenty of drink selections, good wi-fi, and seating. Some of my favorite coffees are the lavender honey latte and, in the winter, the apple-chai latte. There are delicious baked goods offered as well. \nDate: October 21, 2018\nLocation: Chicago, Illinois \n\nimage1.png\n\n\n\n",
      "metadata_storage_path": "aHR0cHM6Ly9zdG9hZ2VpYWNvbnQuYmxvYi5jb3JlLndpbmRvd3MubmV0L2NvZmZlZXJldmlld3MvcmV2aWV3LTUuZG9jeA2",
      "locations": [
        "meeting spot",
        "Chicago",
        "Illinois"
      ],
      "keyphrases": [
        "delicious baked goods",
        "lavender honey latte",
        "apple-chai latte",
        "Fourth Coffee",
        "meeting spot",
        "client meetings",
        "small business",
        "good impression",
        "drink selections",
        "good wi",
        "favorite coffees",
        "Review",
        "mornings",
        "folks",
        "clients",
        "plenty",
        "fi",
        "seating",
        "winter",
        "Date",
        "October",
        "Location",
        "Chicago",
        "Illinois"
      ],
      "sentiment": "[\"positive\"]",
      "merged_content": "\nReview: I often make Fourth Coffee my meeting spot for my client meetings weekday mornings. I own a small business and the folks who work at Fourth Coffee are always very friendly. It leaves a good impression on my clients. There are also plenty of drink selections, good wi-fi, and seating. Some of my favorite coffees are the lavender honey latte and, in the winter, the apple-chai latte. There are delicious baked goods offered as well. \nDate: October 21, 2018\nLocation: Chicago, Illinois \n\nimage1.png\n  \n\n\n",
      "text": [
        ""
      ],
      "layoutText": [
        "{\"language\":\"en\",\"text\":\"\",\"lines\":[],\"words\":[]}"
      ],
      "imageTags": [
        "clothing",
        "person",
        "furniture",
        "human face",
        "chair",
        "table",
        "woman",
        "indoor",
        "window",
        "desk",
        "sitting",
        "people",
        "restaurant"
      ],
      "imageCaption": [
        "{\"tags\":[\"person\",\"woman\",\"laptop\",\"dish\"],\"captions\":[{\"text\":\"a woman showing a woman something on a tablet\",\"confidence\":0.513512134552002}]}"
      ]
    },
    {
      "@search.score": 0.18232156,
      "content": "\n\n\nReview: My favorite part about going to Fourth Coffee is the atmosphere. I love the warm lights and plants. It’s a great place to go get a cup of coffee while working on your next business idea or with friends at school. It’s also right next to the University hub, which makes it so easy to access for students. It just gets so busy on the weekends! I wish it was not so crowded. Since they started offering amazing breakfast sandwiches, I wouldn’t try to go get a coffee Saturday morning.  \nDate: September 1, 2018\nLocation: Los Angeles, California \nimage1.png\n\n\n\nimage2.png\n\n\n\n",
      "metadata_storage_path": "aHR0cHM6Ly9zdG9hZ2VpYWNvbnQuYmxvYi5jb3JlLndpbmRvd3MubmV0L2NvZmZlZXJldmlld3MvcmV2aWV3LTIuZG9jeA2",
      "locations": [
        "school",
        "University hub",
        "Los Angeles",
        "California"
      ],
      "keyphrases": [
        "next business idea",
        "amazing breakfast sandwiches",
        "favorite part",
        "warm lights",
        "great place",
        "University hub",
        "Los Angeles",
        "Fourth Coffee",
        "Review",
        "atmosphere",
        "plants",
        "cup",
        "friends",
        "school",
        "students",
        "weekends",
        "Date",
        "September",
        "Location",
        "California"
      ],
      "sentiment": "[\"positive\"]",
      "merged_content": "\n\n\nReview: My favorite part about going to Fourth Coffee is the atmosphere. I love the warm lights and plants. It’s a great place to go get a cup of coffee while working on your next business idea or with friends at school. It’s also right next to the University hub, which makes it so easy to access for students. It just gets so busy on the weekends! I wish it was not so crowded. Since they started offering amazing breakfast sandwiches, I wouldn’t try to go get a coffee Saturday morning.  \nDate: September 1, 2018\nLocation: Los Angeles, California \nimage1.png\n  \n\n\nimage2.png\n T \n\n\n",
      "text": [
        "",
        "T"
      ],
      "layoutText": [
        "{\"language\":\"en\",\"text\":\"\",\"lines\":[],\"words\":[]}",
        "{\"language\":\"en\",\"text\":\"T\",\"lines\":[{\"boundingBox\":[{\"x\":809,\"y\":32},{\"x\":837,\"y\":31},{\"x\":836,\"y\":56},{\"x\":808,\"y\":55}],\"text\":\"T\"}],\"words\":[{\"boundingBox\":[{\"x\":815,\"y\":31},{\"x\":831,\"y\":31},{\"x\":831,\"y\":56},{\"x\":815,\"y\":56}],\"text\":\"T\"}]}"
      ],
      "imageTags": [
        "wall",
        "indoor",
        "furniture",
        "clothing",
        "interior design",
        "person",
        "kitchen & dining room table",
        "countertop",
        "desk",
        "ceiling",
        "stool",
        "coffee table",
        "floor",
        "woman",
        "window",
        "table",
        "kitchen",
        "chair",
        "room",
        "cafe",
        "furniture",
        "indoor",
        "interior design",
        "houseplant",
        "wall",
        "house",
        "floor",
        "coffee table",
        "musical instrument",
        "table",
        "chair",
        "flooring",
        "clothing",
        "musical keyboard",
        "couch",
        "studio couch",
        "person",
        "room",
        "plant",
        "piano",
        "ceiling",
        "home"
      ],
      "imageCaption": [
        "{\"tags\":[\"indoor\",\"wall\",\"floor\",\"ceiling\"],\"captions\":[{\"text\":\"a person sitting at a table\",\"confidence\":0.53540337085723877}]}",
        "{\"tags\":[\"floor\",\"indoor\",\"living\",\"room\",\"plant\",\"furniture\",\"dining table\"],\"captions\":[{\"text\":\"a person sitting in a chair\",\"confidence\":0.43682509660720825}]}"
      ]
    },
    {
      "@search.score": 0.18232156,
      "content": "Review: I heard that Fourth Coffee had the best seasonal donuts, so I ordered a dozen for my team for an event. Everyone loved them, I’ll definitely order again! \nDate: October 25, 2018\nLocation: Seattle, Washington \n\n",
      "metadata_storage_path": "aHR0cHM6Ly9zdG9hZ2VpYWNvbnQuYmxvYi5jb3JlLndpbmRvd3MubmV0L2NvZmZlZXJldmlld3MvcmV2aWV3LTkuZG9jeA2",
      "locations": [
        "Seattle",
        "Washington"
      ],
      "keyphrases": [
        "best seasonal donuts",
        "Fourth Coffee",
        "Review",
        "dozen",
        "team",
        "event",
        "Everyone",
        "Date",
        "October",
        "Location",
        "Seattle",
        "Washington"
      ],
      "sentiment": "[\"positive\"]",
      "merged_content": "Review: I heard that Fourth Coffee had the best seasonal donuts, so I ordered a dozen for my team for an event. Everyone loved them, I’ll definitely order again! \nDate: October 25, 2018\nLocation: Seattle, Washington \n\n",
      "text": [],
      "layoutText": [],
      "imageTags": [],
      "imageCaption": []
    }
  ]
}
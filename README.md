<p align='center'><b><h1 align='center'>Helakuru-Esana-API(Unofficial)🇱🇰</h1></b></p>
<p align="center">
  <a href="https://t.me/HelakuruNewsLK">
        <img src="https://cdn.taprobyte.com/file/9659b5e014f6f41c02b98.jpg" alt="sdbots" width="440">
    </a>
    <br>
    <b>Nation's News Breaker🇱🇰</b>
    <br>
    <b>•<a href="https://t.me/HelakuruNewsLK">Channel</a>•</b>
</p>

## API Documentation 🚀

### Base URL
```
https://esana-api.vercel.app/
```

---

## Endpoints ✨

### 1. **Get Latest News**

Retrieve the latest news articles, including titles, content, likes, reactions, and links to the full articles.

**URL**:  
```
GET /EsanaV3
```

**Method**: `GET`

**Response**:  
- Returns an object containing a list of posts and a status object.

**Sample Response**:
```json
{
  "Posts": [
    {
      "comments": 4,
      "content": [
        {
          "data": "පාර්ලිමේන්තු මන්ත්‍රී වෛද්‍ය රාමනාතන් අර්චුනාට...",
          "data_en": "Colombo Additional Magistrate Manjula Ratnayake has..."
        },
        ...
      ],
      "id": 106432,
      "likes": 5,
      "link": "https://www.helakuru.lk/esana/news/106432",
      "published": "2024-11-26 11:31:46",
      "reactionList": [
        { "count": 1, "id": 1, "text": "like" },
        { "count": 2, "id": 3, "text": "haha" }
      ],
      "thumb": "https://helakuru.sgp1.cdn.digitaloceanspaces.com/esana/images/lib/archchuna-ramanathan-tt.jpg",
      "title": "පාර්ලිමේන්තු මන්ත්‍රී රාමනාතන්...",
      "title_en": "Warrants will be issued to MP Ramanathan Archuna"
    }
  ],
  "Status": {
    "code": 200,
    "description": "Action Successful ",
    "success": true
  }
}
```

---

### 2. **Get News by ID**

Retrieve details of a specific news article by its ID.

**URL**:  
```
GET /EsanaV3/GetNewsById?id=<news-id>
```

**Method**: `GET`

**Query Parameters**:
| Parameter | Type   | Description                |
|-----------|--------|----------------------------|
| `id`      | string | Unique ID of the news item |

**Response**:  
- Returns an object containing the details of the specific news post, including its content, likes, and reactions.

**Sample Response**:
```json
{
  "Posts": [
    {
      "comments": 0,
      "content": [
        {
          "data": "ගෑස් හිඟයට ඉදිරි දින කිහිපයේ...",
          "data_en": "The president of Laugh company W. K. H Wegapitiya..."
        },
        ...
      ],
      "id": 106428,
      "likes": 0,
      "link": "https://www.helakuru.lk/esana/news/106428",
      "published": "2024-11-26 09:38:26",
      "reactionList": [
        { "count": 0, "id": 1, "text": "like" },
        { "count": 0, "id": 4, "text": "wow" }
      ],
      "thumb": "https://helakuru.sgp1.cdn.digitaloceanspaces.com/esana/images/lib/laugfs-gas[1].jpg",
      "title": "ගෑස් හිඟයට කඩිනමින්...",
      "title_en": "Fast Solutions to Gas Shortage - Laugh Company"
    }
  ],
  "Status": {
    "code": 200,
    "description": "Action Successful-",
    "success": true
  },
  "refresh": 100
}
```

## ⚡️ Support
If you found this project helpful, don't forget to give it a Star⭐ on GitHub. This helps others find and use the project too! ❤️

  - Developer: [@Damantha126](https://github.com/Damantha126)

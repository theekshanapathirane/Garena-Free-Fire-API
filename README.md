# 📝 API Documentation

##  Account Information API
API Route = https://www.public.freefireinfo.site/api/info/{region}/{uid}?key={key}

**Endpoint:** `api/info`
**key:** `astute_ff`
**Method:** `GET`  

This Endpoint Retrieves Account Information based on the Specified Region and User ID.

### 📨 Request Example
```http
GET https://www.public.freefireinfo.site/api/info/sg/1341742864?key=astute_ff
```

### ☑️ Query Parameters

| Parameter | Type   | Required | Description                   |
|-----------|--------|----------|-------------------------------|
| `region`  | string | Yes      | The region code (`sg`, `ind`, `br`,`id`, `tw`, `us`, `sac`, `th`, `me`, `pk`, `cis`, `bd`).|
| `uid`     | int | Yes      | The user ID.                  |
| `key`     | string | Yes      | Join https://t.me/FreeFireInfoSite to get Latest Key.                  |


📚 **Purpose of the API**  

The primary purpose of providing this free API is to enhance the Free Fire community experience. Garena Free Fire does not offer official account information APIs, so this custom solution aims to fill that gap, providing players and developers with valuable account data


🧩 **(Some of🤫) Frameworks and Libraries Used**  
- **Flask**: A micro web framework for Python to build the API endpoints.
- **Flask-CORS**: For handling Cross-Origin Resource Sharing (CORS).
- **PyCryptodome**: For implementing Decryption and Encryption.
- **Requests**: For making HTTP Requests to Server.

# 📁 Additional Information

- This API response Does not Represent the Actual Structure Received from the Official Garena Server.
- The Response structure is simplified in an User-Friendly Structure for the ease of understanding for Anyone at any level of Programming.
- All images related to item IDs shown by the API response (e.g., avatars, banners, outfits, weapons) are available at `https://www.library.freefireinfo.site/icons/{item_code}.png` for the convenience of API users in their development projects.


### 💬 Example of a Successful Reponse May Look Like this,
```json
{
  "Account Avatar Image": "https://library.freefireinfo.site/icons/902044006.png",
  "Account Banner Image": "https://library.freefireinfo.site/icons/901043009.png",
  "Account Booyah Pass": "Premium",
  "Account Booyah Pass Badges": 44,
  "Account Create Time (GMT 0530)": "2019-08-24 15:05:19",
  "Account Evo Access Badge": "Inactive",
  "Account Honor Score": 100,
  "Account Language": "Language_EN",
  "Account Last Login (GMT 0530)": "2024-06-11 14:11:54",
  "Account Level": 69,
  "Account Likes": 22540,
  "Account Name": "FFLKㅤASTUTE",
  "Account Region": "SG",
  "Account Signature": "[c][b]TikTok : @astute_ff\nLEAD Team FFLK",
  "Account UID": "1341742864",
  "Account XP": 2756151,
  "BR Rank Points": 3222,
  "CS Rank Points": 59,
  "Equipped Items": {
    "profile": {
      "Clothes": [
        "https://library.freefireinfo.site/icons/203040003.png",
        "https://library.freefireinfo.site/icons/211044002.png",
        "https://library.freefireinfo.site/icons/204034043.png",
        "https://library.freefireinfo.site/icons/205033044.png",
        "https://library.freefireinfo.site/icons/211044041.png",
        "https://library.freefireinfo.site/icons/214000082.png"
      ],
      "Equipped Skills": [16, 5306, 8, 1, 16, 2706, 8, 2, 16, 22016, 8, 3, 16, 5706],
      "External Items": [
        {
          "Category": "Weapon Skin",
          "Image URL": "https://library.freefireinfo.site/icons/907104110.png",
          "Item ID": 907104110
        },
        {
          "Category": "Animation Skin",
          "Image URL": "https://library.freefireinfo.site/icons/912041001.png",
          "Item ID": 912041001
        },
        {
          "Category": "Transformation Skin",
          "Image URL": "https://library.freefireinfo.site/icons/914000002.png",
          "Item ID": 914000002
        }
      ]
    }
  },
  "Equipped Pet Information": {
    "Pet Level": 7,
    "Pet Name": "FFLK",
    "Pet Type": "Baboon",
    "Pet XP": 6004,
    "Selected?": true
  },
  "Equipped Title": "Boom Artist",
  "Guild Information": {
    "Guild Capacity": 20,
    "Guild Current Members": 15,
    "Guild ID": "3052792498",
    "Guild Level": 1,
    "Guild Name": "FFLKㅤMASTERS",
    "Leader ID": "1341742864"
  },
  "Guild Leader Information": {
    "Leader Ac Created Time (GMT 0530)": "2019-08-24 15:05:19",
    "Leader Animations": [907104110, 912041001, 914000002],
    "Leader Avatar Image": "https://library.freefireinfo.site/icons/902044006.png",
    "Leader BP Badges": 44,
    "Leader BR Points": 3222,
    "Leader Banner Image": "https://library.freefireinfo.site/icons/901043009.png",
    "Leader CS Points": 59,
    "Leader Last Login Time (GMT 0530)": "2024-06-11 14:11:54",
    "Leader Level": 69,
    "Leader Likes": 22540,
    "Leader Name": "FFLKㅤASTUTE",
    "Leader Pin": 910000010,
    "Leader Title": "Boom Artist",
    "Leader UID": "1341742864",
    "Leader XP": 2756151
  },
  "Public Craftland Maps": {
    "Map Codes": "{#FREEFIRE31BD4345E87C6A7C0A476B7343B5CD0B2864}"
  }
}

```
# 😵 Error Responses
API might Show Error Response Upon Users' Inaccurate Requests!

### Error Instances and Solutions

- **Error Code:** 400
  - **Message:** Invalid region.
  - **Solution:** Make sure you are using a valid region code.

- **Error Code:** 429
  - **Message:** Abnormal Requests Detected. Please Avoid Misusing Info API for Visits or Your IP may get Blocked!
  - **Solution:** Avoid excessive requests or contact the API provider for assistance.

- **Error Code:** 500
  - **Message:** An error occurred while processing your request. Please Recheck Your ID & Region.
  - **Solution:** Double-check the provided user ID and region, and retry the request. If the issue persists, contact the API provider for support.

---

API Made By Theekshana(ASTUTE),
All Rights Reserved!

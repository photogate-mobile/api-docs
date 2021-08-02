# GET /api/v1/config
Returns PhotoPrism configuration.

Useful links:
- [API handler implementation](https://github.com/photoprism/photoprism/blob/5076af297963/internal/api/config.go#L18)


# Example
Request: `/api/v1/config`
- `X-Session-Id` header

### Response
<details>
  <summary>Headers</summary>

  <br/>

  | Name              | Value                           |
  | ----------------- | ------------------------------- |
  | Content-Type      | application/json; charset=utf-8 |
  | Date              | Mon, 02 Aug 2021 15:13:12 GMT   |
  | Transfer-Encoding | chunked                         |
</details>  

<details>
  <summary>JSON</summary>

  <br/>

```json
  {
    "mode": "user",
    "name": "PhotoPrism",
    "version": "210523-b1856b9d-Linux-x86_64",
    "copyright": "(c) 2018-2021 Michael Mayer <hello@photoprism.org>",
    "flags": "settings",
    "siteUrl": "http://localhost:2342/",
    "sitePreview": "http://localhost:2342/static/img/preview.jpg",
    "siteTitle": "PhotoPrism",
    "siteCaption": "Browse Your Life",
    "siteDescription": "",
    "siteAuthor": "",
    "debug": false,
    "test": false,
    "demo": false,
    "sponsor": false,
    "readonly": false,
    "uploadNSFW": true,
    "public": false,
    "experimental": false,
    "albumCategories": null,
    "albums": [],
    "cameras": [
      {
        "ID": 6,
        "Slug": "apple-iphone-4s",
        "Name": "Apple iPhone 4S",
        "Make": "Apple",
        "Model": "iPhone 4S"
      },
      {
        "ID": 7,
        "Slug": "apple-iphone-5s",
        "Name": "Apple iPhone 5s",
        "Make": "Apple",
        "Model": "iPhone 5s"
      },
      {
        "ID": 8,
        "Slug": "apple-iphone-6",
        "Name": "Apple iPhone 6",
        "Make": "Apple",
        "Model": "iPhone 6"
      },
      {
        "ID": 9,
        "Slug": "apple-iphone-se",
        "Name": "Apple iPhone SE",
        "Make": "Apple",
        "Model": "iPhone SE"
      },
      {
        "ID": 3,
        "Slug": "canon-eos-5d",
        "Name": "Canon EOS 5D",
        "Make": "Canon",
        "Model": "EOS 5D"
      },
      {
        "ID": 5,
        "Slug": "canon-eos-6d",
        "Name": "Canon EOS 6D",
        "Make": "Canon",
        "Model": "EOS 6D"
      },
      {
        "ID": 4,
        "Slug": "canon-eos-7d",
        "Name": "Canon EOS 7D",
        "Make": "Canon",
        "Model": "EOS 7D"
      },
      {
        "ID": 10,
        "Slug": "huawei-p30",
        "Name": "HUAWEI P30",
        "Make": "HUAWEI",
        "Model": "P30"
      },
      {
        "ID": 2,
        "Slug": "olympus-c2500l",
        "Name": "Olympus C2500L",
        "Make": "Olympus",
        "Model": "C2500L"
      },
      {
        "ID": 1,
        "Slug": "zz",
        "Name": "Unknown",
        "Make": "",
        "Model": "Unknown"
      }
    ],
    "lenses": [
      {
        "ID": 6,
        "Slug": "100-0-mm",
        "Name": "100.0 mm",
        "Make": "",
        "Model": "100.0 mm",
        "Type": ""
      },
      {
        "ID": 2,
        "Slug": "24-0-105-0-mm",
        "Name": "24.0 - 105.0 mm",
        "Make": "",
        "Model": "24.0 - 105.0 mm",
        "Type": ""
      },
      {
        "ID": 8,
        "Slug": "apple-iphone-5s-back-camera-4-12mm-f-2-2",
        "Name": "Apple iPhone 5s back camera 4.12mm f/2.2",
        "Make": "Apple",
        "Model": "iPhone 5s back camera 4.12mm f/2.2",
        "Type": ""
      },
      {
        "ID": 10,
        "Slug": "apple-iphone-6-back-camera-4-15mm-f-2-2",
        "Name": "Apple iPhone 6 back camera 4.15mm f/2.2",
        "Make": "Apple",
        "Model": "iPhone 6 back camera 4.15mm f/2.2",
        "Type": ""
      },
      {
        "ID": 11,
        "Slug": "apple-iphone-se-back-camera-4-15mm-f-2-2",
        "Name": "Apple iPhone SE back camera 4.15mm f/2.2",
        "Make": "Apple",
        "Model": "iPhone SE back camera 4.15mm f/2.2",
        "Type": ""
      },
      {
        "ID": 5,
        "Slug": "ef100mm-f-2-8l-macro-is-usm",
        "Name": "EF100mm f/2.8L Macro IS USM",
        "Make": "",
        "Model": "EF100mm f/2.8L Macro IS USM",
        "Type": ""
      },
      {
        "ID": 7,
        "Slug": "ef16-35mm-f-2-8l-ii-usm",
        "Name": "EF16-35mm f/2.8L II USM",
        "Make": "",
        "Model": "EF16-35mm f/2.8L II USM",
        "Type": ""
      },
      {
        "ID": 3,
        "Slug": "ef24-105mm-f-4l-is-usm",
        "Name": "EF24-105mm f/4L IS USM",
        "Make": "",
        "Model": "EF24-105mm f/4L IS USM",
        "Type": ""
      },
      {
        "ID": 9,
        "Slug": "ef35mm-f-2-is-usm",
        "Name": "EF35mm f/2 IS USM",
        "Make": "",
        "Model": "EF35mm f/2 IS USM",
        "Type": ""
      },
      {
        "ID": 4,
        "Slug": "ef70-200mm-f-4l-is-usm",
        "Name": "EF70-200mm f/4L IS USM",
        "Make": "",
        "Model": "EF70-200mm f/4L IS USM",
        "Type": ""
      },
      {
        "ID": 1,
        "Slug": "zz",
        "Name": "Unknown",
        "Make": "",
        "Model": "Unknown",
        "Type": ""
      }
    ],
    "countries": [
      {
        "ID": "at",
        "Slug": "austria",
        "Name": "Austria"
      },
      {
        "ID": "bw",
        "Slug": "botswana",
        "Name": "Botswana"
      },
      {
        "ID": "ca",
        "Slug": "canada",
        "Name": "Canada"
      },
      {
        "ID": "cu",
        "Slug": "cuba",
        "Name": "Cuba"
      },
      {
        "ID": "fr",
        "Slug": "france",
        "Name": "France"
      },
      {
        "ID": "de",
        "Slug": "germany",
        "Name": "Germany"
      },
      {
        "ID": "gr",
        "Slug": "greece",
        "Name": "Greece"
      },
      {
        "ID": "it",
        "Slug": "italy",
        "Name": "Italy"
      },
      {
        "ID": "za",
        "Slug": "south-africa",
        "Name": "South Africa"
      },
      {
        "ID": "ch",
        "Slug": "switzerland",
        "Name": "Switzerland"
      },
      {
        "ID": "gb",
        "Slug": "united-kingdom",
        "Name": "United Kingdom"
      },
      {
        "ID": "us",
        "Slug": "usa",
        "Name": "USA"
      },
      {
        "ID": "zz",
        "Slug": "zz",
        "Name": "Unknown"
      }
    ],
    "thumbs": [
      {
        "size": "fit_720",
        "use": "Mobile, TV",
        "w": 720,
        "h": 720
      },
      {
        "size": "fit_1280",
        "use": "Mobile, HD Ready TV",
        "w": 1280,
        "h": 1024
      },
      {
        "size": "fit_1920",
        "use": "Mobile, Full HD TV",
        "w": 1920,
        "h": 1200
      },
      {
        "size": "fit_2048",
        "use": "Tablets, Cinema 2K",
        "w": 2048,
        "h": 2048
      },
      {
        "size": "fit_2560",
        "use": "Quad HD, Retina Display",
        "w": 2560,
        "h": 1600
      },
      {
        "size": "fit_4096",
        "use": "Ultra HD, Retina 4K",
        "w": 4096,
        "h": 4096
      },
      {
        "size": "fit_7680",
        "use": "8K Ultra HD 2, Retina 6K",
        "w": 7680,
        "h": 4320
      }
    ],
    "status": "unregistered",
    "mapKey": "D9ve6edlcVR2mEsNvCVs",
    "downloadToken": "bupvwse1",
    "previewToken": "2e78f2ac",
    "jsHash": "911ffd54",
    "cssHash": "7a2bb49d",
    "manifestHash": "e7095a4c",
    "settings": {
      "ui": {
        "scrollbar": true,
        "zoom": false,
        "theme": "default",
        "language": "en"
      },
      "templates": {
        "default": "index.tmpl"
      },
      "maps": {
        "animate": 0,
        "style": "streets"
      },
      "features": {
        "upload": true,
        "download": true,
        "private": true,
        "review": true,
        "files": true,
        "videos": true,
        "folders": true,
        "albums": true,
        "moments": true,
        "estimates": true,
        "people": true,
        "labels": true,
        "places": true,
        "edit": true,
        "archive": true,
        "delete": false,
        "share": true,
        "library": true,
        "import": true,
        "logs": true
      },
      "import": {
        "path": "/",
        "move": false
      },
      "index": {
        "path": "/",
        "convert": true,
        "rescan": false
      },
      "stack": {
        "uuid": true,
        "meta": true,
        "name": false
      },
      "share": {
        "title": ""
      },
      "download": {
        "name": "file"
      }
    },
    "disable": {
      "backups": false,
      "webdav": false,
      "settings": false,
      "places": false,
      "exiftool": false,
      "darktable": false,
      "rawtherapee": false,
      "sips": true,
      "heifconvert": false,
      "ffmpeg": false,
      "tensorflow": false
    },
    "count": {
      "all": 104,
      "photos": 102,
      "videos": 2,
      "cameras": 9,
      "lenses": 10,
      "countries": 12,
      "hidden": 0,
      "favorites": 0,
      "private": 0,
      "review": 2,
      "stories": 0,
      "albums": 0,
      "moments": 7,
      "months": 41,
      "folders": 2,
      "files": 114,
      "places": 39,
      "states": 16,
      "labels": 37,
      "labelMaxPhotos": 10
    },
    "pos": {
      "uid": "pqx6gkxpkfnnbxe1",
      "cid": "s2:47a85a624184",
      "utc": "2020-08-31T16:03:10Z",
      "lat": 52.4525,
      "lng": 13.3092
    },
    "years": [
      2021,
      2020,
      2019,
      2018,
      2017,
      2016,
      2015,
      2014,
      2013,
      2012,
      2011,
      2010,
      2002
    ],
    "colors": [
      {
        "Example": "#AB47BC",
        "Name": "Purple",
        "Slug": "purple"
      },
      {
        "Example": "#FF00FF",
        "Name": "Magenta",
        "Slug": "magenta"
      },
      {
        "Example": "#EC407A",
        "Name": "Pink",
        "Slug": "pink"
      },
      {
        "Example": "#EF5350",
        "Name": "Red",
        "Slug": "red"
      },
      {
        "Example": "#FFA726",
        "Name": "Orange",
        "Slug": "orange"
      },
      {
        "Example": "#D4AF37",
        "Name": "Gold",
        "Slug": "gold"
      },
      {
        "Example": "#FDD835",
        "Name": "Yellow",
        "Slug": "yellow"
      },
      {
        "Example": "#CDDC39",
        "Name": "Lime",
        "Slug": "lime"
      },
      {
        "Example": "#66BB6A",
        "Name": "Green",
        "Slug": "green"
      },
      {
        "Example": "#009688",
        "Name": "Teal",
        "Slug": "teal"
      },
      {
        "Example": "#00BCD4",
        "Name": "Cyan",
        "Slug": "cyan"
      },
      {
        "Example": "#2196F3",
        "Name": "Blue",
        "Slug": "blue"
      },
      {
        "Example": "#A1887F",
        "Name": "Brown",
        "Slug": "brown"
      },
      {
        "Example": "#F5F5F5",
        "Name": "White",
        "Slug": "white"
      },
      {
        "Example": "#9E9E9E",
        "Name": "Grey",
        "Slug": "grey"
      },
      {
        "Example": "#212121",
        "Name": "Black",
        "Slug": "black"
      }
    ],
    "categories": [
      {
        "UID": "lqx6geqlhg1x3t60",
        "Slug": "animal",
        "Name": "Animal"
      },
      {
        "UID": "lqx6gi52m1409jqz",
        "Slug": "architecture",
        "Name": "Architecture"
      },
      {
        "UID": "lqx6gkj2syby8vcc",
        "Slug": "beach",
        "Name": "Beach"
      },
      {
        "UID": "lqx6ggh3deewkz3a",
        "Slug": "beetle",
        "Name": "Beetle"
      },
      {
        "UID": "lqx6gfc2ntxizgmh",
        "Slug": "bird",
        "Name": "Bird"
      },
      {
        "UID": "lqx6getbckaa8fqv",
        "Slug": "building",
        "Name": "Building"
      },
      {
        "UID": "lqx6gef2teck91ov",
        "Slug": "car",
        "Name": "Car"
      },
      {
        "UID": "lqx6gf82dp687lar",
        "Slug": "cat",
        "Name": "Cat"
      },
      {
        "UID": "lqx6gh02r57gola5",
        "Slug": "farm",
        "Name": "Farm"
      },
      {
        "UID": "lqx6gl638h4769yq",
        "Slug": "food",
        "Name": "Food"
      },
      {
        "UID": "lqx6gf11zfyrlpxm",
        "Slug": "insect",
        "Name": "Insect"
      },
      {
        "UID": "lqx6geo1yqat7ao4",
        "Slug": "landscape",
        "Name": "Landscape"
      },
      {
        "UID": "lqx6gha19okjyxwj",
        "Slug": "monkey",
        "Name": "Monkey"
      },
      {
        "UID": "lqx6geoovvzbev9g",
        "Slug": "mountain",
        "Name": "Mountain"
      },
      {
        "UID": "lqx6gef10c04xid6",
        "Slug": "nature",
        "Name": "Nature"
      },
      {
        "UID": "lqx6gef17qtbrhlh",
        "Slug": "plant",
        "Name": "Plant"
      },
      {
        "UID": "lqx6gir1qmdszai3",
        "Slug": "reptile",
        "Name": "Reptile"
      },
      {
        "UID": "lqx6gei37yntqbjs",
        "Slug": "shop",
        "Name": "Shop"
      },
      {
        "UID": "lqx6ghhn570qow7j",
        "Slug": "snow",
        "Name": "Snow"
      },
      {
        "UID": "lqx6gi51dmgbqpgq",
        "Slug": "tower",
        "Name": "Tower"
      },
      {
        "UID": "lqx6gef3h1z1ng51",
        "Slug": "vehicle",
        "Name": "Vehicle"
      },
      {
        "UID": "lqx6gig1n5pi0epy",
        "Slug": "water",
        "Name": "Water"
      },
      {
        "UID": "lqx6gga2d6hk5462",
        "Slug": "wildlife",
        "Name": "Wildlife"
      }
    ],
    "clip": 160,
    "server": {
      "cores": 8,
      "routines": 25,
      "memory": {
        "used": 35293344,
        "reserved": 147345432,
        "info": "Used 35 MB / Reserved 147 MB"
      }
    }
  }
```
</details>  
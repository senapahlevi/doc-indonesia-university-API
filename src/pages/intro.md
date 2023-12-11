---
sidebar_position: 1
---

# Indonesia University API

<!-- Let's discover **Docusaurus in less than 5 minutes**. -->

## Getting Started

Indonesia University API is build to show All List Indonesia University you can contribute using `.csv` files to updated all data in [here](https://github.com/senapahlevi/doc-indonesia-university-API)

## Installation

- [Golang](https://nodejs.org/en/download/) using versino 1.8 and using framework :
  - [Gorm](https://nodejs.org/en/download/) version 18.0 or above:
  - [Gin](https://nodejs.org/en/download/) version 18.0 or above:
- [MySQL](https://nodejs.org/en/download/) version 18.0 or above:

Updated by **2024**.

Clone to your project Golang

```bash
git clone https://github.com/senapahlevi/doc-indonesia-university-API
```

setting `.env`
connect database

```bash
DB_USERNAME=
DB_PASSWORD=
DB_HOST=
DB_PORT=
DB_NAME=
PORT=
```

download all library and framework golang to your local

```bash
go get -u
```

running golang project from terminal

```bash
go run main.go
```

as you can see project from `main.go` is execute

The `go run main.go` command run your project locally and serves ready for you to view at your port example if youre using `PORT=8080` you will running using `http://localhost:8080/`

## API

**Get**

```bash
http://localhost:8080/api/campus?CampusName=Telkom
```

```
{
      "data": [
          {
              "campus_id": 1,
              "name": "Telkom University",
              "address": "Jl. Telekomunikasi Terusan Buah Batu Indonesia 40257, Bandung, Indonesia",
              "provinces": [
                  {
                      "province_id": 12,
                      "name": "Jawa Barat"
                  }
              ]
          },
          {
              "campus_id": 2,
              "name": "Telkom University",
              "address": "Jalan Halimun Raya No.2, RT.15/RW.6, Guntur, Kecamatan Setiabudi, Kota Jakarta Selatan, DKI Jakarta 12980",
              "provinces": [
                  {
                      "province_id": 11,
                      "name": "DKI Jakarta"
                  }
              ]
          },
          {
              "campus_id": 3,
              "name": "Telkom University",
              "address": "Jalan Raya Daan Mogot KM.11, RT.1/RW.4, Kedaung Kali Angke, Cengkareng, Kota Jakarta Barat, DKI Jakarta 11710",
              "provinces": [
                  {
                      "province_id": 11,
                      "name": "DKI Jakarta"
                  }
              ]
          }
      ]
  }
``` 



**Get Detail ID**

```bash
http://localhost:8080/api/campus/1
```

and `json` result is

```
{
    "data": {
        "campus_id": 1,
        "name": "Telkom University",
        "address": "Jl. Telekomunikasi Terusan Buah Batu Indonesia 40257, Bandung, Indonesia",
        "provinces": [
            {
                "province_id": 12,
                "name": "Jawa Barat"
            }
        ]
    }
}
```

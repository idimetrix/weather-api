# weather-api

[![License](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square)](/LICENSE)
[![Build Status](https://travis-ci.org/idimetrix/weather-api.svg?branch=master)](https://travis-ci.org/idimetrix/weather-api)
[![Go Report Card](https://goreportcard.com/badge/github.com/idimetrix/weather-api)](https://goreportcard.com/report/github.com/idimetrix/weather-api)
[![GoDoc](https://godoc.org/github.com/idimetrix/weather-api?status.svg)](https://godoc.org/github.com/idimetrix/weather-api)

> A REST API to check the current weather.

> https://weather-restful.herokuapp.com/weather/Singapore
https://weather-restful.herokuapp.com/weather/{city}

## Install
```sh
dep ensure
```
## Build
```sh
go build
```
## Run
```sh
./weather-api
```
## Usage
```sh
curl http://localhost:3000/weather/{city}
```
## Example
#### Request
```sh
curl http://localhost:3000/weather/Singapore
```
#### Response
```json
{
  "temperature": "+28 °C",
  "wind": "11 km/h",
  "description": "Partly cloudy",
  "forecast": [
    {
      "day": "1",
      "temperature": "+30 °C",
      "wind": "13 km/h"
    },
    {
      "day": "2",
      "temperature": "32 °C",
      "wind": "5 km/h"
    },
    {
      "day": "3",
      "temperature": " °C",
      "wind": "11 km/h"
    }
  ]
}
```

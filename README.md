
# Building Services with ASP.NET Web API

## Fitness Frog Client App

## Supported User Actions

* Viewing a list of entries
* Adding an entry
* Editing an entry
* Deleting an entry

## Endpoints

* /api/entries GET, POST
* /api/entries/1 GET, PUT, DELETE
* /api/activities GET
* /api/intensities GET

## HTTP Status Codes

* 200 OK
* 201 Created 
* 204 No Content
* 400 Bad Request
* 500 Internal Server Error

- Nuget > Microsoft.AspNet.WebApi
- Route default is in Treehouse.FitnessFrog.Spa > WebApiConfig.cs
- Soap UI > GET > 
	- http://localhost:51487/api/entries
	- http://localhost:51487/api/entries/1
	- HEADER = application/json
	- HEADER = application/xml

- http://localhost:51487/api/entries
	- raw / json / post
```json
{
  "date": "1/1/2017",
  "activityId": 1,
  "duration": 4.5,
  "intensity": 1,
  "exclude": false,
  "notes": null
}
```
- `[HttpGet]` = http method attributes  vs. http method names `Get()` for EntriesController.cs, and may use `GetEntries()`
- Nuget > simpleinjector.integration.webapi.webhost.quickstart


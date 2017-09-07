---
layout: article
title:  "Create a Glove Using BoxList"
categories: guides
modified: 2017-09-05
image:
  teaser: glove-issue-list.jpg
share: true
comments: true
ads: false
---

Vestibulum ultricies erat ut urna congue, id blandit velit eleifend. Proin hendrerit, orci rhoncus vestibulum bibendum, justo nisi sodales felis, eu gravida mi purus et sapien.
{% include toc.html %}

## About BoxList

Vestibulum ultricies erat ut urna congue, id blandit velit eleifend. Proin hendrerit, orci rhoncus vestibulum bibendum, justo nisi sodales felis, eu gravida mi purus et sapien. Cras fringilla molestie nibh, non auctor orci vehicula quis. Nam luctus magna sed lorem interdum elementum. Mauris finibus mi sit amet leo pharetra consequat. Nunc neque lacus, aliquet vel risus ac, gravida malesuada ipsum. Quisque aliquam ante vel luctus placerat.

![BoxList](http://placehold.it/900x450.gif "BoxList")

### List 1

Duis non dignissim elit, quis pretium risus. Vestibulum maximus tincidunt ex sit amet fringilla. Nam lacinia elit nec massa venenatis pellentesque. Donec nec urna sollicitudin, lacinia magna quis, volutpat felis. Duis a tellus sit amet sapien tristique rhoncus. Vivamus semper quis arcu nec feugiat. Nulla vitae elit nisi. In sit amet erat ac risus lacinia aliquet.

![BoxChoice]({{ site.url }}/images/boxlist.jpg "BoxList")

### List 2

Vestibulum nec lacus sit amet diam vestibulum iaculis id nec velit. Nulla facilisis justo sit amet magna finibus ultrices. Ut nec venenatis velit. Fusce elementum egestas nunc, vel ultricies ex scelerisque vel. Ut at sem iaculis, consequat orci ac, maximus libero. Morbi sapien ante, sollicitudin quis nibh vel, vulputate egestas justo. Cras accumsan nisi vel consectetur lacinia. Nunc lacinia nibh eget imperdiet vehicula. Nulla nec pulvinar justo. Morbi nisi ligula, varius consequat tempus sit amet, tempor ac tellus. Etiam viverra vestibulum turpis, et commodo massa.

## Get Information to Create a Glove

Duis non dignissim elit, quis pretium risus. Vestibulum maximus tincidunt ex sit amet fringilla. Nam lacinia elit nec massa venenatis pellentesque. Donec nec urna sollicitudin, lacinia magna quis, volutpat felis. Duis a tellus sit amet sapien tristique rhoncus. Vivamus semper quis arcu nec feugiat. Nulla vitae elit nisi. In sit amet erat ac risus lacinia aliquet.

Note. Vestibulum ultricies erat ut `code` blandit velit eleifend. Go here <a href="https://servicechannel.zendesk.com/hc/en-us/articles/208072226-API-Integration">link</a> proin hendrerit, orci rhoncus vestibulum bibendum, justo nisi sodales felis, eu gravida mi purus et sapien. Cras fringilla molestie nibh, non auctor orci vehicula quis. Nam luctus magna sed lorem interdum elementum. Mauris finibus mi sit amet leo pharetra consequat. Nunc neque lacus, aliquet vel risus ac, gravida malesuada ipsum. Quisque aliquam ante vel luctus placerat.
{: .notice-inverse}

Vestibulum nec lacus sit amet diam vestibulum iaculis id nec velit. Nulla facilisis justo sit amet magna finibus ultrices. Ut nec venenatis velit. Fusce elementum egestas nunc, vel ultricies ex scelerisque vel. Ut at sem iaculis, consequat orci ac, maximus libero.

* `LocationId`
* `AreaId` and `ExtendedAreaName`
* `ProblemType`
* `AssetType`
* `ProblemCode`

Duis non dignissim elit, quis pretium risus. Vestibulum maximus tincidunt ex sit amet fringilla. Nam lacinia elit nec massa venenatis pellentesque. Donec nec urna sollicitudin, lacinia magna quis, volutpat felis. Duis a tellus sit amet sapien tristique rhoncus. Vivamus semper quis arcu nec feugiat. Nulla vitae elit nisi. In sit amet erat ac risus lacinia aliquet.

### LocationId

`LocationId` vestibulum nec lacus sit amet diam vestibulum iaculis id nec velit. Nulla facilisis justo sit amet magna finibus ultrices.

Required Parameter | Parameter Type | Example Value
-------------- | -------------- | --------------
Authorization | Header | Bearer `{access-token}`

GET /locations
{: .notice-info}

##### Example request

```http
GET https://aselivanava.github.io/locations HTTP/1.1
Authorization: Bearer {access-token}
```     

##### Example response

Response code: HTTP/1.1 200 OK

```json
{
    "glossary": {
        "title": "example glossary",
		"GlossDiv": {
            "title": "S",
			"GlossList": {
                "GlossEntry": {
                    "ID": "SGML",
					"SortAs": "SGML",
					"GlossTerm": "Standard Generalized Markup Language",
					"Acronym": "SGML",
					"Abbrev": "ISO 8879:1986",
					"GlossDef": {
                        "para": "A meta-markup language, used to create markup languages such as DocBook.",
						"GlossSeeAlso": ["GML", "XML"]
                    },
					"GlossSee": "markup"
                }
            }
        }
    }
}
```

<a href="https://sb2api.servicechannel.com/swagger/ui/index#!/Locations/Locations_GetLocations_0" class="btn">Test it!</a>

Use the response to get the following field:

Required Field | Response Body Field
-------------- | --------------
`LocationId` | `Locations` — `Id`

### AreaId

`AredId` vestibulum nec lacus sit amet diam vestibulum iaculis id nec velit. Nulla facilisis justo sit amet magna finibus ultrices. Ut nec venenatis velit. Fusce elementum egestas nunc, vel ultricies ex scelerisque vel. Ut at sem iaculis, consequat orci ac, maximus libero. Morbi sapien ante, sollicitudin quis nibh vel, vulputate egestas justo.

POST /subscribers/<wbr>current<wbr>/storedashboards<wbr>/current/<wbr>issuelist/<wbr>areas
{: .notice-success}

Required Parameter | Parameter Type | Example Value
-------------- | -------------- | --------------
Authorization | Header | Bearer `{access-token}`

##### Example request

```http
GET https://aselivanava.github.io/subscribers/current/storedashboards/current/issuelist/areas HTTP/1.1
Authorization: Bearer {access-token}
```

##### Example response

```json
myObj = {
    "name":"John",
    "age":30,
    "cars": {
        "car1":"Ford",
        "car2":"BMW",
        "car3":"Fiat"
    }
 }
```

<a href="https://sb2api.servicechannel.com/swagger/ui/index#!/Locations/Locations_GetLocations_0" class="btn">Test it!</a>

Use the response to get the following fields:

Required Field | Response Body Field
-------------- | --------------
`AreaId` | `IssueAreas` — `ID`
`ExtendedAreaName` | `IssueAreas` — `Name`

### ProblemType

`ProblemType` vestibulum nec lacus sit amet diam vestibulum iaculis id nec velit.

GET /subscribers<wbr>/current/storedashboards<wbr>/current/issuelist<wbr>areas/{areaId}/<wbr>problemtypes
{: .notice-danger}

Required Parameter | Parameter Type | Example Value
-------------- | -------------- | --------------
Authorization | Header | Bearer `{access-token}`
areaId	| Path	| 4935

##### Example request

```http
GET https://aselivanava.github.io/subscribers/current/storedashboards/current/issuelist/areas/4935/problemtypes HTTP/1.1
Authorization: Bearer {access-token}
```

##### Example response

```json
myObj = {
    "name":"John",
    "age":30,
    "cars": {
        "car1":"Ford",
        "car2":"BMW",
        "car3":"Fiat"
    }
 }
```

<a href="https://sb2api.servicechannel.com/swagger/ui/index#!/Locations/Locations_GetLocations_0" class="btn">Test it!</a>

Use the response to get the following field:

Required Field | Response Body Field
-------------- | --------------
`ProblemType`	| `ProblemGroupNames` — choose any name

### AssetType

`AssetType` vestibulum nec lacus sit amet diam vestibulum iaculis id nec velit. Nulla facilisis justo sit amet magna finibus ultrices. Ut nec venenatis velit. Fusce elementum egestas nunc, vel ultricies ex scelerisque vel. Ut at sem iaculis, consequat orci ac, maximus libero. Morbi sapien ante, sollicitudin quis nibh vel, vulputate egestas justo. Cras accumsan nisi vel consectetur lacinia. Nunc lacinia nibh eget imperdiet vehicula. Nulla nec pulvinar justo. Morbi nisi ligula, varius consequat tempus sit amet, tempor ac tellus. Etiam viverra vestibulum turpis, et commodo massa.

GET /subscribers/<wbr>current/storedashboards/<wbr>current/issuelist<wbr>/areas/<wbr>{areaId}/problemtypes/<wbr>{problemType}/<wbr>equipmenttypes?locationId={locationId}
{: .notice-info}

Required Parameter | Parameter Type | Example Value
-------------- | -------------- | --------------
Authorization | Header | Bearer `{access-token}`
areaId | Path	| 4935
problemType	| Path	| “Elevator”
locationId	| Query	| 2006071467

##### Example request

```http
GET https://aselivanava.github.io/subscribers/current/storedashboards/current/issuelist/areas/4935/problemtypes/Elevator/equipmenttypes?locationId=2006071467 HTTP/1.1
Authorization: Bearer {access-token}
```

##### Example response

```json
{
   "IssueEquipmentTypes": [
      "Freight Elevator",
      "Passenger Elevator"
   ]
}
```
<a href="https://sb2api.servicechannel.com/swagger/ui/index#!/Locations/Locations_GetLocations_0" class="btn">Test it!</a>

Use the response to get the following field:

Required Field | Response Body Field
-------------- | --------------
`AssetType`	| `IssueEquipmentTypes` — choose any name

### ProblemCode

`ProblemCode` vestibulum nec lacus sit amet diam vestibulum iaculis id nec velit. Nulla facilisis justo sit amet magna finibus ultrices. Ut nec venenatis velit. Fusce elementum egestas nunc, vel ultricies ex scelerisque vel. Ut at sem iaculis, consequat orci ac, maximus libero. Morbi sapien ante, sollicitudin quis nibh vel, vulputate egestas justo. Cras accumsan nisi vel consectetur lacinia. Nunc lacinia nibh eget imperdiet vehicula. Nulla nec pulvinar justo. Morbi nisi ligula, varius consequat tempus sit amet, tempor ac tellus. Etiam viverra vestibulum turpis, et commodo massa.

GET /subscribers/<wbr>current/storedashboard/<wbr>current/<wbr>issuelist/<wbr>areas/{areaId}/<wbr>problemtypes/<wbr>{problemType}/<wbr>equipmenttypes/<wbr>{equipmentType}/<wbr>problemcod
{: .notice-warning}

Required Parameter | Parameter Type | Example Value
-------------- | -------------- | --------------
Authorization | Header | Bearer `{access-token}`
areaId	| Path	| 4935
problemType	| Path	| “Elevator”
equipmentType	| Path	| “Freight Elevator”

##### Example request

```http
GET https://aselivanava.github.io/subscribers/current/storedashboards/current/issuelist/areas/4935/problemtypes/Elevator/equipmenttypes/Freight%20Elevator/problemcodes HTTP/1.1
Authorization: Bearer {access-token}
```

##### Example response

```json
myObj = {
    "name":"John",
    "age":30,
    "cars": {
        "car1":"Ford",
        "car2":"BMW",
        "car3":"Fiat"
    }
 }
```

<a href="https://sb2api.servicechannel.com/swagger/ui/index#!/Locations/Locations_GetLocations_0" class="btn">Test it!</a>

Use the response to get the following field:

Required Field | Response Body Field
-------------- | --------------
`ProblemCode` | `Problems` — choose any name

## Create a Glove Using Basic Parameters

Hestibulum nec lacus sit amet diam vestibulum iaculis id nec velit. Nulla facilisis justo sit amet magna finibus ultrices. Ut nec venenatis velit. Fusce elementum egestas nunc, vel ultricies ex scelerisque vel. Ut at sem iaculis, consequat orci ac, maximus libero. Morbi sapien ante, sollicitudin quis nibh vel, vulputate egestas justo. Cras accumsan nisi vel consectetur lacinia. Nunc lacinia nibh eget imperdiet vehicula. Nulla nec pulvinar justo. Morbi nisi ligula, varius consequat tempus sit amet, tempor ac tellus. Etiam viverra vestibulum turpis, et commodo massa.

DELETE /subscribers/current<wbr>/storedashboards<wbr>/current<wbr>/issuelist<wbr>/areas/{areaId}<wbr>/problemtypes<wbr>/{problemType}/equipmenttypes<wbr>/{equipmentType}<wbr>/problemcodes}
{: .notice-info}

Required Parameter | Parameter Type | Example Value
-------------- | -------------- | --------------
Authorization | Header | Bearer `{access-token}`
Content-Type | Header | application/json
request | Body | See example request

##### Example request

```http
POST https://aselivanava.github.io/workorders HTTP/1.1
Content-Type: application/json
Authorization: Bearer {access-token}
```

```json
myObj = {
    "name":"John",
    "age":30,
    "cars": {
        "car1":"Ford",
        "car2":"BMW",
        "car3":"Fiat"
    }
 }

```

##### Example response

```json
myObj = {
    "name":"John",
    "age":30,
    "cars": {
        "car1":"Ford",
        "car2":"BMW",
        "car3":"Fiat"
    }
 }
```
<a href="https://sb2api.servicechannel.com/swagger/ui/index#!/Locations/Locations_GetLocations_0" class="btn">Test it!</a>

Hestibulum nec lacus sit amet diam vestibulum iaculis id nec velit. Nulla facilisis justo sit amet magna finibus ultrices. Ut nec venenatis velit. Fusce elementum egestas nunc, vel ultricies ex scelerisque vel. Ut at sem iaculis, consequat orci ac, maximus libero. Morbi sapien ante, sollicitudin quis nibh vel, vulputate egestas justo. Cras accumsan nisi vel consectetur lacinia. Nunc lacinia nibh eget imperdiet vehicula. Nulla nec pulvinar justo. Morbi nisi ligula, varius consequat tempus sit amet, tempor ac tellus. Etiam viverra vestibulum turpis, et commodo massa.

## Creating a Glove Using Additional Parameters

Hestibulum nec lacus sit amet diam vestibulum iaculis id nec velit. Nulla facilisis justo sit amet magna finibus ultrices. Ut nec venenatis velit. Fusce elementum egestas nunc, vel ultricies ex scelerisque vel. Ut at sem iaculis, consequat orci ac, maximus libero. Morbi sapien ante, sollicitudin quis nibh vel, vulputate egestas justo. Cras accumsan nisi vel consectetur lacinia. Nunc lacinia nibh eget imperdiet vehicula. Nulla nec pulvinar justo. Morbi nisi ligula, varius consequat tempus sit amet, tempor ac tellus. Etiam viverra vestibulum turpis, et commodo massa.

### Troubleshooting Tip

Hestibulum nec lacus sit amet diam vestibulum iaculis id nec velit. Nulla facilisis justo sit amet magna finibus ultrices. Ut nec venenatis velit. Fusce elementum egestas nunc, vel ultricies ex scelerisque vel. Ut at sem iaculis, consequat orci ac, maximus libero. Morbi sapien ante, sollicitudin quis nibh vel, vulputate egestas justo. Cras accumsan nisi vel consectetur lacinia. Nunc lacinia nibh eget imperdiet vehicula. Nulla nec pulvinar justo. Morbi nisi ligula, varius consequat tempus sit amet, tempor ac tellus. Etiam viverra vestibulum turpis, et commodo massa.

### Interactive Troubleshooting

Hestibulum nec lacus sit amet diam vestibulum iaculis id nec velit. Nulla facilisis justo sit amet magna finibus ultrices. Ut nec venenatis velit. Fusce elementum egestas nunc, vel ultricies ex scelerisque vel. Ut at sem iaculis, consequat orci ac, maximus libero. Morbi sapien ante, sollicitudin quis nibh vel, vulputate egestas justo. Cras accumsan nisi vel consectetur lacinia. Nunc lacinia nibh eget imperdiet vehicula. Nulla nec pulvinar justo. Morbi nisi ligula, varius consequat tempus sit amet, tempor ac tellus. Etiam viverra vestibulum turpis, et commodo massa.

#### About the Interactive Troubleshooting

Hestibulum nec lacus sit amet diam vestibulum iaculis id nec velit. Nulla facilisis justo sit amet magna finibus ultrices. Ut nec venenatis velit. Fusce elementum egestas nunc, vel ultricies ex scelerisque vel. Ut at sem iaculis, consequat orci ac, maximus libero. Morbi sapien ante, sollicitudin quis nibh vel, vulputate egestas justo. Cras accumsan nisi vel consectetur lacinia. Nunc lacinia nibh eget imperdiet vehicula. Nulla nec pulvinar justo. Morbi nisi ligula, varius consequat tempus sit amet, tempor ac tellus. Etiam viverra vestibulum turpis, et commodo massa.

#### Get AdditionalFields

Hestibulum nec lacus sit amet diam vestibulum iaculis id nec velit. Nulla facilisis justo sit amet magna finibus ultrices. Ut nec venenatis velit. Fusce elementum egestas nunc, vel ultricies ex scelerisque vel. Ut at sem iaculis, consequat orci ac, maximus libero. Morbi sapien ante, sollicitudin quis nibh vel, vulputate egestas justo. Cras accumsan nisi vel consectetur lacinia. Nunc lacinia nibh eget imperdiet vehicula. Nulla nec pulvinar justo. Morbi nisi ligula, varius consequat tempus sit amet, tempor ac tellus. Etiam viverra vestibulum turpis, et commodo massa.

#### Create a Glove Using AdditionalFields

Hestibulum nec lacus sit amet diam vestibulum iaculis id nec velit. Nulla facilisis justo sit amet magna finibus ultrices. Ut nec venenatis velit. Fusce elementum egestas nunc, vel ultricies ex scelerisque vel. Ut at sem iaculis, consequat orci ac, maximus libero. Morbi sapien ante, sollicitudin quis nibh vel, vulputate egestas justo. Cras accumsan nisi vel consectetur lacinia. Nunc lacinia nibh eget imperdiet vehicula. Nulla nec pulvinar justo. Morbi nisi ligula, varius consequat tempus sit amet, tempor ac tellus. Etiam viverra vestibulum turpis, et commodo massa.

#### Additional Parameters to Consider

Hestibulum nec lacus sit amet diam vestibulum iaculis id nec velit. Nulla facilisis justo sit amet magna finibus ultrices. Ut nec venenatis velit. Fusce elementum egestas nunc, vel ultricies ex scelerisque vel. Ut at sem iaculis, consequat orci ac, maximus libero. Morbi sapien ante, sollicitudin quis nibh vel, vulputate egestas justo. Cras accumsan nisi vel consectetur lacinia. Nunc lacinia nibh eget imperdiet vehicula. Nulla nec pulvinar justo. Morbi nisi ligula, varius consequat tempus sit amet, tempor ac tellus. Etiam viverra vestibulum turpis, et commodo massa.

### Beg Information

Hestibulum nec lacus sit amet diam vestibulum iaculis id nec velit. Nulla facilisis justo sit amet magna finibus ultrices. Ut nec venenatis velit. Fusce elementum egestas nunc, vel ultricies ex scelerisque vel. Ut at sem iaculis, consequat orci ac, maximus libero. Morbi sapien ante, sollicitudin quis nibh vel, vulputate egestas justo. Cras accumsan nisi vel consectetur lacinia. Nunc lacinia nibh eget imperdiet vehicula. Nulla nec pulvinar justo. Morbi nisi ligula, varius consequat tempus sit amet, tempor ac tellus. Etiam viverra vestibulum turpis, et commodo massa.

## Find Duplicate Gloves

Hestibulum nec lacus sit amet diam vestibulum iaculis id nec velit. Nulla facilisis justo sit amet magna finibus ultrices. Ut nec venenatis velit. Fusce elementum egestas nunc, vel ultricies ex scelerisque vel. Ut at sem iaculis, consequat orci ac, maximus libero. Morbi sapien ante, sollicitudin quis nibh vel, vulputate egestas justo. Cras accumsan nisi vel consectetur lacinia. Nunc lacinia nibh eget imperdiet vehicula. Nulla nec pulvinar justo. Morbi nisi ligula, varius consequat tempus sit amet, tempor ac tellus. Etiam viverra vestibulum turpis, et commodo massa.

### Possible Duplicates

Hestibulum nec lacus sit amet diam vestibulum iaculis id nec velit. Nulla facilisis justo sit amet magna finibus ultrices. Ut nec venenatis velit. Fusce elementum egestas nunc, vel ultricies ex scelerisque vel. Ut at sem iaculis, consequat orci ac, maximus libero. Morbi sapien ante, sollicitudin quis nibh vel, vulputate egestas justo. Cras accumsan nisi vel consectetur lacinia. Nunc lacinia nibh eget imperdiet vehicula. Nulla nec pulvinar justo. Morbi nisi ligula, varius consequat tempus sit amet, tempor ac tellus. Etiam viverra vestibulum turpis, et commodo massa.

### Potential Recalls

Hestibulum nec lacus sit amet diam vestibulum iaculis id nec velit. Nulla facilisis justo sit amet magna finibus ultrices. Ut nec venenatis velit. Fusce elementum egestas nunc, vel ultricies ex scelerisque vel. Ut at sem iaculis, consequat orci ac, maximus libero. Morbi sapien ante, sollicitudin quis nibh vel, vulputate egestas justo. Cras accumsan nisi vel consectetur lacinia. Nunc lacinia nibh eget imperdiet vehicula. Nulla nec pulvinar justo. Morbi nisi ligula, varius consequat tempus sit amet, tempor ac tellus. Etiam viverra vestibulum turpis, et commodo massa.

## Create a Second Glove

Hestibulum nec lacus sit amet diam vestibulum iaculis id nec velit. Nulla facilisis justo sit amet magna finibus ultrices. Ut nec venenatis velit. Fusce elementum egestas nunc, vel ultricies ex scelerisque vel. Ut at sem iaculis, consequat orci ac, maximus libero. Morbi sapien ante, sollicitudin quis nibh vel, vulputate egestas justo. Cras accumsan nisi vel consectetur lacinia. Nunc lacinia nibh eget imperdiet vehicula. Nulla nec pulvinar justo. Morbi nisi ligula, varius consequat tempus sit amet, tempor ac tellus. Etiam viverra vestibulum turpis, et commodo massa.
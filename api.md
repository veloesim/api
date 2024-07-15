## [1 Plans](#11-getAllPlans)

[1.1 getAllPlans](#11-getAllPlans)

[1.2 getOnePlan](#12-getOnePlan)

## [2 Organizations](#21-getMyOrganization)

[2.1 getMyOrganization](#21-getMyOrganization)

## [3 Orders](#31-orderOne)

[3.1 orderOne](#31-orderOne)

## [4 Esims](#41-getAllEsims)

[4.1 getAllEsims](#41-getAllEsims)

[4.2 getOneEsim](#42-getOneEsim)

[4.3 getEsimTopUpPlans](#43-getEsimTopUpPlans)

[4.4 topUpEsim](#44-topUpEsim)


# 1. Plans
## 1.1 getAllPlans

### Description
This request can be used to retrieve the list of plans.


### Inputs
|Parameter|Presence|Description|
|-----|--------|-----------|
|limit|Optional|The maximum number of results to return|
|offset|Optional|The number of results to skip before starting to return results|
|areaRegions|Optional|An array of strings for searching by area names with case-insensitive partial matching|
|areaNames|Optional|An array of strings for searching by area regions with case-insensitive partial matching|
|areaIds|Optional|An array of IDs for filtering results by specific area ID|

#### Request
```sh
curl --location 'https://api.veloesim.com:2053/api/wholesale/plans?limit=6&offset=0&areaIds=5&areaIds=151' \
--header 'Authorization: Apikey {{apiKey}}'
```
#### Answer

```json
{
  "count": 12,
  "rows": [
    {
      "id": 33,
      "dataAmount": 1000,
      "duration": 7,
      "price": 5.5,
      "areas": [
        {
          "id": 5,
          "name": "Chile",
          "region": "South America",
          "iso": "CL"
        }
      ]
    },
    {
      "id": 622,
      "dataAmount": 3000,
      "duration": 30,
      "price": 13,
      "areas": [
        {
          "id": 5,
          "name": "Chile",
          "region": "South America",
          "iso": "CL"
        }
      ]
    },
    {
      "id": 1014,
      "dataAmount": 5000,
      "duration": 30,
      "price": 19,
      "areas": [
        {
          "id": 5,
          "name": "Chile",
          "region": "South America",
          "iso": "CL"
        }
      ]
    },
    {
      "id": 1548,
      "dataAmount": 10000,
      "duration": 30,
      "price": 31,
      "areas": [
        {
          "id": 5,
          "name": "Chile",
          "region": "South America",
          "iso": "CL"
        }
      ]
    },
    {
      "id": 1999,
      "dataAmount": 20000,
      "duration": 30,
      "price": 52,
      "areas": [
        {
          "id": 5,
          "name": "Chile",
          "region": "South America",
          "iso": "CL"
        }
      ]
    },
    {
      "id": 148,
      "dataAmount": 1000,
      "duration": 7,
      "price": 4,
      "areas": [
        {
          "id": 151,
          "name": "Europe+",
          "region": null,
          "iso": null
        },
        {
          "id": 19,
          "name": "Austria",
          "region": "Europe",
          "iso": "AT"
        },
        {
          "id": 24,
          "name": "Belgium",
          "region": "Europe",
          "iso": "BE"
        },
        {
          "id": 25,
          "name": "Bulgaria",
          "region": "Europe",
          "iso": "BG"
        },
        {
          "id": 31,
          "name": "Switzerland",
          "region": "Europe",
          "iso": "CH"
        },
        {
          "id": 34,
          "name": "Cyprus",
          "region": "Middle East",
          "iso": "CY"
        },
        {
          "id": 35,
          "name": "Northern Cyprus",
          "region": "Europe",
          "iso": "CYP"
        },
        {
          "id": 36,
          "name": "Czech Republic",
          "region": "Europe",
          "iso": "CZ"
        },
        {
          "id": 37,
          "name": "Germany",
          "region": "Europe",
          "iso": "DE"
        },
        {
          "id": 38,
          "name": "Denmark",
          "region": "Europe",
          "iso": "DK"
        },
        {
          "id": 39,
          "name": "Estonia",
          "region": "Europe",
          "iso": "EE"
        },
        {
          "id": 41,
          "name": "Spain",
          "region": "Europe",
          "iso": "ES"
        },
        {
          "id": 42,
          "name": "Finland",
          "region": "Europe",
          "iso": "FI"
        },
        {
          "id": 44,
          "name": "United Kingdom",
          "region": "Europe",
          "iso": "GB"
        },
        {
          "id": 49,
          "name": "Greece",
          "region": "Europe",
          "iso": "GR"
        },
        {
          "id": 52,
          "name": "Croatia",
          "region": "Europe",
          "iso": "HR"
        },
        {
          "id": 53,
          "name": "Hungary",
          "region": "Europe",
          "iso": "HU"
        },
        {
          "id": 54,
          "name": "Canary Islands",
          "region": "Europe",
          "iso": "IC"
        },
        {
          "id": 56,
          "name": "Ireland",
          "region": "Europe",
          "iso": "IE"
        },
        {
          "id": 60,
          "name": "Iceland",
          "region": "Europe",
          "iso": "IS"
        },
        {
          "id": 69,
          "name": "Liechtenstein",
          "region": "Europe",
          "iso": "LI"
        },
        {
          "id": 71,
          "name": "Lithuania",
          "region": "Europe",
          "iso": "LT"
        },
        {
          "id": 72,
          "name": "Luxembourg",
          "region": "Europe",
          "iso": "LU"
        },
        {
          "id": 73,
          "name": "Latvia",
          "region": "Europe",
          "iso": "LV"
        },
        {
          "id": 82,
          "name": "Malta",
          "region": "Europe",
          "iso": "MT"
        },
        {
          "id": 86,
          "name": "Netherlands",
          "region": "Europe",
          "iso": "NL"
        },
        {
          "id": 87,
          "name": "Norway",
          "region": "Europe",
          "iso": "NO"
        },
        {
          "id": 92,
          "name": "Poland",
          "region": "Europe",
          "iso": "PL"
        },
        {
          "id": 93,
          "name": "Portugal",
          "region": "Europe",
          "iso": "PT"
        },
        {
          "id": 96,
          "name": "Romania",
          "region": "Europe",
          "iso": "RO"
        },
        {
          "id": 61,
          "name": "Italy",
          "region": "Europe",
          "iso": "IT"
        },
        {
          "id": 101,
          "name": "Sweden",
          "region": "Europe",
          "iso": "SE"
        },
        {
          "id": 103,
          "name": "Slovenia",
          "region": "Europe",
          "iso": "SI"
        },
        {
          "id": 104,
          "name": "Slovakia",
          "region": "Europe",
          "iso": "SK"
        },
        {
          "id": 110,
          "name": "Turkey",
          "region": "Middle East",
          "iso": "TR"
        },
        {
          "id": 118,
          "name": "Holy See (Vatican City State)",
          "region": "Europe",
          "iso": "VA"
        },
        {
          "id": 43,
          "name": "France",
          "region": "Europe",
          "iso": "FR"
        }
      ]
    }
  ]
}
```
## 1.2 getOnePlan

### Description
This request can be used to retrieve plan.


### Inputs
| Parameter |Presence|Description|
|-----------|--------|-----------|
| id        |Mandatory|ID of the plan|

#### Request
```sh
curl --location 'https://api.veloesim.com:2053/api/wholesale/plans/2' \
--header 'Authorization: Apikey {{apiKey}}'
```
#### Answer

```json
{
  "id": 1,
  "dataAmount": 1000,
  "duration": 7,
  "price": 20,
  "areas": [
    {
      "id": 16,
      "name": "Andorra",
      "region": "Europe",
      "iso": "AD"
    }
  ]
}
```

# 2. Organizations
## 2.1 getMyOrganization

### Description
This request can be used to retrieve your organization.

#### Request
```shell
curl --location 'https://api.veloesim.com:2053/api/wholesale/organizations' \
--header 'Authorization: Apikey {{apiKey}}'
```
#### Answer

```json
{
  "balance": 89,
  "name": "Fortis"
}
```

# 3. Orders
## 3.1 orderOne

### Description
This request can be used to purchase the plan. 
If the customer email is provided, the plan will be assigned to the customer, and the customer will become a VeloeSIM user. 
The user will receive a password to log in to the VeloeSIM application.

### Inputs
| Parameter        | Presence  | Description               |
|------------------|-----------|---------------------------|
| planId           | Mandatory | ID of the plan            |
| customerEmail    | optional  | Email of the customer     |
| customerFullName | optional  | Full name of the customer |

#### Request
```shell
curl --location 'https://api.veloesim.com:2053/api/wholesale/orders' \
--header 'Content-Type: application/json' \
--header 'Authorization: Apikey {{apiKey}}' \
--data '{"planId": 2604}'
```
#### Answer

```json
{
  "iosSetup": "https://esimsetup.apple.com/esim_qrcode_provisioning?carddata=LPA:1$address.test$X2-2XXXX7-LCIUXQ",
  "iccid": "89372040161688888888",
  "matchingId": "X2-2XXXX7-LCIUXQ",
  "smdpAddress": "address.test",
  "profileStatus": "RELEASED",
  "installedAt": null,
  "assignedPlans": [
    {
      "initialQuantityInBytes": 1000000000,
      "remainingQuantityInBytes": 1000000000,
      "startTime": null,
      "endTime": null,
      "isExpired": false,
      "areas": [
        {
          "id": 49,
          "name": "Greece",
          "region": "Europe",
          "iso": "GR"
        }
      ]
    }
  ]
}
```

# 4. Esims
## 4.1 getAllEsims

### Description
This request can be used to retrieve all esims assigned to your organization.

### Inputs
|Parameter|Presence|Description|
|-----|--------|-----------|
|limit|Optional|The maximum number of results to return|
|offset|Optional|The number of results to skip before starting to return results|

#### Request
```shell
curl --location 'https://api.veloesim.com:2053/api/wholesale/esims?limit=6&offset=0' \
--header 'Authorization: Apikey {{apiKey}}'
```
#### Answer

```json
{
  "count": 5,
  "rows": [
    {
      "iosSetup": "https://esimsetup.apple.com/esim_qrcode_provisioning?carddata=LPA:1$address.test$K2-22KXXXX-8L2N1T",
      "iccid": "8937204016163448888",
      "matchingId": "K2-22KXXXX-8L2N1T",
      "smdpAddress": "address.test",
      "profileStatus": "RELEASED",
      "installedAt": null,
      "assignedPlans": [
        {
          "id": 89,
          "planId": 5,
          "initialQuantityInBytes": 1000000000,
          "remainingQuantityInBytes": 1000000000,
          "startTime": null,
          "endTime": null,
          "isExpired": false,
          "areas": [
            {
              "id": 49,
              "name": "Greece",
              "region": "Europe",
              "iso": "GR"
            }
          ]
        }
      ]
    },
    {
      "iosSetup": "https://esimsetup.apple.com/esim_qrcode_provisioning?carddata=LPA:1$address.test$K2-22XXXX-1H27S99",
      "iccid": "8937204016163448888",
      "matchingId": "K2-22XXXX-1H27S99",
      "smdpAddress": "address.test",
      "profileStatus": "RELEASED",
      "installedAt": null,
      "assignedPlans": [
        {
          "id": 90,
          "planId": 5,
          "initialQuantityInBytes": 1000000000,
          "remainingQuantityInBytes": 1000000000,
          "startTime": null,
          "endTime": null,
          "isExpired": false,
          "areas": [
            {
              "id": 49,
              "name": "Greece",
              "region": "Europe",
              "iso": "GR"
            }
          ]
        }
      ]
    },
    {
      "iosSetup": "https://esimsetup.apple.com/esim_qrcode_provisioning?carddata=LPA:1$address.test$K2-22XXXX-1JBDHTX",
      "iccid": "8937204016163448888",
      "matchingId": "K2-22XXXX-1JBDHTX",
      "smdpAddress": "address.test",
      "profileStatus": "RELEASED",
      "installedAt": null,
      "assignedPlans": [
        {
          "id": 91,
          "planId": 5,
          "initialQuantityInBytes": 1000000000,
          "remainingQuantityInBytes": 1000000000,
          "startTime": null,
          "endTime": null,
          "isExpired": false,
          "areas": [
            {
              "id": 49,
              "name": "Greece",
              "region": "Europe",
              "iso": "GR"
            }
          ]
        }
      ]
    },
    {
      "iosSetup": "https://esimsetup.apple.com/esim_qrcode_provisioning?carddata=LPA:1$address.test$K2-22XXXX-URAUIK",
      "iccid": "8937204016163448888",
      "matchingId": "K2-22XXXX-URAUIK",
      "smdpAddress": "address.test",
      "profileStatus": "RELEASED",
      "installedAt": null,
      "assignedPlans": [
        {
          "id": 92,
          "planId": 5,
          "initialQuantityInBytes": 1000000000,
          "remainingQuantityInBytes": 1000000000,
          "startTime": null,
          "endTime": null,
          "isExpired": false,
          "areas": [
            {
              "id": 49,
              "name": "Greece",
              "region": "Europe",
              "iso": "GR"
            }
          ]
        }
      ]
    },
    {
      "iosSetup": "https://esimsetup.apple.com/esim_qrcode_provisioning?carddata=LPA:1$address.test$K2-22XXXX-LCIUXQ",
      "iccid": "8937204016163448888",
      "matchingId": "K2-22XXXX-LCIUXQ",
      "smdpAddress": "address.test",
      "profileStatus": "RELEASED",
      "installedAt": null,
      "assignedPlans": [
        {
          "id": 93,
          "planId": 5,
          "initialQuantityInBytes": 1000000000,
          "remainingQuantityInBytes": 1000000000,
          "startTime": null,
          "endTime": null,
          "isExpired": false,
          "areas": [
            {
              "id": 49,
              "name": "Greece",
              "region": "Europe",
              "iso": "GR"
            }
          ]
        }
      ]
    }
  ]
}
```
## 4.2 getOneEsim

### Description
This request can be used to retrieve the eSIM assigned to your organization.

### Inputs
| Parameter |Presence| Description           |
|-----------|--------|-----------------------|
| iccid     |Mandatory| the iccid of the eSIM |

#### Request
```shell
curl --location 'https://api.veloesim.com:2053/api/wholesale/esims/8937204016163448888' \
--header 'Authorization: Apikey {{apiKey}}'
```
#### Answer

```json
{
  "iosSetup": "https://esimsetup.apple.com/esim_qrcode_provisioning?carddata=LPA:1$address.test$K2-22XXXX-LCIUXQ",
  "iccid": "8937204016163448888",
  "matchingId": "K2-22XXXX-LCIUXQ",
  "smdpAddress": "address.test",
  "profileStatus": "RELEASED",
  "installedAt": null,
  "assignedPlans": [
    {
      "id": 89,
      "planId": 5,
      "initialQuantityInBytes": 1000000000,
      "remainingQuantityInBytes": 1000000000,
      "startTime": null,
      "endTime": null,
      "isExpired": false,
      "areas": [
        {
          "id": 49,
          "name": "Greece",
          "region": "Europe",
          "iso": "GR"
        }
      ]
    }
  ]
}
```

## 4.3 getEsimTopUpPlans

### Description
This request retrieves the available top-up plans for the eSIM.

### Inputs
| Parameter |Presence| Description           |
|-----------|--------|-----------------------|
|limit|Optional|The maximum number of results to return|
|offset|Optional|The number of results to skip before starting to return results|
| iccid     |Mandatory| the iccid of the eSIM |
| planId    |Mandatory| ID of the plan |

#### Request
```shell
curl --location 'https://api.veloesim.com:2053/api/wholesale/esims/8937204016163448888/top-up' \
--header 'Authorization: Apikey {{apiKey}}'
```
#### Answer

```json
{
    "count": 5,
    "rows": [
        {
            "id": 5,
            "dataAmount": 1000,
            "duration": 7,
            "price": 5,
            "areas": [
                {
                    "id": 124,
                    "name": "Albania",
                    "region": "Europe",
                    "iso": "AL"
                }
            ]
        },
        {
            "id": 593,
            "dataAmount": 3000,
            "duration": 30,
            "price": 12,
            "areas": [
                {
                    "id": 124,
                    "name": "Albania",
                    "region": "Europe",
                    "iso": "AL"
                }
            ]
        },
        {
            "id": 985,
            "dataAmount": 5000,
            "duration": 30,
            "price": 18,
            "areas": [
                {
                    "id": 124,
                    "name": "Albania",
                    "region": "Europe",
                    "iso": "AL"
                }
            ]
        },
        {
            "id": 1524,
            "dataAmount": 10000,
            "duration": 30,
            "price": 25,
            "areas": [
                {
                    "id": 124,
                    "name": "Albania",
                    "region": "Europe",
                    "iso": "AL"
                }
            ]
        },
        {
            "id": 1976,
            "dataAmount": 20000,
            "duration": 30,
            "price": 42,
            "areas": [
                {
                    "id": 124,
                    "name": "Albania",
                    "region": "Europe",
                    "iso": "AL"
                }
            ]
        }
    ]
}
```

## 4.4 topUpEsim

### Description
This request tops up the eSIM.

### Inputs
| Parameter |Presence| Description           |
|-----------|--------|-----------------------|
| iccid     |Mandatory| the iccid of the eSIM |
| planId    |Mandatory| ID of the plan |

#### Request
```shell
curl --location 'https://api.veloesim.com:2053/api/wholesale/esims/8937204016163448888/top-up' \
--header 'Content-Type: application/json' \
--header 'Authorization: Apikey {{apiKey}}'
--data '{
    "planId": 1
}'
```
#### Answer

```json
{
  "iosSetup": "https://esimsetup.apple.com/esim_qrcode_provisioning?carddata=LPA:1$address.test$K2-22XXXX-LCIUXQ",
  "iccid": "8937204016163448888",
  "matchingId": "K2-22XXXX-LCIUXQ",
  "smdpAddress": "address.test",
  "profileStatus": "RELEASED",
  "installedAt": null,
  "assignedPlans": [
    {
      "id": 89,
      "planId": 5,
      "initialQuantityInBytes": 1000000000,
      "remainingQuantityInBytes": 402593548,
      "startTime": "2024-05-18T19:24:18.000Z",
      "endTime": "2024-05-25T20:00:00.000Z",
      "isExpired": false,
      "areas": [
        {
          "id": 49,
          "name": "Greece",
          "region": "Europe",
          "iso": "GR"
        }
      ]
    },
    {
      "id": 95,
      "planId": 5,
      "initialQuantityInBytes": 1000000000,
      "remainingQuantityInBytes": 1000000000,
      "startTime": null,
      "endTime": null,
      "isExpired": false,
      "areas": [
        {
          "id": 49,
          "name": "Greece",
          "region": "Europe",
          "iso": "GR"
        }
      ]
    }
  ]
}
```

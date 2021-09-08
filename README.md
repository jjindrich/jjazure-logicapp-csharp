# JJAzure LogicApp demo
Using Azure LogicApps Standard

https://docs.microsoft.com/en-us/azure/logic-apps/create-single-tenant-workflows-visual-studio-code

## How to run service locally

Start Azurit as Azure Storage simulator

Next hit F5 or run command

```ps
func host start
```

Open Overview page on workflow.json to get Url

## Test simple HTTP TestStateless service

Test this url

```ps
curl "http://localhost:7071/api/TestStateless/triggers/manual/invoke?api-version=2020-05-01-preview&sp=%2Ftriggers%2Fmanual%2Frun&sv=1.0&sig=XwoqbC3bQA9pOij-hiEW6cqP7UomyrGLVbZg7xzvwpw"
```

# Test simple HTTP GET TestGet service

This service run HTTP GET endpoint and return result based on "name" property in url.

Test this url - change /a to your value

```ps
curl "http://localhost:7071/api/TestGet/triggers/manual/invoke/a?api-version=2020-05-01-preview&sp=%2Ftriggers%2Fmanual%2Frun&sv=1.0&sig=3SBS6PVCHNiOdJImJvZbK51zb1pleoaeykuZvi9aZP4"
```

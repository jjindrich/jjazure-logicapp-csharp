# JJAzure LogicApp demo
Using Azure LogicApps Standard

https://docs.microsoft.com/en-us/azure/logic-apps/create-single-tenant-workflows-visual-studio-code

# Run simple HTTP TestStateless service

Start Azurit as Azure Storage simulator

Next hit F5 or run command

```ps
func host start
```

Open Overview page on workflow.json to get Url

Test this url like you will get response

```ps
curl "http://localhost:7071/api/TestStateless/triggers/manual/invoke?api-version=2020-05-01-preview&sp=%2Ftriggers%2Fmanual%2Frun&sv=1.0&sig=XwoqbC3bQA9pOij-hiEW6cqP7UomyrGLVbZg7xzvwpw"
```

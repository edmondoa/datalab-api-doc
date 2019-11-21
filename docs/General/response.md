# Responses
`200`
```json 
{
  "status": {
    "success": true,
    "previousPage": "1",
    "count": "1",
    "nextPage": "3",    
  },
  "request": {
    <key> : <value>,
    "resource" : "resource url"
  },
  "payload": { 
        /* Application-specific data would go here. */ 
    } 
}

```
`400`
```json
{
  "status": {
    "success" : false,
    "message" : "Something went wrong"   
  },
  "request": {
   <key> : <value>,
    "resource" : "resource url"
  }
}

```


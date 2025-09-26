# [NAME] API v[X.Y.Z]

```
LEGEND: REQ:required OPT:optional AUTH:authentication RATE:rate-limit ERR:error-codes MIME:content-type
VARS: X:version Y:endpoint-count Z:max-payload-size
```

## OVERVIEW
```
BASE:[https://api.domain.com/v[X]] AUTH:[method] RATE:[X]req/min MIME:[json|xml|form]
```

## ENDPOINTS
```
GET /[resource] → [response-object] AUTH:[req|opt|none] RATE:[X]/min
POST /[resource] → [create-response] BODY:[schema] AUTH:req RATE:[X]/min  
PUT /[resource]/[id] → [update-response] BODY:[schema] AUTH:req RATE:[X]/min
DELETE /[resource]/[id] → [delete-response] AUTH:req RATE:[X]/min
```

## REQUEST SCHEMAS
```js
[ResourceCreate]{field:type REQ, field:type OPT, nested:{subfield:type}}
[ResourceUpdate]{field:type OPT, field:type OPT}
```

## RESPONSE SCHEMAS  
```js
[Success]{data:[ResourceObject], meta:{total:int,page:int}}
[Error]{error:{code:int,message:string,details:[string]}}
```

## AUTH
```
METHOD:[jwt|oauth|apikey|basic] HEADER:[Authorization|X-API-Key]
TOKEN:[Bearer [token]|[scheme] [credentials]] SCOPE:[read|write|admin]
```

## ERRORS
```
400:bad-request→[validation-details] 401:unauthorized→[auth-required]
403:forbidden→[insufficient-permissions] 404:not-found→[resource-missing]
429:rate-limit→[retry-after] 500:server-error→[contact-support]
```

## RATE LIMITS
```
GLOBAL:[X]req/min PER-ENDPOINT:[Y]req/min BURST:[Z]req/10s
HEADERS:X-RateLimit-Remaining,X-RateLimit-Reset
```

## VALIDATION
```
✓all-endpoints-tested ✓auth-enforced ✓rate-limits-active ✓errors-documented
```

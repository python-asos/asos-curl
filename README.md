# asos-curl
ASOS executor plugin for HTTP(s) requests

## Parameters

You can configure the executor by setting the following parameters in the task:

```json
{
	"url": "https://example.com/",
	"method": "GET",
	"get_params": {"param": "value"},
	"post_data": {"item": "content"},
	"no_dump": true
}
```

Supported methods: GET, POST, PUT, PATCH, OPTIONS

## ASOS Task example

```json
{
  "url": "https://example.com/api/dance",
  "task_type": "curl",
  "get_params": {
    "page": 1,
    "perPage": 8,
    "filter": true
  },
  "request_type": "GET",
  "task_interval": 60
}
```

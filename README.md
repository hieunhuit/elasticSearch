# Elastic Search 7.x Basic
## Clone an index
```sh
POST http://127.0.0.1:9200/_reindex
{
    "source": {
        "index": "sourceindexname"
    },
    "dest": {
        "index": "destindexname"
    }
}
```
Response
```sh
{
    "took": 489,
    "timed_out": false,
    "total": 114,
    "updated": 0,
    "created": 114,
    "deleted": 0,
    "batches": 1,
    "version_conflicts": 0,
    "noops": 0,
    "retries": {
        "bulk": 0,
        "search": 0
    },
    "throttled_millis": 0,
    "requests_per_second": -1.0,
    "throttled_until_millis": 0,
    "failures": []
}
```

# Performance test results with 20 todos initially added

Brief description of the used server: HTTP/1.1

Brief description of local machine used: MacBook Pro, Processor: 2,2 GHz 6-Core Intel Core i7, Memory: 16 GB 2400 MHz DDR4

## No Caching

Results based on the K6 test run on project assignment https://github.com/aiotrope/tetraval main branch.

### Retrieving todos

http_reqs: 11359

http_req_duration - median: 8.69ms

http_req_duration - 99th percentile: 26.23ms

## With Redis Caching

Results based on the K6 test run on project assignment https://github.com/aiotrope/limerence main branch.

### Retrieving todos

http_reqs: 14724

http_req_duration - median: 6.68ms

http_req_duration - 99th percentile: 16.86ms

## Reflection

The application with Redis cache has a higher http request rate compared to the app without caching. The request duration for application without caching has longer request duration compared to the app with redis cache. Redis caching based on the test run can generate higher request rate and lower the request duration time.

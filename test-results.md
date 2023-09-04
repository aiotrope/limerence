# Performance test results with 20 todos initially added

Brief description of the used server (choose one): HTTP/1.1

Brief description of local machine used: MacBook Pro, Processor: 2,2 GHz 6-Core Intel Core i7, Memory: 16 GB 2400 MHz DDR4

## No Caching

### Retrieving todos

http_reqs: 147032

http_req_duration - median: 630.75µs

http_req_duration - 99th percentile: 1.32ms


## With Redis Caching

### Retrieving todos

http_reqs: 14724

http_req_duration - median: 6.68ms

http_req_duration - 99th percentile: 16.86ms 

## Reflection

Brief reflection on the results of the tests -- why do you think you saw the results you saw:

The test results show that the JSON API without database has a greater request rate and is considerably faster than the API with Postgresql database, which could be attributed to the slower performance of the relational database structure.
## Why we need to cache
- Reuse accessed resources
- Reduce latency and Increase throughput
- Lower not only the cost of time but also other

## Strategies
- Cache-Aside
- Read-Though
- Write-Though
- Write-Back

### Cache-Aside
Most used and intuitional strategy.

![cache-aside example](https://github.com/Elfen-Lied/Elfen-Lied.github.io/blob/master/assets/images/2.png)

#### When accessing data:
1. Check if data is available in cache instance
2. If yes, return data
3. Otherwise, execute orignal plan (etc. query database)
4. Application write returned data into cache instance

#### When updating data:
1. Update data source first
2. Then expire data in cache instance



# Offshore Configuration

## Configuration

#### Cache

you can configure the cache by adding a `cache` object key in the offshore.initialize config object.
all options are optional.

##### options:
`adapter:` use a specific adapter ( ex: {adapter: require('offshore-memory')} ) 
`defaultCacheTime:` time in ms to keep cache if no `cacheTime` in query is specified

###### default adapter options:
`prefix:` the files prefix name.
`path:` a directory to place cache files

###### exemple:
```javascript
    offshore.initialize({ cache: { prefix: 'test_cache_', defaultCacheTime: 100 }, ... 
```

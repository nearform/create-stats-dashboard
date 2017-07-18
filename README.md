# create-stats-dashboard

A wrapper to create and initialise a stats dashboard on kibana using [import-kibana-dashboard](http://github.com/nearform/import-kibana-dashboard), for easy manipulation of [stats](http://github.com/nearform/stats) sent via [stats-to-elasticsearch](http://github.com/nearform/stats-to-elasticsearch)

## installation
```
npm install -g @nearform/create-stats-dashboard
```

## CLI Usage

```
$ create-stats-dashboard -h $ES_HOST -p $ES_PORT
```

## Programmatic usage

```js
const createStatsDashboard = require('@nearform/create-stats-dashboard')
createStatsDashboard({
  host: 'es-host', // default localhost
  port: 'es-port', // default 9200
})
```

## License
Apache-2.0
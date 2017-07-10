# import-stats-dashboard

Initialise a stats dashboard on kibana using import-kibana-dashboard

## installation
```
npm i create-stats-dashboard
```

## CLI Usage

```
$ import-stats-dashboard -h $ES_HOST -p $ES_PORT
```

## Programmatic usage

```js
const importStatDashboard = require('create-stats-dashboard')
importStatDashboard({
  host: 'es-host', // default localhost
  port: 'es-port', // default 9200
})
```

## License
Apache-2.0
# create-stats-dashboard

A wrapper to create and initialise a stats dashboard on kibana using [import-kibana-dashboard](http://github.com/nearform/import-kibana-dashboard), for easy manipulation of [stats](http://github.com/nearform/stats) sent via [stats-to-elasticsearch](http://github.com/nearform/stats-to-elasticsearch)

## Intro to the nearform stats tooling

Created with the purpose to make creating visualisations about your process easy. At nearform, we achieve this using the modules [stats](http://github.com/nearform/stats), [stats-to-elasticsearch](http://github.com/nearform/stats-to-elasticsearch) and [create-stats-dashboard](http://github.com/nearform/create-stats-dashboard). This makes it very easy to collect process stats in elasticsearch and visualise them in a dashboard in kibana, similar to that below:

<img src='./assets/dashboard-screenshot.png' alt='a kibana stats dashboard screenshot'>

Once your dashboard is setup with create-stats-dashboard, all you should need to do is require the stats-to-elasticsearch module and point it at the dashboard to get cool (and useful) visualisations!
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

## Useful links

- [stats](http://github.com/nearform/stats) - makes generating the stats to be visualised a breeze!
- [stats-to-elasticsearch](http://github.com/nearform/stats-to-elasticsearch) - makes sending the stats to es a breeze!
- [create-stats-dashboard](http://github.com/nearform/create-stats-dashboard) - makes creating your kibana dashboard a breeze!


## License
Apache-2.0
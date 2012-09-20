# Flatiron-REPL

## Allow your app to get a repl easily

```javascript
app.use(require('flatiron-repl'), {
  port: 1337,
  whitelist: [
    '127.0.0.1',
    {address:'10.0.0.1', port: '777'}
  ]
});
```

## Client executable included

```bash
rrepl 1337
```

And once we are in the REPL

```javascript
> app.config.get('database:url')
'127.0.0.1:5984'
```
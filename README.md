# Como usar esse buildpack no Heroku

### Adicione ao seu app Heroku

```
heroku buildpacks:add --index 1 https://github.com/seu-usuario/heroku-buildpack-mongo-tools
heroku buildpacks:add heroku/ruby # ou outro buildpack principal
```

> O buildpack Mongo deve vir antes do Ruby para configurar corretamente o PATH.

###  Teste se funcionou

```
heroku run bash
```

- E dentro do bash:

```
which mongodump
mongodump --version
```


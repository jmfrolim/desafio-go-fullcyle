<h1>Desafio golang FullCycle Docker</h1>

<h2>Imagem no Docker HUB:</h2>

<b>jmfrolim/codeducation</b>

<h2>Dockerfile</h2>

1. Construir o container:
```
$ docker-compose up -d --build
```

2. Construir a imagem:
```
$ docker build -t jmfrolim/codeeducation ./app -f ./app/Dockerfile
```

3. Upload para o Docker Hub:
```
$ docker push jmfrolim/codeeducation
```

4. Testar a execução:
```
$ docker container run jmfrolim/codeeducation
```

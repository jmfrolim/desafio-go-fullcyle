<h1>Desafio golang FullCycle Docker</h1>

<h3> <b>O desafio</b> </h3>
<h4>


Publicar uma imagem no docker hub. Quando executarmos:

docker run <seu-user>/codeeducation

Temos que ter o seguinte resultado: Code.education Rocks!

Se você perceber, essa imagem apenas realiza um print da mensagem como resultado final, logo, vale a pena dar uma conferida no próprio site da Go Lang para aprender como fazer um "olá mundo".

Lembrando que a Go Lang possui imagens oficiais prontas, vale a pena consultar o Docker Hub.

3) A imagem de nosso projeto Go precisa ter menos de 2MB =)
</h4>

</br>

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

# DockerDOOM
Primero he descargado el binario con link de una version pasada de la pagina, ya que la original no esta disponible actualmente. <br>
[link](https://web.archive.org/web/20160310005603/https://gideonred.com/bins/dockerdoomd.tar.gz)

Una vez descargado, lo he descomprimido con ```tar -vzxf dockerdoomd.tar.gz``` <br>
Para la prueba crearé 2 contenedores de prueba con el comando de ejemplo oficial ```for i in {1..2} ; do docker run -d -t ubuntu:14.04; done``` <br>
![imagen](https://user-images.githubusercontent.com/91600940/168313001-b2d12a38-3b75-41f0-bff0-37ee1f6a1f15.png)



Luego he ejecutado el binario directamente con ```./dockerdoomd```.
```
2022/05/13 16:25:47 Pulling image from public repo
Using default tag: latest
latest: Pulling from gideonred/dockerdoom
Image docker.io/gideonred/dockerdoom:latest uses outdated schema1 manifest format. Please upgrade to a schema2 image for better future compatibility. More information at https://docs.docker.com/registry/spec/deprecated-schema-v1/
a3ed95caeb02: Pull complete 
3b1d42cd9af9: Pull complete 
707a1369b69a: Pull complete 
2dcca790c489: Pull complete 
0196e3ce559c: Pull complete 
682077412d02: Pull complete 
30a6ea0d5ddf: Pull complete 
Digest: sha256:294ac5e8f73512348369d00dffd772733325b4d0468b141ae5e83381df252946
Status: Downloaded newer image for gideonred/dockerdoom:latest
docker.io/gideonred/dockerdoom:latest
2022/05/13 16:26:30 Image downloaded
2022/05/13 16:26:30 Trying to start docker container ...
2022/05/13 16:26:30 Waiting 5 seconds for "dockerdoom" to show in "docker ps". You can change this wait with -dockerWait.
PORT=5900
2022/05/13 16:26:35 Docker container started, you can now connect to it with a VNC viewer at port 5900
PORT=5900
```

Para la conexión he utilizado el programa *Remmina*, el cual soporta conexiones **VNC**.<br>
Como ponia en el resultado de la consola, utiliza el puerto **5900**
![imagen](https://user-images.githubusercontent.com/91600940/168309717-d3c4742f-f8c9-40cd-8a6a-c833ae57baf0.png) <br>
La contraseña a utilizar es ```1234``` <br>
![imagen](https://user-images.githubusercontent.com/91600940/168310245-1a7e5e8b-3fe6-455b-996b-a4687ec1e05a.png)

Una vez dentro del juego, se puede ver estan los contenedores como enemigos. <br>
![imagen](https://user-images.githubusercontent.com/91600940/168313711-a8d2a71f-293e-449e-9125-2712984cefd1.png) <br>
Después de una dura batalla, una vez que los enemigos han sido completamente eliminados, también se eliminan los contenedores que estaban ligados a ellos. <br>
![imagen](https://user-images.githubusercontent.com/91600940/168314683-c9983399-4d1a-42ce-ac1b-e438458ac4e1.png)

![imagen](https://user-images.githubusercontent.com/91600940/168314254-13ec0dc5-b473-4541-93b5-579858e1b874.png)



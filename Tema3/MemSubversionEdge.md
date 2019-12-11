##### Instal·lació de subversion:
Per tal de descarregar la imatge del Subversion Edge des de Docker Hub, farem:
```bash
1 $ docker run -d mamohr/subversion-edge
2 Unable to find image 'mamohr/subversion-edge:latest' locally
3 latest: Pulling from mamohr/subversion-edge
4 469cfcc7a4b3: Pull complete
5 7e814dc876c6: Pull complete
6 144c1c97a750: Pull complete
7 17eb6ecf9d0a: Pull complete
8 12492ca50197: Pull complete
9 32dc87336990: Pull complete
10 Digest: sha256:547356
    c2d4c2b2a7eb6e8f7b84de52118ca7089b98d2400f7c723e2280022ab6
11 Status: Downloaded newer image for mamohr/subversion-edge:latest
```
De moment, veiem els contenidors que tenim en execució:
```bash
1 :~$ docker ps
2 CONTAINER ID              IMAGE               COMMAND                                                                              CREATED                        STATUS                PORTS                                                                                                     NAMES
3 3a44963e4e29 mamohr/subversion-edge "/config/bootstrap.sh"
    26 seconds ago Up 25 seconds 3343/tcp, 4434/tcp, 18080/
        tcp nifty_ramanujan
```
I anem a aturar-lo i eliminar-lo:
```bash
1 $ docker stop 3a44963e4e29
2 3a44963e4e29
3 $ docker rm 3a44963e4e29
4 3a44963e4e29
```
Ara tornarem a llençar el contenidor de la següent forma:
```bash
$ docker run -d -p 3343:3343 -p 4434:4434 -p 18080:18080 --name  svnserver mamohr/subversion-edge
2 bcebfd61510e4fb5c456503a81c528f535d2407a90df1a8a031b1300edc8335a
```
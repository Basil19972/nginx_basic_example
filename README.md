# nginx_basic_example

A Basic Example how to set up a mini Webserver for static Websites

# Nginx: Mini Webserver für Static Content

So sieht das Dockerfile aus sehr simple

![Bildschirm­foto 2023-01-27 um 12.04.26.png](Nginx%20Mini%20Webserver%20fu%CC%88r%20Static%20Content%204b81f840f539489e8355bcde5bd50025/Bildschirmfoto_2023-01-27_um_12.04.26.png)

![Bildschirm­foto 2023-01-27 um 12.04.38.png](Nginx%20Mini%20Webserver%20fu%CC%88r%20Static%20Content%204b81f840f539489e8355bcde5bd50025/Bildschirmfoto_2023-01-27_um_12.04.38.png)

Mit dem befehl wird das Image erstellt

```
docker build -t html-server-image:v1 .
```

MIt dem Befehl wird der Container gestartet

```
docker run -d -p 80:80 html-server-image:v1
```

## Um das Docker Image anderen zu Teilen

Dort wo man sich mit dem Terminal befindet wird eine zip.tar datei erstellt welche dann wieder geladen werden kann.

### zum speichern:

```
docker save html-server-image:v1 > walImage.tar
```

### um das Image zu laden

```
docker load < walimage.tar
```


# How to set up a web server using Docker?

For this tutorial we are going to set up a simple web server and deploy a web page on our local machine.

## Lets Get started:

### Step 1: Make a directory

```bash
$ mkdir test
$ cd test
```

### Step 2: Now create a file name 'Dockerfile' (Make sure that this do not have any extansion)

```bash
$ touch Dockerfile
```

### Step 3: Next create a simple web page 'index.html'

```bash
$ vim index.html
```
copy and paste code from below:
```HTML
<!DOCTYPE html>
<html>
  <body>
  
  <h1>Hello world!!</h>
  
  </body>
</html>
```
Once its done press ```Esc``` and type ```:wq``` to save and exit

### Step 4: Now open 'Dockerfile' in vi editor

```bash
$ vi Dockerfile
```
Now, copy and paste the code below in vi editor
```bash
FROM centos:latest

MAINTAINER NewstarCorporation

RUN yum -y install httpd

COPY index.html /var/www/html/

CMD [“/usr/sbin/httpd”, “-D”, “FOREGROUND”]

EXPOSE 80
```
Then exit out of vi editor using ```Esc``` >> ```:wq```

### Step 5: Next we are going to build the image using docker build.

```bash
$ docker build /test/ -t webserver:v1
```

(Test is our current directory, and -t is name the image, in our case "webserver:v1")

### Step 6: Run docker image

```bash
$ docker build /test/ -t webserver:v1
```

### Step 7: Now to see the results on web browser

```web
http://<host ip>:1234/
```


## A Gunicorn based app

- Write the Dockerfile
- Build the image with `docker build -t guni-app .`
- Run the container with `docker run -d -p 80:80 -v /opt/docker-course/apps/2.2:/app --name guni-server guni-app`
- Note the -v flag. That means now the local directory is "mounted" on the container, and any changes you make are reflected on the server, thanks to the --reload flag.

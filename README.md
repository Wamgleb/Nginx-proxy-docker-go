# Nginx-proxy-docker-go
We will set up your workspace and create a simple Go web app, which you’ll later containerize. 
The Go app will use the powerful gorilla/mux request router, chosen for its flexibility and speed.

My first import net/http and gorilla/mux packages, which provide HTTP server functionality and routing.

Deploy the nginx-proxy by running:

docker-compose -f nginx-proxy-compose.yaml up -d

You’ve deployed nginx-proxy and its Let’s Encrypt companion using Docker Compose. Next, you’ll create a Dockerfile for your Go web app.
Remember to replace your_domain both times with your domain name. Save and close the file.
You’ll run your Go web app in the background via Docker Compose with the following command:

docker-compose -f go-app-compose.yaml up -d

You can navigate to https://your_domain/ to see your homepage. 

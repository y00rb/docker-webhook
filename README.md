## docker-webhook
The project is works for automated-build on [docker-hub](https://hub.docker.com/)

#### How used?
Please used `POST` request to [docker repo](https://hub.docker.com/r/yangbodotnet/docker-webhook/) after each commit on github.
```bash
curl -H "Content-Type: application/json" --data '{"build": true}' -X POST https://registry.hub.docker.com/u/yangbodotnet/docker-webhook/trigger/ab3e1dca-4543-4742-ba95-0096128dcb39/
```
- the docker-hub will tigger building proccess follow **Build Setting**
- docker-hub will tagging each individaul image after built

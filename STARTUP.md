To start MQTT daemon : 
```
docker run -d --restart unless-stopped \
    --name mqtt \
    -p 1883:1883 \
    -p 9001:9001 \
    --memory 50m \
    --cpus=0.25 \
    -v /home/omartin/proj/mosquitto:/mosquitto \
    eclipse-mosquitto:latest
```
This can run anywhere. In my project, it runs on the Raspberry PI (BrickPi)

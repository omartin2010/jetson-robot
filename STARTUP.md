To start MQTT daemon : 
```
docker run --rm -d \
    --name mqtt \
    -p 1883:1883 \
    -p 9001:9001 \
    -v /home/robot/mosquitto/mosquitto.conf:/mosquitto/config/mosquitto.conf \
    eclipse-mosquitto:latest
```
This can run anywhere. In my project, it runs on the Raspberry PI (BrickPi)

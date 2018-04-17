# Command
Install homebridge on PI3



## run
```
sudo docker rm hb -f
sudo docker run \
--net=host \
--name=homebridge \
-e PUID=911 -e PGID=911 \
-e HOMEBRIDGE_CONFIG_UI=1 \
-e HOMEBRIDGE_CONFIG_UI_PORT=8080 \
-v /home/pi/homebridge:/homebridge \
-d=true \
--name=hb \
oznu/homebridge:raspberry-pi

sudo docker logs hb
```

# Zoneminder 1.30.4 for Raspberry Pi

To run:
```
docker run \
   -d \
   -e TZ="Europe/Berlin" \
   --restart=always \
   --privileged="true" \
   -p 8080:80 \
   --name zoneminder \
   -v "/media/zm/config":"/config":rw \
   -v "/media/zm/data":"/var/cache/zoneminder":rw \
   murphaph/rpi-zoneminder	
```

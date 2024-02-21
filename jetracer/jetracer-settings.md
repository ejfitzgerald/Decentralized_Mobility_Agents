# JetRacer
Find the detials of the JetRacer ROS AI Kit in this [official wiki](https://www.waveshare.com/wiki/JetRacer_ROS_AI_Kit)

## To run the vehicle around
Browse to the jupyter notebook *ip-address-of-jetracer:8888* (password: `jetson`) and navigate to **parking.ipynb**, this code runs the vehicle in a straight line and stops when it detects the aruco marker on the [mock charger](/mock-charger/infra-settings.md)

Note: For advanced driving scenario (track following) use **lab_drive.ipynb** (beware that it has to be driven on a track)

## Kuksa client 
This will publish JetRacer identification
```
docker run --rm -it --net=host indrasenr/kuksa-client:publisher
```

## DDS
to run the publisher
```
cd dds/
docker run -it --rm --name publisher -v $(pwd)/config:/config -v $(pwd):/app --net=host indrasenr/dds:cdds_v2 python3 /app/publisher.py
```
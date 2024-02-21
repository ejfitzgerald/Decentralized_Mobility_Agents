# JetRacer
Find the detials of the JetRacer ROS AI Kit in this [official wiki](https://www.waveshare.com/wiki/JetRacer_ROS_AI_Kit)

## To run the vehicle around
Browse to the jupyter notebook *ip-address-of-jetracer:8888* and navigate to **parking.ipynb**, this code runs the vehicle in a straight line and stops when it detects the aruco marker on the [mock charger](/mock-charger/infra-settings.md)

## Kuksa client, this will publish JetRacer identification
```
docker run --rm -it --net=host indrasenr/kuksa-client:publisher
```
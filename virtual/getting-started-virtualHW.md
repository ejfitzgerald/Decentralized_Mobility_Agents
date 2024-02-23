## To run the virtual HW on macbook m1/m2 (arm64)
In the first terminal
```
docker run --rm -it --privileged --net=host --name virtual-rpi4 indrasenr/vsoc:rpi4-bcx-arm64
```
in the next terminal, to run DDS publisher example
```
docker exec -it virtual-rpi4 /bin/bash
cd dds
python3 publisher.py
```
in third terminal, to run DDS subscriber example
```
docker exec -it virtual-rpi4 /bin/bash
cd dds
python3 subscriber.py
```

## To run the virtual HW on linux machine (amd64)
```
docker run --rm -it --privileged --net=host --name virtual-rpi4 indrasenr/vsoc:rpi4-bcx-amd64
```
to run the DDS example, follow the same steps as for the Macbook



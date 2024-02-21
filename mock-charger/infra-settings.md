## Kuksa client 
this will subscribe JetRacer identification
```
docker run --rm -it --net=host indrasenr/kuksa-client:subscriber
```

## To display the aruco marker
```
ssh indra@<tailscale-ip-address>
```
password: bosch123

```
cd aruco
streamlit run streamlit-app.py
```
then browse to `tailscale-ip-address:8501/aruco_marker_generator`, choose the *Marker ID*, use **Generate and Display Marker** button to display the aruco marker and **Clear Display** button to clear the aruco marker
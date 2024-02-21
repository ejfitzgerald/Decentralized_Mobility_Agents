## SSI flow 
Refer to the below figure for the SSI flow, here vehicle is [JetRacer](/jetracer/jetracer-settings.md) or simulated vehicle in MetaVerse, infrastructure is the [mock-charger](/mock-charger/infra-settings.md) and SSI server is the [Bosch Infrastucture](/host/bosch-host-settings.md).

### To play with the flow
On the Bosch infrastructure, run the following
```
cd work/ssi/
conda activate py39_ssi
streamlit run ssi-dashboard.py
```

![Figure](/figures/SSI_flow.png) 
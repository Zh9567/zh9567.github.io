# Bus Position map
As we are currently figuring out how to make the python code work on the site, so we just release the code here for you to download to check it out.

## Data sources
[GTFS Realtime - data.gov.my](https://developer.data.gov.my/realtime-api/gtfs-)

## How to run (desktop)
You might need to install these packages first:
```
pip install flask flask-cors protobuf requests gtfs-realtime-bindings
```

1. Download `app.py` and `index.html`.
2. Run `app.py` with Python.
```
python "path_to_file\app.py"
```
> A list of vehicles is shown at `http://localhost:5000/vehicles` in json format.
3. Open `index.html` in a browser.

## Technical notes
* Rapid KL: Some new or leased buses are not shown, or shown with an incorrect number plate (where the bus with that number plate is actually retired).
* MRT Feeder Bus: Some buses are not shown in Putrajaya and Cyberjaya.
* All Prasarana bus services: Buses that are not in service or waiting for next trip is not shown.
* Causeway Link: Some buses outside Greater Johor Bahru area are not shown. BAS.MY Melaka is not shown (it is reported that it was shown during first few months of service). Some buses that are not in service or waiting for next trip is not shown.

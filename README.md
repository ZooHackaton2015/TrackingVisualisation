# TrackingVisualisation
Simple visualisation for tracking device

# Description
Our solution is using GoogleMaps JS API and OpenCellID API. 
It parses the input string, which is just for this demo purposes in 
format like:

```
  <point1text, will be shown on marker>+CENG:0,"<bts information according to AT commands descriptions>".
  <point2text, will be shown on marker>+CENG:0,"<bts information according to AT commands descriptions>".
  <point3text, will be shown on marker>+CENG:0,"<bts information according to AT commands descriptions>".
  ...
```

from the second parts of the bts infromation, it gets MCC, MNC, LAC, CELLID and label. Then use this to get info from OpenCellID and creates path and markers using google API (it's verry well documented). 

For running the demo you need to get API key for OpenCellID as well as for GoogleMaps API Key. It should be obvious where to put them in the code.

#https://github.com/splunk/security_content/blob/develop/detections/endpoint/local_account_discovery_with_net.yml

#https://github.com/AlienVault-OTX/OTX-Python-SDK

#https://github.com/AlienVault-OTX/OTX-Python-SDK/blob/master/howto_use_python_otx_api.ipynb

from OTXv2 import OTXv2, IndicatorTypes
from pandas.io.json import *
from datetime import datetime, timedelta
otx = OTXv2("<API KEY>")

l = ['65907dc1aa71349e21f223a7', '6639c5a2a700d80b13f64258', '6639e815d63e06c21679e9da']

for i in l:
  indicators1 = i
  indicators2 = otx.get_pulse_indicators(indicators1)
  for x in indicators2: #works
    print("Pulse:" + i + "\n" + "Indicator:\n" + x["indicator"] + "\n" + "Type:\n" + x["type"] + '\n' + "Title:\n" + x['title'] + "\n\n")
  

# Get all the indicators associated with a pulse - works


#indicators = otx.get_pulse_indicators("65907dc1aa71349e21f223a7")
#65907dc1aa71349e21f223a7
#6639c5a2a700d80b13f64258
#6639e815d63e06c21679e9da

#print(indicators)



#for indicator in indicators: #works
  #print("Indicator:\n" + indicator["indicator"] + "\n" + "Type:\n" + indicator["type"] + '\n' + "Title:\n" + indicator['title'] + "\n\n")

  
# Get everything OTX knows about google.com
#otx.get_indicator_details_full(IndicatorTypes.DOMAIN, "google.com")


  
#print(otx.get_indicator_details_full(IndicatorTypes.DOMAIN, "google.com"))

# sharkeu
Home Assistant integration for SharkIQ with EU vacuums

This is just an adaptation of the [existing integration](https://github.com/home-assistant/core/tree/dev/homeassistant/components/sharkiq) with the [Unofficial SDK for Shark IQ](https://github.com/ajmarks/sharkiq) using EU servers.

This integration will not work for the US, just use the original and supported one.

## Installation 
Just copy the `sharkiqeu` directory to the `custom_components` folder on your home assistant installation. 


## Known Issues

#### Integration loses connection frequently
There is an open [issue](https://github.com/home-assistant/core/issues/44775) referring to this, the issue is due to the tokens only being valid for 24h, the current quick fix is just to reload the application daily using an automation

This could be fixed directly in the custom component but until then check out this [solution](https://github.com/home-assistant/core/issues/44775#issuecomment-758230213).

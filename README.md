# Remote gateway TTN configuration

TTN gateways using [this setup](https://github.com/ttn-zh/ic880a-gateway/tree/spi) can be configured to allow remote configuration. In that case, the gateways checks if there's a new setting file on each start up and if so, replaces the local configuration file.

## How to contribute?

Adding your remote configuration file here is easy:
- Create one JSON file with your gateway's EUI **in uppercase** as the name. So, if you gateway EUI is `B827EBFFFE4E743F`,  the file should be called `B827EBFFFE4E743F.json`
- The content of the file should be your `local_conf.json`, if you're unusure, copy [this file as template](https://github.com/ttn-zh/gateway-remote-config/blob/master/template.json) and update the following fields:
  - Gateway EUI
  - Email
  - Description
  - Server address (check [this list](https://www.thethingsnetwork.org/wiki/Backend/Connect/Gateway) if you are not using the European router)
  - Latitude, longitude and altitude
- Then [create a pull request](https://help.github.com/articles/creating-a-pull-request/) with it
- Wait a bit for it to be merged
- Profit!

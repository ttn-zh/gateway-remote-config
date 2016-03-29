# Remote gateway TTN configuration

TTN gateways using [this setup](https://github.com/ttn-zh/ic880a-gateway/tree/spi) can be configured to allow remote configuration. In that case, the gateways checks if there's a new setting file on each start up and if so, replaces the local configuration file.

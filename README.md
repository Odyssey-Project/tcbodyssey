# Hackathon TorizonCore Jan 2023 - OS Customization #

This project contains OS customization for the hackathon from 25/jan/2023, focused on building a demo project focused on DevOps for a multi-developer team.

## Customization ##

Before the event:

* [Provisioning at scale](https://developer.toradex.com/torizon/torizoncore/best-practices/production-programming-in-torizon/#provisioning-at-scale): create the custom image with online provisioning credentials.

## Build ##

Setup TCB then run:

```bash
export $(cat .env | xargs) && torizoncore-builder build --set MACHINE="colibri-imx6" --set ONLINE_PROVISIONING_DATA="$ONLINE_PROVISIONING_DATA"
```

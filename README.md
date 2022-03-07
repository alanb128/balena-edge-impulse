# balena-edge-impulse
Updated for 2022!

Quick project for running Edge Impulse on balena, specifically providing an example of accessing the Pi V2 camera using libcamera on Bullseye.

This project also installs the files required to run the [Edge Impulse Python SDK](https://docs.edgeimpulse.com/docs/linux-python-sdk).
## Use

You need to have a balena account and an Edge Impulse account with a working project.

Add the following device configuration variables:

`BALENA_HOST_CONFIG_gpu_mem` = 64

`BALENA_HOST_CONFIG_start_x` = 1


Push this project to your fleet (Raspberry Pi 4 only) and then SSH into the "ei" container.

Run `edge-impulse-linux` and follow the prompts.

Further usage instructions here: https://docs.edgeimpulse.com/docs/raspberry-pi-4#3-connecting-to-edge-impulse

## Notes

The Edge Impulse Linux software seems to require a Pulseaudio server, which is why we are using the audio block.

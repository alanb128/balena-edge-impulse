# balena-edge-impulse
Quick project for running Edge Impulse on balena. Updated for 2022

Currently this is broken with the error:

```
[SER] Using camera bcm2835-isp (/dev/video15) starting...
Failed to initialize linux tool Capture process failed with code 1
```

When starting a video capture source... We're actively looking for a solution.

## Use

You need to have a balena account and an Edge Impulse account with a working project.

Add the following device configuration variables:

`BALENA_HOST_CONFIG_gpu_mem` = 128

`BALENA_HOST_CONFIG_start_x` = 1


Push this project to your fleet (Raspberry Pi 4 only) and then SSH into the "ei" container.

Run `edge-impulse-linux` and follow the prompts.

Further usage instructions here: https://docs.edgeimpulse.com/docs/raspberry-pi-4#3-connecting-to-edge-impulse

## Notes

The Edge Impulse Linux software seems to require a Pulseaudio server, which is why we are using the audio block.

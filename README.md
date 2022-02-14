# balena-edge-impulse
Quick project for running Edge Impulse on balena. Updated for 2022

## Use

You need to have a balena account and an Edge Impulse account with a working project.

Push this project to your fleet (Raspberry Pi 4 only) and then SSH into the "ei" container.

Run `edge-impulse-linux` and follow the prompts.

Further usage instructions here: https://docs.edgeimpulse.com/docs/raspberry-pi-4#3-connecting-to-edge-impulse

## Notes

Currently only USB webcams seem to work - Pi Cam V2 coming soon!

The Edge Impulse Linux software seems to require a Pulseaudio server, which is why we are using the audio block.

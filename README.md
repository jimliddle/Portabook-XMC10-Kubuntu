# Portabook-XMC10-Kubuntu

This details the Kubuntu 20.04 install for a KingJim PortaBook XMC10

- Flash the Kubuntu ISO onto a USB using some like balenaEtcher
- Place the resultant USB into the Portabook USB slot
- Turn on the Portabook and press F2 to launch boot options
- Choose to boot from the USB
- Choose the option to run the live preview
- The Live preview will launch and everything (WiFi, USB, Sound, Bluetooth etc) should work fine
- When ready choose to install to the PortaBook by double clicking the option on the Kubuntu desktop
(Note due to the Portabook's disk size you will need to overwrite whatever OS you are currently using so you should back up anything you need prior to actually moving forward with the install)
- Choose the default suggested disk layout
- Step through the install options until complete
- Post first boot enter the terminal and alter grub as follows:<br/>
<code>GRUB_CMDLINE_LINUX_DEFAULT="quiet splash intel_idle.max_cstate=1"</code><br/>
(This will stop system freezes due to the Cherry Trail processor low power state)

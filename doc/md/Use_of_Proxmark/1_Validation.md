## 1. Validating proxmark client functionality

If all went well you should get some information about the firmware and memory usage as well as the prompt,  something like this.

```
[=] Session log /home/iceman/.proxmark3/log_20200521.txt
[+] loaded from JSON file /home/iceman/.proxmark3/preferences.json
[=] Using UART port /dev/ttyS7
[=] Communicating with PM3 over USB-CDC


██████╗ ███╗   ███╗ ████╗  
██╔══██╗████╗ ████║   ══█║ 
██████╔╝██╔████╔██║ ████╔╝ 
██╔═══╝ ██║╚██╔╝██║   ══█║ 
██║     ██║ ╚═╝ ██║ ████╔╝     Iceman ☕
╚═╝     ╚═╝     ╚═╝ ╚═══╝  ❄️ bleeding edge
 
 https://github.com/rfidresearchgroup/proxmark3/

 [ Proxmark3 RFID instrument ] 

 [ CLIENT ]
  client: RRG/Iceman/master/v4.9237-2-g2cb19874 2020-05-21 22:00:00
  compiled with GCC 9.3.0 OS:Linux ARCH:x86_64
 
 [ PROXMARK RDV4 ]
  device.................... RDV4
  firmware.................. RDV4
  external flash............ present
  smartcard reader.......... present
  FPC USART for BT add-on... absent

 [ ARM ]
 bootrom: RRG/Iceman/master/v4.9237-2-g2cb19874 2020-05-21 22:00:10
      os: RRG/Iceman/master/v4.9237-2-g2cb19874 2019-05-21 22:00:26
 compiled with GCC 9.2.1 20191025 (release) [ARM/arm-9-branch revision 277599]

 [ FPGA ]
  LF image built for 2s30vq100 on 2020-07-08 at 23: 8: 7
  HF image built for 2s30vq100 on 2020-07-08 at 23: 8:19
  HF FeliCa image built for 2s30vq100 on 2020-07-08 at 23: 8:30

 [ Hardware ] 
  --= uC: AT91SAM7S512 Rev A
  --= Embedded Processor: ARM7TDMI
  --= Internal SRAM size: 64K bytes
  --= Architecture identifier: AT91SAM7Sxx Series
  --= Embedded flash memory 512K bytes ( 59% used )

[usb] pm3 --> 
```

This `[usb] pm3 --> ` is the Proxmark3 interactive prompt.


### To get interactive help

For basic help type `help`. Or for help on a set of sub commands type the command followed by `help`. For example `hf mf help`.

### First tests

These commands will return some info about your Proxmark software and hardware status.
```
[usb] pm3 --> hw status
[usb] pm3 --> hw version
[usb] pm3 --> hw tune
```

You are now ready to use your newly flashed proxmark3 device.  Many commands uses the `h` parameter to show a help text.

### To quit the client
```
[usb] pm3 --> quit
```
or simple press `CTRL-D`.

## Next steps

Some configuration steps are still needed.

For the next steps, please read the following pages:

* [First Use and Verification](/doc/md/Use_of_Proxmark/2_Configuration-and-Verification.md)
* [Commands & Features](/doc/md/Use_of_Proxmark/3_Commands-and-Features.md)
 

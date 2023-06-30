# Default Keymap for XIUDI's 60% XD60 PCB

![Default Keymap for XD60](https://img.alicdn.com/imgextra/i1/1713761720/TB2K0gTalPxQeBjy1XcXXXHzVXa_!!1713761720.png)

## Additional Notes
Default Keymap for XD60 as indicated on the original sale page.

## Build

To build the default keymap, simply run:

    make xiudi/xd60/rev2:default  # XD60 rev2
    make xiudi/xd60/rev3:default  # XD60 rev3
    
    
## From VIA
 * steps:
 * configure keymap in via, save to: xd60_rev_3_layout.json
 * qmk via2json -km via -kb xiudi/xd60/rev3 ./xd60_rev_3.layout_via.json -o xd60_rev_3_layout.json
 * qmk json2c xd60_rev_3_layout.json -o keymap.c

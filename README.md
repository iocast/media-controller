# media-controller

source from https://www.instructables.com/DIY-USB-Media-Controller-for-PC/

install arduino-cli

```bash
sudo curl -fsSL https://raw.githubusercontent.com/arduino/arduino-cli/master/install.sh | sudo BINDIR=/usr/local/bin sh
```

search board support

```bash
arduino-cli core search leonardo
```

install board support

```bash
arduino-cli core install arduino:avr
```

install libraries

```bash
arduino-cli lib install FastLED
arduino-cli lib install HID-Project
```

build

```bash
arduino-cli compile -b arduino:avr:leonardo media-controller/ --output-dir ./build
arduino-cli compile -b arduino:avr:leonardo media-controller-inverted/ --output-dir ./build
```



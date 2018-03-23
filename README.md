# Android Things Weather Station sample

This sample shows integration of multiple Android Things peripheral to build a connected Weather Station.

## Screenshots

![Weather Station sample demo][demo-gif]

[(Watch the demo on YouTube)][demo-yt]

## Pre-requisites

- Android Things compatible board
- Android Studio 2.2+
- [Rainbow Hat for Android Things](https://shop.pimoroni.com/products/rainbow-hat-for-android-things) or the following individual components:
    - 1 [bmp280 temperature sensor](https://www.adafruit.com/product/2651)
    - 1 [segment display with I2C backpack](https://www.adafruit.com/product/1270)
    - 1 push button
    - 1 resistor
    - jumper wires
    - 1 breadboard
    - (optional) 1 [APA102 compatible RGB Led strip](https://www.adafruit.com/product/2241)
    - (optional) 1 [Piezo Buzzer](https://www.adafruit.com/products/160)

## Schematics

If you have the Raspberry Pi [Rainbow Hat for Android Things](https://shop.pimoroni.com/products/rainbow-hat-for-android-things), just plug it onto your Raspberry Pi 3.

![Schematics for Raspberry Pi 3](rpi3_schematics.png)

## Build and install

On Android Studio, click on the "Run" button.
If you prefer to run on the command line, type
```bash
./gradlew installDebug
adb shell am start com.example.androidthings.weatherstation/.WeatherStationActivity
```

If you have everything set up correctly:
- The segment display will show the current temperature.
- If the button is pressed, the display will show the current pressure.
- If a Piezo Buzzer is connected, it will plays a funny sound on startup.
- If a APA102 RGB Led strip is connected, it will display a rainbow of 7 pixels indicating the current pressure.


## License

Copyright 2016 The Android Open Source Project, Inc.

Licensed to the Apache Software Foundation (ASF) under one or more contributor
license agreements.  See the NOTICE file distributed with this work for
additional information regarding copyright ownership.  The ASF licenses this
file to you under the Apache License, Version 2.0 (the "License"); you may not
use this file except in compliance with the License.  You may obtain a copy of
the License at

  http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.  See the
License for the specific language governing permissions and limitations under
the License.

[demo-yt]: https://www.youtube.com/watch?v=FcdwfKehX_0&list=PLWz5rJ2EKKc-GjpNkFe9q3DhE2voJscDT&index=14
[demo-gif]: demo1.gif
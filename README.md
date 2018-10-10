![Logo](admin/xiaomiairpurifier.png)
# ioBroker.xiaomiairpurifier

Xiaomi Air Purifier adapter for ioBroker IoT platform. 

## Cloud Connection
To control the Air Purifier with the cloud adapter just add the state "favoritelevel" to your Cloud Adapter. After that you can send f.e. the following commands through Alexa:
*Alexa, turn the air purifier on*,
*Alexa, set the air purifier to 50%*,
*Alexa, turn the air purifier off*

If you set in the Cloud adapter the "On Value" to "Last active value" the device allways start running in the latest acitve power level.


## Control States
To control your air purifier, the following objects can be written:

| State          | Description |
| :---           | :---        |
| power          | Turn the device on / off  |
| auto           | Activate the auto mode of the device. |
| silent         | Activate the silent mode of the device. |
| favorite       | Activate the favorite mode of the device. |
| favoriteLevel  | Control the power of the favorite mode in the range from 0-100%. This will also turn on / off the device if neccessary |

## Info States
The following information is collected from your air purifier (read-only states):

### Device Info

| State       | Description |
| :---        | :---        |
| mode        | The actual device mode, just valid, if the device is powered on. |
| temperature | The messured temperature in °C of the device. |
| humidity    | The messured relative humidity in % of the device. |
| pm25        | The air polution in PM2.5. |

### 0.0.1
* (JoJ123) initial release

## License
The MIT License (MIT)

Copyright (c) 2018 Johannes Jaeger <johannesjaegeroffice@gmail.com>

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.

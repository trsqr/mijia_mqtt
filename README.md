# mijia_mqtt
Simple script to report temperature, humidity and battery level of Xiaomi Mijia Bluetooth Temperature and Humidity Sensor to MQTT. Requires gatttool, mosquitto_pub, bc and xxd tools to be installed.

I'm running this from cron on an Intel Compute Stick.

Temperatures returned are Celsius degrees.

## Example

```
root@green:~/src/mijia_mqtt# ./mijia_mqtt.sh -a 4c:65:a8:d9:3e:76 -n lab -b 192.168.99.13 -d
Querying 4c:65:a8:d9:3e:76 for temperature and humidity data.
Querying 4c:65:a8:d9:3e:76 for battery data.
Temperature: 21.2, Humidity: 59.2, Battery: 97
```

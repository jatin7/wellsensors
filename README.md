# wellsensors
This is a temporary repo for well sensor data.

Note that the output of log-synth is a list of individual JSON maps.  To convert to an array, use:
```
sed -e '1 s/^/[\n/' -e '$ s/$/\n]/' -e '$ ! s/$/,/' ws_1m.json > ws_new.json
```
Then, use the file ws_new.json for loading into MapR-DB.

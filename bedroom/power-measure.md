
# Power Measure

**!! Cannot be used alone !!**

## General Configuration
Option|Key|Value
---|:-:|:-:
Status LED GPIO|"l"|2
mDNS TTL|"ttl"|60
Setup Mode Toggle Count|"z"|60
Log Output|"o"|3
Invoke Setup Mode|"b"|GPIO 0<br>Hold for 8 seconds

## Accessory
Section|Key|Value
---|:-:|:-:
Service Type|"t"|75
Chip Type|"n"|1
Chip Data|"dt"|[GPIO 5, GPIO 4, GPIO 12]
Reading Period|"j"|1
Voltage Factor|"vf"|0.447090777
Current Factor|"cf"|0.010266694
Power Factor|"pf"|0.061005322

```JSON
{
	"c": {
		"l": 2,
		"ttl":60,
		"z":0,
		"o":3,
		"b": [
			{
				"g": 0,
				"t": 5
			}
		]
	},
	"a": [
		{
			"t": 75,
			"n": 1,
			"dt":[5,4,12],
			"j":1,
			"vf": 0.447090777,
			"cf": 0.010266694,
			"pf": 0.061005322
		}
	]
}
```
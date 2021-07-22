# Aquarium Controller

## General Configuration
Option|Key|Value
---|:-:|:-:
Status LED GPIO|"l"|13
mDNS TTL|"ttl"|60
Setup Mode Toggle Count|"z"|0
Invoke Setup Mode|"b"|{"GPIO": 0, "type": 5}

## Accessory 1 - Fish Feeder
Section|Key|Value
---|:-:|:-:
Maximum Use Time|"d"|1
Action 0|"0"|{"GPIO": 4}
Action 1|"1"|{"GPIO": 4, "value": 1, "inching": 0.3}
Digital Inputs|"b"|{"GPIO": 5, "type": 0}

## Accessory 2 - Light
Section|Key|Value
---|:-:|:-:
Action 0|"0"|{"GPIO": 14, "value": 1}
Action 1|"1"|{"GPIO": 14}
Digital Inputs|"b"|{"GPIO": 12, "type": 0}

```JSON
{
	"c":{
		"l":13,
		"ttl":60,
		"z":0,
		"b":[{
			"g":0,
			"t":5
		}]
	},
	"a":[{
			"d": 1,
			"0":{
				"r":[{
					"g":4
				}]
			},
			"1":{
				"r":[{
					"g":4,
					"v":1,
					"i":0.3
				}]
			},
			"b":[{
				"g":5,
				"t": 0
			}]
		},
		{
			"0":{
				"r":[{
					"g":14,
					"v":1
					}]
			},
			"1":{
				"r":[{
					"g":14
					}]
			},
			"b":[{
				"g":12,
				"t": 0
			}]
		}
	]
}
```
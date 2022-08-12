# Home Assistant NHL Card
A Home Assistant frontend custom card for the [ha-mlb](https://github.com/simplysynced/ha-mlb) integration.  This was originaly made by @D34DC3N73R for the NFL and can be found here [ha-nfl-card](https://github.com/D34DC3N73R/ha-nfl-card)

#### &nbsp;&nbsp;&nbsp;PREGAME


#### &nbsp;&nbsp;&nbsp;IN GAME


#### &nbsp;&nbsp;&nbsp;POSTGAME


#### &nbsp;&nbsp;&nbsp;POSTPONED




## HACS Installation
- In the HACS UI, click the 3 dots in the upper right
- Click 'Add Custom Repository'
- Fill in the repo url https://github.com/SimplySynced/ha-mlb-card and choose 'Lovelace' category.
- install the custom card
- Add the following to your resources
```
url: /hacsfiles/ha-nhl-card/ha-mlb-card.js
type: module
```

## Manual Installation
- Download [ha-mlb-card.js](https://raw.githubusercontent.com/SimplySynced/ha-mlb-card/main/dist/ha-mlb-card.js)
- Copy to www/community/ha-mlb-card/ (make the ha-mlb-card directory)
- Add the following to your resources
```
url: /hacsfiles/ha-mlb-card/ha-mlb-card.js
type: module
```

## Options
| Name | Description | Default | Required |  Values |
| --- | --- | --- | --- | --- |
| `entity` | Name of ha-mlb sensor | `sensor.nhl` | Yes  | Valid sensor |

## Minimal Required Configuration
```
type: 'custom:mlb-card'
entity: sensor.mlb
```
Where `sensor.mlb` is the sensor name from the [ha-mlb](https://github.com/simplysynced/ha-mlb) integration.
# PetKit blueprints

| Blueprint                         | What it does                                                                                                      |
| --------------------------------- | ----------------------------------------------------------------------------------------------------------------- |
| `fountain_drink_counter.yaml`     | Increments a counter on each off-to-on transition of the `Pet drinking` binary sensor, with optional daily reset. |
| `fountain_no_drinks_alert.yaml`   | Fires when the binary sensor has stayed `off` for X hours.                                                        |
| `fountain_low_drinks_alert.yaml`  | Fires once a day if today's count is below a percentage of the 7-day median.                                      |
| `fountain_high_drinks_alert.yaml` | Fires once a day if today's count is above a percentage of the 7-day median.                                      |

The alert blueprints depend on the counter blueprint and the companion
package YAML. See [`docs/automations.md`](../../../docs/automations.md) for
the full setup.

### Import

In Home Assistant: **Settings → Automations & Scenes → Blueprints →
Import Blueprint**, and paste the raw URL for the blueprint you want, e.g.:

```
https://github.com/Jezza34000/homeassistant_petkit/blob/main/blueprints/automation/petkit/fountain_drink_counter.yaml
```

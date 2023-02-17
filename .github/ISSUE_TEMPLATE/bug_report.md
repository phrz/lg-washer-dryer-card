---
name: Bug report
about: Create a report to help us improve
title: "[BUG] give a title"
labels: ''
assignees: ''

---

**Describe the bug**
A clear and concise description of what the bug is.

**What I have tried (required)**
- [ ] I checked what the entity name of my washer/dryer/machine is, and it either matches what's in the default configuration (i.e. `sensor.washer`, `sensor.dryer`) or, if it's different, I've modified both `configuration.yaml` and the Lovelace configuration for this card to make it match.
- [ ] My LG account is in English, and the state names returned by the LG ThinQ integration are in English, or I've gone through `configuration.yaml` and the Lovelace configuration to change the state tests to the appropriate state strings in my language.
- [ ] If my washer/dryer does not look like the one in the default card picture, I've checked that the state names returned by my machine matches the ones in the code, such as showing a hyphen (`'-'`) as the `run_state` entity value when the machine is not running.

**Screenshots**
If applicable, add screenshots to help explain your problem.

**Configuration**
```yaml
# Paste the washer/dryer portion of your configuration.yaml here.
```

```yaml
# Paste the Lovelace card code here.
```

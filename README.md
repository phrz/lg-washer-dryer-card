![IMG_1843 2](https://user-images.githubusercontent.com/2007088/112699616-35751b00-8e5a-11eb-9bf8-cc09af4847a9.PNG)
This repo is for Home Assistant users who want cards that look like their LG washer/dryer's physical displays. You'll need the LG ThinQ integration already installed.

# Installation (manual)
1. Where `config` is the location of your `configuration.yaml` file, create `config/www` if it does not already exist. Then place the contents from this repository's `config/www` into yours.
2. On your Lovelace dashboard, click the three dots in the top right, and select `Edit Dashboard`. Now click the three dots again, and click `Manage Resources`. Tap `Add Resource` in the bottom right, then enter `/local/7segment.css` and ensure the type is set to `Stylesheet`. Complete the entry.
3. Add the contents of this repository's `configuration.yaml` to your own. If you already have a template sensors entry like this, these sensors can be added alongside your other template sensors.
4. **Important:** rename `sensor.washer` to the entity ID of your LG Washer, `sensor.washer_run_state` to the corresponding Washer Run State sensor, `sensor.dryer` to your dryer, and `sensor.dryer_run_state` to the Dryer Run State sensor.
5. Now go to your desired Lovelace dashboard, go to `Edit Dashboard`, and add a Vertical Stack card. Enter the Code Editor and paste in the contents of either `washer-card.yaml` or `dryer-card.yaml`, depending on which one you want to insert.
6. _Optional:_ as written, these cards show a list of settings (temperature, cycle, etc.) underneath when the washer/dryer is running. If you don't want that, just remove the conditional card from the stack, or take the washer/dryer Picture Elements card out of the stack entirely and place it as its own card.

# Notes
7segment font (c) Jan Bobrowski (OFL) - http://torinak.com/7segment

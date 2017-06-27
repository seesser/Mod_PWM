# Mod_PWM
Modded GPIOPWM with Logic for CraftBeerPi 3.
### This Plugin is for CraftBeerPi 3
This is an add on for the CraftBeerPi 3 that is a modded form of the GPIOPWM. This Pugin makes it possible to run the Mod_PWM_Logic that adds power reduction and power ramp up to the GPIOPWM actor. Please set you heater actor the Mod_PWM and your kettle logic to Mod_PWM_Logic. 
# Mod_PWM_Logic
Power step down logic to the Mod_PWM actor with power ramp up.
### This Plugin is for CraftBeerPi 3 and only for Mod_PWM heater actor
This logic allows the user to pick a percent of power reduction of the currently set power setting.  This step down in power will start at a picked degee from target temp.  The Power level will automatically go back to it's full preselected power level when target temp is outside reduction temp reange.  There is also a ramp up feature that helps with amp draw from the heater.  This setting alows you to pick the percent of power the heater will increase in 1/10 sec cycles until at desired power level.
### Bug!
This logic and actor uses a shared varible for the power level.  Because of this all actors running Mod_PWM will share the same power level.

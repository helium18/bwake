<h1 align="center">bwake</h1>

![image](https://user-images.githubusercontent.com/86223025/164252138-fa2b0c67-a185-4961-abec-7a428497b2f9.png)

## Why ?
Using your laptop while it's charging is certainly not the best practise.

If your device doesn't support setting thresholds to limit the battery levels while charging and you're looking for something that serves a similar purpose, then you're at the right place.

## What it does
Estimates the time required to charge the battery to the given threshold (defaults to 80%). 

Then puts your device to sleep (it uses `rtcwake` behind the scenes). 

When the battery charges to the limit specified, the device is woken up and an alarm is played.

## Things to note
1. It's just an estimate, there's a 90% chance that it'll go above / below the threshold a bit ~ 5%-10%.
2. Consider running the script with `sudo`. (To avoid entering the password manually every time before the device is slept)
3. The alarm should be named `sound.ogg` and be placed in `$HOME`. An option to override this behavior will be provided in the future 

Feature requests and bug reports are welcome. 

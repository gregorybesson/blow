# Yet Another Blow Effect

Detect the blow of your user to create innovative interactions ;)

1. I've used the excellent https://github.com/mattdiamond/Recorderjs audio plugin from Matt Diamond.
2. I've added the PR from https://github.com/osondoar for managing callbacks
3. I've remembered an advice from Myles Borins (https://github.com/TheAlphaNerd) while we were working on a cool demo based on https://github.com/famous. His advice was to apply a basic low-pass filter to a gyroscope + socketjs + famo.us stuff (http://www.dspguide.com/ch19/2.htm)

Myles Borins quote:
> basically you have current state, input, and a co-efficient
> `current state = current state * co + input * 1 -  co`

This advice could be applied to the microphone captation : If I apply this filter and verify that it is satisfied during a sufficent amount of time, I can conclude that the user is blowing in his Mic !

Of course, if the sound you produce is stable enough, you'll be able to trigger the blow event. 

To be continued. Don't hesitate to criticize and / or improve it !

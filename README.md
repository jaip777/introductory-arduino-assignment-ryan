# introductory-arduino-assignment-ryan
introductory-arduino-assignment-ryan created by GitHub Classroom

# GROUP MEMBERS: Ryan, Alex, Jai

# Log 1 : November 8th 2017

Up to this point, we have done a lot of work on this arduino assignment, but also encountered many issues.
From the get-go, we easily set up our board, but had several issues with it since our board was not running as it should with the code that we were uploading. We had initially thought that there were issues with the wiring, since if we held the wires in certain poistions as we pressed the button, it would work normally. However, if we were not holding the wire in that certain position, it would not work when we pressed the button. 

With the help of M. Reynolds, we went through the code that we were uploading had faults in it, and we quickly fixed those and got the button to work properly. Since then, our major focus has been trying to figure out how to get the light to stay off on default, and then turn on when we press and hold the button, as opposed to its current state where it's default is on, and the light turns off when we press the button. This has proved to be more difficult than we had initally thought it would be, due to the fact that the code that we had thought would work proved to be insignificant in changing the results. Nevertheless, we are continuing to try and accomplish this goal, and will hopefully find a way to get it to work. 

# Log 2 : November 15th 2017

We figured it out! As mentionned in our previous log, our main goal was to figure out a way to have the light start Off as its default state, and then turn on when the button is pressed. Initially, the light started on, by default, and then would turn off when we pressed the button. However, today, we found a way to have it start off by default! We went into the code, and we put an ! in front of "LED State", in the line: 'digitalWrite(LEDpin, LEDstate);', so that now it looks like this: 'digitalWrite(LEDpin, !LEDstate);'. This solution worked, and we now have our desired results. However, occasionally, it will not work, or it works with a delay. Our next steps are to fix this so that it works properly every time by figuring out the debounce code.

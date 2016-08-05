# MTurk2Limesurvey

When I went to set up a study using MTurk and Limesurvey I didn't immediately find a solution to pass a workerID from Mechanical Turk to prefill an answer in a Limesurvey question. This is useful to do in order to only pay those who completed the task appropriately. 

A solution for surveys hosted on Qualtrix can be found [here](http://sapir.psych.wisc.edu/wiki/index.php/MTurk). The current code adapts this to work with Limesurvey. NB the question can be set to invisible in Limesurvey so that the participant cannot change the captured workerID.

The comments in the .html file should (hopefully) explain how to customise the code for your own use.

The generated HIT page is extremely simple:

![alt text](https://github.com/ianhussey/MTurk2Limesurvey/blob/master/Screenshot.png "Screenshot")



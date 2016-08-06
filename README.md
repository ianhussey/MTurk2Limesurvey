# MTurk2Limesurvey

### Description 
When I went to set up a study using MTurk and Limesurvey I didn't immediately find a solution to pass a workerID from Mechanical Turk to prefill an answer in a Limesurvey question. This is useful to do in order to only pay those who completed the task appropriately. 

A solution for surveys hosted on Qualtrix can be found [here](http://sapir.psych.wisc.edu/wiki/index.php/MTurk). The current code adapts this to work with Limesurvey. NB the question can be set to invisible in Limesurvey so that the participant cannot change the captured workerID.

This code passes html5 validation using https://validator.w3.org, and as such can generate an AMT Layout ID. 

### Usage
This code should be placed in the AMT requester web interface under `Create>Edit project>Design layout>Source`.

The location of your specific limesurvey installation and the question that is to be prefilled must be specified. Limesurvey answer prefill URLs take the format `https://www.example.com/index.php/survey/index/sid/STUDY_ID_HERE]/newtest/Y?[STUDY_ID_HERE]X[QUESTION_GROUP_ID_HERE]X[QUESTION_ID_HERE]=gelb&amp;[STUDY_ID_HERE]X[QUESTION_GROUP_ID_HERE]X[QUESTION_ID_HERE]=[PREFILLED_ANSWER_HERE]`

- e.g. `https://www.limey.ugent.be/LIPLAB/index.php/survey/index/sid/111111/newtest/Y?111111X111X1111=gelb&amp;111111X111X1111=test`

- See <https://manual.limesurvey.org/Workarounds:_Survey_behaviour#Prefilling_survey_answers_using_the_survey_URL>

The generated HIT page is extremely simple:

![alt text](https://github.com/ianhussey/MTurk2Limesurvey/blob/master/Screenshot.png "Screenshot")





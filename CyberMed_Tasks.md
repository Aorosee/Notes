# CYBERMED TASK LIST
>Last Changes: 5/4/2020 </br>

## CURRENT WORKING ON (Priority first)</br>
* Reviewing codes and making them more simple. </br>
* Complete a video session work-flow. </br>
</br>

## REVIEWING </br>
</br>

## ISSUES & FEATURES </br>
**5/4/2020:** </br>
* Change success/fail words to green/red spots. </br>
* Implement patient's online status and device status to webservice. </br>
* Delete 'close camera' button & delete 'Chrome is better' sentence. </br>
* Check the internet connection speed if I can. Optional </br>
* Detect if user is using mobile or pc. Optional </br>
</br>

**5/1/2020:** </br>
* Modify the outcome of PatientWaitingRoom.aspx. </br>
* Implement the hardware check and connection checks. </br>
* Modify the video session sidebar outcome. </br>
* Re-design the QA site database management. </br>
</br>

**4/16/2020:** </br>
* Refreshing the page will not resume provider's call. </br>
* <s>When provider cancel the outgoing ringbox as soon as the ringbox just showing up, then the cancel button only dismiss the ringbox but the calling percedure is still on.</s> </br>
</br>

**4/15/2020:** </br>
* <s>Don't show callback option on appointment which comes from yesterday or earlier. OR pop-up warn provider do not use past or future appointment.</s> </br>
</br>

**4/14/2020:** </br>
* A weird issue. Provider get a same room_number ringbox 30 mins after video call.</br>
* Help MJ to refine the video layout in order to suit mobile version. </br>
* <s>If patient is busy or offline, the outgoing would not still show and never dismiss.</s> </br>
* <s>Two timers stand together.</s> </br>
</br>

**4/13/2020:** </br>
* Complete a video session work-flow. </br>
* Reviewing codes and making them more simple. </br>
* Layout problem in CyberMed Corp website. </br>
* <s>When provider missed call, it should not block another call come in.</s> </br>
* <s>Complete the first test percedue of CDOC_ONLINE.</s> </br>
</br>

**4/10/2020:** </br>
* Provider could read Room db table first before patient clean them. </br>
* <s>Provider Radwin should show "patient has leave" when patient hangup before/right after provider pick up.</s> </br>
</br>

**4/9/2020:** </br> 
* Patient call provider will mark Room table's caller and receiver as a same type (pat to pat). (NEED to be REPRODUCE) </br>
* <s>Console log may expose room informations, such as appId and room_number and uid.</s> </br>
* <s>Missed Call doesn't go to MISSED section.</s> </br>
* <s>Incoming Box show again after a normal flow start from provider callback to patient.</s> </br>

**4/8/2020:** </br> 
* <s>Pat -> provider, pat hang-up right before provider accepts. Provider has video. Provider hangs up. Still online status 2.</s>  </br>
* <s>Patient leave should notify provider.</s>  </br>
* <s>Provider normal leave ok. Provider calling cancel button leave does not have end time.</s> </br>
* <s>Patient -> Provider. Patient end call. Provider end call. Calling screen call again. --> Provider online_room must be NULL. (If “” then the calling screen will popup again).</s>  </br>
* <s>“This Party currently is busy or offline” -> “The other party is currently busy or offline, please try again later”.</s> </br>
* <s>Two Register_as_room_guest functions inside the Webservice.</s> </br>
* <s>Patient hangup, provider online status is 1??</s>   </br>
* <s>Patient left. Provider still on video. However, provider end_time marked.</s>  </br>
* <s>Complete window not opened when patient hang up.</s>  </br>
</br>

## DONE </br>
* `BRANCH issueFix` Provider web call patients needs to set self online room number (in provider table). **MERGED**</br>
* `BRANCH issueFix` “This Party currently is busy or offline” -> “The other party is currently busy or offline, please try again later”.  **MERGED** </br>
* `BRANCH issueFix` Two Register_as_room_guest functions inside the Webservice.  **MERGED** </br>
* `BRANCH issueFix` Patient hangup, provider online status is 1??  **MERGED** </br>
* `BRANCH issueFix` Patient left. Provider still on video. However, provider end_time marked.  **MERGED** </br>
* `BRANCH issueFix` Complete window not opened when patient hang up.  **MERGED**  </br>
* `BRANCH issueFix` Provider normal leave ok. Provider calling cancel button leave does not have end time.  **MERGED** </br>
* `BRANCH issueFix` Patient -> Provider. Patient end call. Provider end call. Calling screen call again. --> Provider online_room must be NULL. (If “” then the calling screen will popup again).  **MERGED** </br>
* `BRANCH issueFix` Incoming Box show again after a normal flow start from provider callback to patient.  **MERGED** </br>
* `BRANCH issueFix` Patient leave should notify provider.  **MERGED** </br>
* `BRANCH issueFix` Pat -> provider, pat hang-up right before provider accepts. Provider has video. Provider hangs up. Still online status 2.  **MERGED** </br>
* `BRANCH refineCodes` Console log may expose room informations, such as appId and room_number and uid.  **MERGED** </br>
* `BRANCH twoTimers` Two timers stand together.  **MERGED** </br>
* Complete the first test percedue of CDOC_ONLINE. </br>
* `BRANCH fridayChange` Don't show callback option on appointment which comes from past or future. **COMMITED** </br>
* `BRANCH fridayChange` Provider Radwin should show "patient has leave" when patient hangup before/right after provider pick up. **COMMITED** </br>
* `BRANCH fridayChange` When provider cancel the outgoing ringbox as soon as the ringbox just showing up, then the cancel button only dismiss the ringbox but the calling percedure is still on. **COMMITED** </br>
* `BRANCH fridayChange` If patient is busy or offline, the outgoing would not still show and never dismiss. **COMMITED** </br>
</br>
* `BRANCH fridayChange` When provider missed call, it should not block another call come in. **COMMITED** </br>

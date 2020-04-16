# CYBERMED TASK LIST
>Last Changes: 4/16/2020 </br>

## CURRENT WORKING ON (Priority first)</br>
* Provider Radwin should show "patient has leave" when patient hangup before/right after provider pick up. </br>
* Don't show callback option on appointment which comes from yesterday or earlier. </br>
* Provider could read Room db table first before patient clean them. </br>
* Complete the test percedue of CDOC_ONLINE. </br>
* Complete a video session work-flow. </br>
* Reviewing codes and making them more simple. </br>
</br>

## REVIEWING </br>
</br>

## ISSUES & FEATURES </br>
**4/15/2020:** </br>
* Don't show callback option on appointment which comes from yesterday or earlier. </br>
</br>

**4/14/2020:** </br>
* If patient is busy or offline, the outgoing ringbox would not timeout. </br>
* A weird issue. Provider get a same room_number ringbox 30 mins after video call.</br>
* Help MJ to refine the video layout in order to suit mobile version. </br>
* <s>Two timers stand together.</s> </br>
</br>

**4/13/2020:** </br>
* Complete a video session work-flow. </br>
* Complete the test percedue of CDOC_ONLINE. </br>
* Reviewing codes and making them more simple. </br>
* When provider missed call, it should not block another call come in. </br>
* Layout problem in CyberMed Corp website. </br>
</br>

**4/10/2020:** </br>
* Provider could read Room db table first before patient clean them. </br>
* Provider Radwin should show "patient has leave" when patient hangup before/right after provider pick up. </br>
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
</br>

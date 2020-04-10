# CYBERMED TASK LIST
>Last Changes: 4/10/2020 </br>

## CURRENT WORKING ON </br>
* Console log may expose room informations, such as appId and room_number. </br>
</br>

## REVIEWING </br>
</br>

## ISSUES & FEATURES </br>
**4/9/2020:** </br> 
* Console log may expose room informations, such as appId and room_number. </br>
* Patient call provider will mark Room table's caller and receiver as a same type (pat to pat). </br>
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
* `BRANCH issueFix` Provider web call patients needs to set self online room number (in provider table). **PUSHED**</br>
* `BRANCH issueFix` “This Party currently is busy or offline” -> “The other party is currently busy or offline, please try again later”.  **PUSHED** </br>
* `BRANCH issueFix` Two Register_as_room_guest functions inside the Webservice.  **PUSHED** </br>
* `BRANCH issueFix` Patient hangup, provider online status is 1??  **PUSHED** </br>
* `BRANCH issueFix` Patient left. Provider still on video. However, provider end_time marked.  **PUSHED** </br>
* `BRANCH issueFix` Complete window not opened when patient hang up.  **PUSHED**  </br>
* `BRANCH issueFix` Provider normal leave ok. Provider calling cancel button leave does not have end time.  **COMMITED** </br>
* `BRANCH issueFix` Patient -> Provider. Patient end call. Provider end call. Calling screen call again. --> Provider online_room must be NULL. (If “” then the calling screen will popup again).  **COMMITED** </br>
* `BRANCH issueFix` Incoming Box show again after a normal flow start from provider callback to patient.  **COMMITED** </br>
* `BRANCH issueFix` Patient leave should notify provider.  **COMMITED** </br>
* `BRANCH issueFix` Pat -> provider, pat hang-up right before provider accepts. Provider has video. Provider hangs up. Still online status 2.  **COMMITED** </br>
</br>

This folder contains a copy of the FFXIV_ACT_Plugin ability & status definition JSON files as of version 2.6.3.8, for FFXIV Patch 6.05.  

These files adhere to the following json structure:
"job": descriptive string of the job suppored by this data.  The job name is arbitrary.
"actions": an array of action definitions, each entry starting with a key representing the action id in hex. 
"statuseffects": an array of status effect defintions, each entry starting with a key representing the status id in hex.

Actions support the following nodes:
"damage": zero or more instances that indicate different variations of damage done by the action.  Acceptable fields are:
  "potency": the potency for the damage entry
  "combo": the 'combo' potency for the damage entry
  "targetindex": the target index this damage applies to.  This allows variations of damage for the initial target vs additional targets
"heal": zero or more instances that indicate different varitions of heals done by the action.  Acceptable fields are:
  "potency": the potency for the heal entry
  "targetindex": the target index this heal applies to.  Similar behavior as for the damage entry's target index field.
  
Status effects support the following nodes:
"potency": zero or more instances that indicate the following types of potency multipliers (TBD)
"timeproc": zero or one instance that indicates a DoT, HoT, or ground effect
"multiplier": zero or more instances that indicate a critical or direct hit effect multiplier
"damageshield": zero or one instance that indicates how to simulate a damage shield
"reactiveproc": zero or one instance that indicates the presence of reactive damage or heals

  

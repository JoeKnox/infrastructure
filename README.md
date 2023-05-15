# infrastructure
just building something for the house

This is my learning project:
1. Design my network to include practical and main devices/computers, a second one for IoT, and a third to contain things that I am trying to make and break.

2.  This is also my attempt at making myself document and track things.  Getting used to writing as well.   


05/02/23- designed a base format of goals and objectives and first iteration software.

05/04/23- used go.gliffy.com (free trial version)to design the hardware and layout and todo list see network map(red-things that need done, purple-kthings that I need to learn)

5/06/23  6:30 AM Began moving the hardware from its basement location to the lab and rerouting all of the cable.   Recycled, trimmed, rerouted and terminated a all cables and cleaned up the routes/lines.  Fully tested prior to cleaning up the cable routes and paths.  One issue with connection of megans desktop computer.  It showed no internet connectivity until a google search was committed and then it came right back on-line. Ready for reallocation of resources 9:30 AM 

5/07/23  After using the Linux provided by Raspberry Pi for a day, I switched to Kali Linux.
  -this brings the OS inventory to 
    -1 desktop windows 11 (various virtual machines)
    -1 desktop dual boot Ubuntu/windows 10
    -1 Raspberry Pi - Kali Linux
    -1 Raspberry Pi - Debian
    -1 Tablet Windows 10
    
 5/13/23 4:30AM- Woke up early to work on school projects. The internet was not working.  little pieces would get through every 20 minutes or so but not enough to work.  I went through the normal process of restarts.  No success.  I began trying to diagnose if it was computer, network, bridge or ISP  issues... First I started with pinging the router from my computer. GOOD (not the computer signal).  then Ping across the subent to another Device GOOD (router good).  Pinged to another subnet GOOD.(load balancer good)   Ping the Bridge/Modem  GOOD (Probably not the Bridge/Modem).  Checked out the bridge logs to find that the bridge was reporting a DoS attack "Smurf"  Which seems unlikely and after an internet search says that that is a tendency of netgear to give false positives on DoS attacks.  Leads me to Signal from ISP. 

5/13/23 5:30PM   through out the day the situation had improved. Noticably by 1:00PM after the rain had stopped for 2 hours.  by 5:30 PM we realize we have reliable service.  This makes me begin to wonder if the signal cable isnt being compromised by water

5/13/23 9:30PM   Service become flakey again.  (Began to Rain lightly)   

5/14/23  5:30 AM  No internet service.   The ground is very wet.   Contact Spectrum through Phone Chat.  ("Something suspicious on the line")

5/14/23  4:30 PM   Service tech confirms that it is the signal into the house.  He confirms the issue at the pole.  Diagnosis "There is a reflection of the signal down the line like a refelction from water" Schedules maintainence to fix the line.

5/15/23  5:30 PM   no sign of rain, nor maintenance.... but signal appears to be holding 


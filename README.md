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

5/20/23  Setting up Linux Firewalls and emails
        -could not get data in or out despite allowing Ports 443, 80, and 25 on UFW firewall when UFW was enabled.   Also had issues with the screen blacking out once UFW was installed.  (see Photos)

5/23/23 No luck   Reached out to school instructors as the firewall unit was what we were working on.  No response.

5/31/23 finally returning to project
  -removed GPU and using motherboard's GPU-Stable
  -specifically had to call out to allow outgoing http, tcp, https and smtp protocols in UFW firewall to allow use of internet and email.
 
6/5/23   
  -TP-link (ER605) firewall/load balancer/switch device.  
  -On friday night there was a substantial power surge that was enough to trip breakers and GFCI's  (I think more voltage leaked to the ground more so than surge but moot point) .  In the morning I did not have internet service.  All of the lights on all of the bridge/modems/routers showed that it should be fine.
  -Instead of a hard reset I sat at the computer and tried to log into the modem to reset it.  I could not ping it 
  -I pinged the firewall.   its there.  I replugged around the firewall box to the modem.  internet works fine.   
  -change to the original configuration and open Chrome to log into the firewall box.  Change some settings/restart it.   cannot get data through the box. and it said that the "dhcp link [was] down".  after hours of trying the same things just different ways.  
  -I concede it must be the physical firewall box,  and I go buy a new one.   
  -I put it in and out of the box, it works fine. I go to login to setup a mirrored port for my monitoring and.... its dies... same situation as hours ago...restarts, internet searching (bypassing the physical firewall), thinking it was my computer, even though nothing else was connecting to the internet... 
  -nothing works. I shut everything down and go to bed, wake up sunday, start everything up.  
  -Open up FIREFOX  and login to the firewall box and everything works perfectly fine and I can make changes.  
  -I already have chrome up so I tried to login and make a couple of changes to the firewall-everything dies-
  -immediately, bring up firefox, log in and everything is restored to working order.  
  -after a total of about 6 or so hours of struggle, all that I needed to do was try a different browser.  IDK pretty remedial but maybe file that away as something when nothing makes sense. 

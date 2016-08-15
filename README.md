##Two stand-alone utility applications...

###Disclaimer
In early 2014 I decided to use my own recognizance to 1) learn a little VB.NET and 2) apply said knowledge to make my life as a software support technician a bit easier.

Written in early 2014, they are apparently still being used by the Apple Engineers that just so happened to stumble upon their use while I was seemingly less busy doing more enjoyable things.  And with that said, NDA redactions ahoy!

###Behold! The FolderMonitoringTool...

![](images/FolderMonitoringTool_main.jpg)

![](images/FolderMonitoringTool_options.jpg)

###...which I just now renamed to *Meerkat Tunneling Application*

It is state-of-the-art manufacturing facility, and their SMT (surface mount technology) database generates .xml files to pass information from one machine / process to the next.  At the end of each procedure, if all is well, those .xml files are then parsed back into the database. If all did not go well, those files either bottleneck at the process where the error occurs or, even worse, populates the database with incorrect data.

After spending a few days manually opening 30 different remote directories and keeping a constant eye on them, I decided to automate that process. The result is this application, which monitors any directory specified by the user, throwing visual alerts should any specified thresholds occur.

---

###Behold! The RemoteServicesManager

![](images/RemoteServicesControl.jpg)

Several times a day, certain server-based processes would get hung and need to be remotely restarted.  The process was easy enough, but it took longer than I thought it should (firing up the virtual machine, network latency, etc.).  Plus, if there were too many people logged into said server you had to find out who was logged in and then ask them to log out (if they were done doing whatever it was that they were doing).  So, to alleviate my frustrations, and also for kicks, I decided to see what I could do.

This application allows the user to start and stop services from a list of user-specifed remote servers, as well as view the last 100 errors related to each service.  So, instead of taking 5 minutes to restart a service, it now takes 20 seconds.  And, as an added bonus, it also bypasses the user limit, allowing access as long as the user had access right via Active Directory.


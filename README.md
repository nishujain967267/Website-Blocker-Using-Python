# Website-Blocker-Using-Python
This is real world program which blocks certain distracting website like Facebook, Youtube etc during your work hours.

About the program : What we are going to in this program is that we will pass the link of websites which you think is distracting and the time that you are working on your computer and program will block those website.


Every system have host file whether it is Mac, Windows or Linux.
Host file in Mac and Linux :
/etc/hosts
Host file in Windows:

C:\Windows\System32\drivers\etc
Working of host file: Host is an operating system file which maps hostnames to IP addresses. In this program we will be mapping hostnames of websites to our localhost address. Using python file handling manipulation we will write the hostname in hosts.txt and remove the lines after your working hours.
Host file in Mac:



Special note for Windows users : Windows user need to create a duplicate of OS’s host file. Now provide the path of the duplicate file in hosts_path mentioned in the script.

Scheduling above script in Mac : For scheduling above script in Mac you have to open crontab in your terminal as a root.

Write following command in terminal:
sudo crontab -e


Now press “i” to go into insert/editing mode and write @reboot python_script_path .
Save the tab by pressing first esc to quit write mode and fall back to command mode and now write “:wq” and finally press enter to validate.
Restart your system and see the magic.
Scheduling in Windows: Scheduling of above script is little bit trick but I will guide you step by step-

First of all change the extension of your script from “.py” to “.pyw”.
You may see website blocker already scheduled because I have already scheduled in my computer for my testing purpose. Follow further instruction of scheduling carefully in order to schedule website blocker in your computer.

Click on “create task”. Fill the name of your choice and flag “Run with highest privilege”.
Now go to triggers, select “At startup” for begin the taskGo to Action bar and create a new action and give path of your script.
Go to conditions bar and unflag the power sectionPress ok and you can see the script scheduled.
Finally restart your computer and see the magic.
Note: You can also check instantly by clicking run button.

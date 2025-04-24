# Metasploit-for-reconnaissance

### Developed By : SANJAY M
### Register No  : 212223230187

# Metasploit
Metasploit for reconnaissance in pentesting

# AIM:

To get introduced to Metasploit Framework and to  perform reconnaissance  in pentesting .

## DESIGN STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode

### Step 2:

Investigate on the various categories of tools as follows:

### Step 3:

Open terminal and try execute some kali linux commands

## EXECUTION STEPS AND ITS OUTPUT:


Find out the ip address of the attackers system



## OUTPUT:


![{609553AC-8064-4429-BE0F-EAF8564E0D2B}](https://github.com/user-attachments/assets/7dbba18b-8662-4763-88ca-dae2e4dbedbf)



Invoke msfconsole:



## OUTPUT:


![{37C0E04D-F449-4A56-8CE6-3402271196B3}](https://github.com/user-attachments/assets/6713fe52-dbcb-45fc-b1ce-29ca79916e0b)



Type help or a question mark "?" to see the list of all available commands you can use inside msfconsole.


![{20083162-63EE-46AB-9E7A-F9E641A3882E}](https://github.com/user-attachments/assets/ae7648a6-04ee-419a-9599-f7938a9550d2)


Port Scanning:


Following command is executed for scanning the systems on our local area network with a TCP scan (-sT) looking for open ports between 1 and 1000 (-p1-1000).


msf >  nmap -sT 192.168.1810/24 -p1-1000


![{95BDBC09-D7D7-4A9D-818D-09340D7F9570}](https://github.com/user-attachments/assets/22fc1965-d58b-480a-8521-a72a89df6762)


step4:
use the db-nmap command to scan and save the results into Metasploit's postgresql attached database. In that way, you can use those results in the exploitation stage later.

scan the targets with the command db_nmap as follows.


msf > db_nmap 192.168.181.0/24


![image](https://github.com/user-attachments/assets/02da64eb-1bd6-419f-a3b1-b5c9032f6eba)


Metasploit has a multitude of scanning modules built in. If we open another terminal, we can navigate to 

Metasploit's auxiliary modules and list all the scanner modules.


cd /usr/share /metasploit-framework/modules/auxiliary


kali > ls -l

![{1C4282F6-43A8-4842-817C-AFF4A7BE3A66}](https://github.com/user-attachments/assets/e07d1243-fb80-49d9-99b5-404cf974e644)


Search is a powerful command in Metasploit that you can use to find what you want to locate. 


msf >search name:Microsoft type:exploit


![{17F661AA-C9BE-441A-88AC-DFF4985DBFF6}](https://github.com/user-attachments/assets/be2feed2-8991-4db2-97b5-eaedad3d6c9f)


search type:auxiliary mysql


![image](https://github.com/user-attachments/assets/f057c773-0743-462f-9d52-c169da173a59)



search type:auxiliary mysql


![{D65E284A-664C-4F77-9AF7-1D73E854FAB1}](https://github.com/user-attachments/assets/760c8927-db15-4207-9f00-fd797e146eaf)


use 11


![{BBB12364-3F3C-4A90-A678-7D0123C840B9}](https://github.com/user-attachments/assets/ada6edb1-dbb6-4ebb-b024-8c2cd832b0cc)


set RHOSTS <IP>


![{0B1BD85A-9A9D-4FCC-A14C-3A1CE5DF4795}](https://github.com/user-attachments/assets/cc519e5d-d2b6-4cd0-8848-b1e2a6b5fe91)


use auxiliary/scanner/mysql/mysql_login


![{F2A6D54D-69AB-4F2E-AC1E-56BC353C6175}](https://github.com/user-attachments/assets/9d26212c-b7fd-40de-b92b-595f8b24aecf)


set PASS_FILE /usr/share/wordlists/rockyou.txt


set RHOSTS <metasploitable-ip-address>


set BLANK_PASSWORDS true


set verbose no


run


![image](https://github.com/user-attachments/assets/eb780a66-e1eb-4f0f-add0-fd7f72e4be7e)

## RESULT:
The Metasploit framework for reconnaissance is  examined successfully

# Docker-Windows-10-Home
Docker Install in Windows 10 Home
## how to install docker on windows home?
## the easy way to install docker on windows home edition
### Prerequisite
  * [x] Enable Virtualization in BIOS
  * [x] Active Internet Connection
### update may 2020 - the simple solution is simply subscribe to windows insider program and to get the next version of windows home the include out of the box hyper-v and wsl2. 

### Steps
  1. Download or Clone This Repo [Click Here](https://github.com/MaxySpark/Docker-Windows-10-Home/archive/master.zip)
  2. Extract The ZIP File
  3. Right click on the `hyperV.bat` file and **_Run as Administrator_**  
  4. __*Restart*__ the Computer
  5. Right click on the `container.bat` file and **_Run as Administrator_**
  6. __*Restart*__ the Computer
  7. Open the `docker.reg` file or Right click and **_Merge_** (_Registry Values will be automatically reverted to its original values after a restart_)
  __*after version 2.3*__ docker windows installation checks your windows version . so you need to manipulate it
  Change in \HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion :
  EditionID: Core --> Professional
  ProductName: Windows 10 Home --> Windows 10 Pro
  (Not sure “ProductName” it’s necessary, I think only the “EditionID” key is used)
  __*After installing docker, remember to restore the original keys !!!*__

  8. Download the Docker Desktop installer [Click Here](https://download.docker.com/win/stable/Docker%20for%20Windows%20Installer.exe)
  9. Install it
  10. Bingo _**Docker**_ is Ready to Use
  
### NB: Before Step 9 Don't Forget To Run Step 7
 
Reference : [Docker Forum](https://forums.docker.com/t/installing-docker-on-windows-10-home/11722)
  

# LView League of Legends Script 
# PATCHED 11.22 !!!
What is this
LView is a python based scripting platform for League of Legends. The engine is external that means it is not injected into leagues process. The engine is running in a separate process and reads the games state using ReadProcessMemory.

# Building

You need Visual Studio 2019 to compile this.
  1. You need to install python 3.9 for 32bits (Make sure you check the Add to PATH checkbox in the installer: https://www.python.org/ftp/python/3.9.0/python-3.9.0.exe)
  2. directx 11: Must install directx end user runtimes: https://www.microsoft.com/en-us/download/details.aspx?id=35 .Extract this and run dxsetup
  3. boost::python. Due to the size of the boost libraries you must download boost yourself:
      1. Download boost 1.75.0 (https://www.boost.org/users/history/version_1_75_0.html) 
      2. Download boost 1.75.0 alternative: https://mega.nz/file/UB5SCLaK#F1RsqfctCn2rzH_xVqwE3l224u550SmmHg62xiueKp0
      3. Unarchive it in LView/boost
  !IMPORTANT! 
  Open up VS Command Prompt with Admin permission.
  
  Type: cd C:\Lview\Boost (change it to your path / boost folder) bootstrap 
  
  wait few seconds and type: 
  
  .\b2
  
  Wait for it to fully install.
  
  
  
  
  4. Open Visual Studio (Release x86) right click on the Project -> Properties.
  
  Search for VC++ Directories
  
  INCLUDE Path: C:\LView\boost\ (your boost folder)
  
  LIBRARY Path: C:\LView\boost\stage\lib\ (your boost\stage\lib folder)
  
  Save and Build
  7. Copy Release/ConsoleApplication.exe to LView/ConsoleApplication.exe
  8. Into the LView Folder you'll find config.ini file open with editor and edit:  `::scriptsFolder=\<folder\>`
  10. Run LView/ConsoleApplication.exe and have fun!

  
![Screenshot](https://i.imgur.com/IK9SxKd.png)

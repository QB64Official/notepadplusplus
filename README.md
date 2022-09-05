# QB64 language files for NotePad++ v.8.4 64bits

First Edition by PauloAstro at 14 August 2022. 
Last reviewed at 29 Aug 2022.


0) Introduction.
1) Language files installation.
2) Config NotePad++ to use F5 key to compile .bas files and execute your  .exe file
3) Version History.



## 0. Introduction.

If you are new to NotePad++ (NP++) or just want to test QB64 code files in a modern App in Windows just download the last Portable edition
of NP++ (v.8.4.4) and copy the files as described in '1.'.

If you would like to add the QB64 configurations files to your present Notepad++ installation you will have to edit manually your config files of Notepad++ 
and add the extra information inside overrideMap.xml and shortcuts.xml on this files pack.



## 1. Language files installation 
**1.1.** Copy qb64_UDL_DarkMode_vX.XXX.xml to the 'userDefineLangs' folder. This file can also be added manually from inside NP++ at:
     Menu-Languages -> User Defined Language -> Define your Language -> Click 'Import...'
     
**1.2.** Copy QB64FList.xml to the 'functionList' folder of NP++.

**1.3.** Copy overrideMap.xml to the 'functionList' folder or if you have more than one UDL FunctionList rules, just edit the present overrideMap.xml file by adding the following code line:
     
    <association id="QB64FList.xml" userDefinedLangName="QB64"/>

as explained inside the overrideMap.xml file.

**1.4.** Copy config.xml to the main folder of NP++, and replace the existing one.



## 2. Config NotePad++ to use F5 key to compile .bas files and execute your .exe file  

**2.1.** Copy QB64_noIDE.exe to your QB64 folder, aside with QB64.exe.

**2.2.** Configure manually windows 10 to open all .bas files with QB64_noIDE.exe, selecting the "Open With.." option for any .bas file.

**2.3.** Install the "RunMe" plugin on NP++ at Menu-Plugins -> Plugins Admin ->, and restart it after installation.

**2.4.** On NP++ Menu-Settings -> Shortcut Mapper -> 'Plugin commands' menu, and on 'Filter' enter 'Run' and change the shortcut key of 
     'Shell execute current file' to F5. And click 'Close'.	
      Now when pressing F5 it will compile the active NP++ document with QB64_noIDE.exe.

**2.5.** If you are editing a .bas file and if after pressing F5 for compilation you pretend to run your .exe file (a lot of times): 
     go to Menu-Run -> Run -> Select your [file_name].exe file inside QB64 folder and click 'save' to add it to the Run Menu Apps.
     Now you can edit/add a shortcut key to run your executable file.



## 3. Version History  
			

Rev.0.2 - 27 Aug 2022.
- Added Macro to insert Line Coments (only works when selecting the entire line or more). 
- Added Macro to remove Line Coments (only works when selecting the entire line or more). 
(Macros are saved at shortcuts.xml file)		
- Updated QB64FList.xml (see file for updates history)		
- Added new qb64_UDL_DarkMode_v0.003.xml for DarkMode color Preferences.
- added config.xml - file with more NP++ colours configuration for DarkMode use. 
		
		
Rev.0.1 - 20 Aug 2022.
- Updated UDL to qb64_UDL_v0.002.xml
	
Rev.0.0 - 15 Aug 2022.

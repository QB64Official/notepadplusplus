*****************************************************************
*																*
*         QB64 language files for NotePad++ v.8.4.4 64bits		*
*																*
*																*
*****************************************************************


First Edition by PauloAstro at 14 August 2022. 
Last reviewed at 27 Aug 2022.


0) Introduction.
1) Language files installation.
2) Config NotePad++ to use F5 key to compile .bas files and execute your  .exe file
3) Version History.
		
0) Introduction --------------------------------------------------------

If you are new to NotePad++ (NP++) or just want to test QB64 code files in a modern App in Windows just download the last Portable edition
of NP++ (v.8.4.4) and copy the files as described in '1)'.

If you would like to add the QB64 configurations files to your present Notepad++ installation you will have to edit manually your config files of Notepad++ 
and add the extra information inside overrideMap.xml and shortcuts.xml on this files pack.

This QB64 language implementation on NotePad++ (v.8.4.4, 64bits) Portable edition uses only 5 configuration files (.xml) to be copied to the NP++ folders:

	1 - qb64_UDL_DarkMode_vX.XXX.xml - file that holds the language keywords and rules based on the User Design Language interface for NP++.
		The "DarkMode" file should be used when using the DarkMode on NP++. The colors are similar to the QB64 Original IDE.
	2 - QB64FList.xml - file that holds the rules to identify the FUNCTION, SUB and TYPE used on .bas .bi and .bm files for the QB64 language.
	3 - overrideMap.xml - Add only one configuration line (<association id="QB64FList.xml" userDefinedLangName="QB64"/>) that tells NP++ the FunctionList rules
		to be used for QB64 user defined Language (UDL).
	4 - shortcuts.xml - file with the 2 macros to use Ctrl+R to add comments and Ctrl+Shift+R to remove them, but only works when selecting one
		entire line or more. 
	5 - config.xml - file with more NP++ colours configuration to use with qb64_UDL_DarkMode_vX.XXX.xml keywords configuration file.
	6 - qb64_noIDE.exe is not a NP++ config file but just a version of QB64.exe (v2.0.2) without the QB64 IDE, so that compilation can
		happen easier in NP++
		
		

1) Language files installation -----------------------------------------

	1.1) Copy qb64_UDL_DarkMode_vX.XXX.xml to the 'userDefineLangs' folder. This file can also be added manually from inside NP++ at:
		 Menu-Languages -> User Defined Language -> Define your Language -> Click 'Import...'
	1.2) Copy QB64FList.xml to the 'functionList' folder of NP++.
	1.3) Copy overrideMap.xml to the 'functionList' folder or if you have more than one UDL FunctionList rules, just edit the present overrideMap.xml file
		 by adding the following code line:
	
		<association id="QB64FList.xml" userDefinedLangName="QB64"/>
		
	    as explained inside the overrideMap.xml file.
	1.4) Copy config.xml to the main folder of NP++, and replace the existing one.


2) Config NotePad++ to use F5 key to compile .bas files and execute your .exe file  -------------------

	2.1) Copy QB64_noIDE.exe to your QB64 folder, aside with QB64.exe.
	2.2) Configure manually windows 10 to open all .bas files with QB64_noIDE.exe, selecting the "Open With.." option for any .bas file.
	2.3) Install the "RunMe" plugin on NP++ at Menu-Plugins -> Plugins Admin ->, and restart it after installation.
	2.4) On NP++ Menu-Settings -> Shortcut Mapper -> 'Plugin commands' menu, and on 'Filter' enter 'Run' and change the shortcut key of 
		'Shell execute current file' to F5. And click 'Close'.	
		 Now when pressing F5 it will compile the active NP++ document with QB64_noIDE.exe.	
	2.5) If you are editing a .bas file and if after pressing F5 for compilation you pretend to run your .exe file (a lot of times): 
		 go to Menu-Run -> Run -> Select your [file_name].exe file inside QB64 folder and click 'save' to add it to the Run Menu Apps.
		 Now you can edit/add a shortcut key to run your executable file.



3) Version History  -----------------------------------
			

	Rev.0.2 - 20 Aug 2022.
		- Added Macro to insert Line Coments (only works when selecting the entire line or more). 
		- Added Macro to remove Line Coments (only works when selecting the entire line or more). 
		  (Macros are saved at shortcuts.xml file)		
		- Updated QB64FList.xml (see file for updates history)
		- Updated UDL to qb64_UDL_v0.003.xml
		- Added new qb64_UDL_DarkMode_v0.003.xml for DarkMode color Preferences.
		
	Rev.0.1 - 26 Aug 2022.
		- - Updated UDL to qb64_UDL_v0.002.xml
	
	Rev.0.0 - 15 Aug 2022.
	


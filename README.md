# Opencore-For-i5-4460-Gtx-970-H97M-D3H

OpenCore Build 0.7.7


My Hardware List:-
  
    1.Intel i5-4460 (Hashwell)
    2.Gigabyte H97M D3H (LGA 1150)
    3.Msi Gtx 970
    4.8Gb Ram (4Gb x 2)
    5.Adata SU800 256Gb SSD (For Macos)
    6.Wd 1tb Internal HDD (For Data Storage)
    7.Tp-Link T2u Plus(Mercusys MU6H AC650)


Requried Files To Downlaod:

 (1) Pre-Install Files :-
 
 
    1.Latest Opencore Pkg :- https://github.com/acidanthera/OpenCorePkg
    
    2.Plist Editor :- https://github.com/corpnewt/ProperTree (Windows/Linux/Macos)
                                                   OR 
                      https://mackie100projects.altervista.org/opencore-configurator/ (macOS Only)
                      
    3.GenSMBIOS :- https://github.com/corpnewt/GenSMBIOS
    
    
    
 (2) Post-Install Files :-
 
    1.Latest Nvidia Web Driver (Till Macos 10.13.6) :- https://www.tonymacx86.com/nvidia-drivers/
    
    2.Tp-Link T2u Plus(Mercusys MU6H AC650) :- https://www.tp-link.com/us/support/download/archer-t2u-plus/ (Select According To Your Macos Version)
    
    
    
Making Bootable Opencore Hackintosh:-
    
      1. Gether Kext You Required 
      2. Edit config.plist as your hardware shown in opencore site
      3. If you Are Using the same config.plist as me then use GenSMBIOS (Removed Mine For Privacy issues):-
              iMac15,1 - For dGpu User(Till Macos 10.13.6 / High Sierra)
                       OR
              iMac14,4 - For iGpu User
      4. Edit Your BIOS Setting And Boot From USB
      


If Having Issues While Installing Hackintosh:(Ignore If You Installed Successfully WIthout Any Error)
  
  Q1. Can't Install Macos On SSD After One/Two Installation Reboot Can't Find Marcos List on Opencore BootMenu:
           
           Step 1:-
              This Problem Happens Because Of SSD Disk Format issue(APFS is THe MAin Reason)
           
           Step 2:-
              For This Problem, You Have To First Install Macos On HDD 
           
           Step 3:-
              After Installing In HDD You Have to Reboot To Recovery And Format SSD To Mac OS Extended (Journaled)
              Now Clone Your HDD TO SSD Via Restore Option in Disk Utility in Recovery
              After Successful Clone Format your HDD And Reboot
           
           Step 4:-
              After Booting From The SSD Add EFI To Your SSD
              Done You Installed Successfully Marcos On Non-Compatible SSD Drive 
              
              
              
  Q2. Issue With Nvidia Web Driver / Low Graphics Memory:
            
           Step 1:-
                  Source Of fix:- (https://www.youtube.com/watch?v=kJdMOlDYSWM)
                  Reboot To Recovery And Open Terminal And Write "csrutil disable" Now Reboot To macOS
                  
           Step 2:-
                  Open Terminal And Write "sudo nano -w /system/library/coreservices/systemversion.plist"
                  
           Step 3:-
                  Change Ver. "17G14042" <-- #Check The macOS Latest Version Of Macos From (https://www.tonymacx86.com/nvidia-drivers/)
                  CTRL +x
                  Y
                  Enter
                  Reboot And Install Nvidia Web Driver Pkg
                  Done
                  
                  

Useful Links For Scratch Build Of Hackintosh Opencore ( Not Me ):-
    
    1. Pre-Installtion Guide :-
    
            https://youtu.be/uzJgD3UgVnA
            
    2. Post Installtion Guide :-
    
            https://youtu.be/IP7crXa-5lo





Having Any Query Or Want To Thank me:-
    
    1. linkedin.com/in/ankitpipalia
    2. instagram.com/ankitpipalia
    2. twitter.com/ankitpipalia

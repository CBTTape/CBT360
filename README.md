# CBT360
Converted to GitHub via [cbt2git](https://github.com/wizardofzos/cbt2git)

This is still a work in progress. 
Due to amazing work by Alison Zhang and Jake Choi repos are no longer deleted.

```
//***FILE 360 IS FROM THE STATE OF WISCONSIN,  WILSON STREET        *   FILE 360
//*           REGIONAL COMPUTING CENTER WITH THE FOLLOWING MEMBERS  *   FILE 360
//*           THIS FILE IS IN IEBUPDTE SYSIN FORMAT :               *   FILE 360
//*                                                                 *   FILE 360
//*       Note:  The COMMAND program was fixed (2006/Feb) by        *   FILE 360
//*              Mike Tomkins.  email: mjt6@daimlerchrysler.com     *   FILE 360
//*                                                                 *   FILE 360
//*           ASMCMD     THIS MEMBER IS THE JCL TO ASSEMBLE AND     *   FILE 360
//*                      LINKEDIT COMMAND INTO A LINKLIST           *   FILE 360
//*                      LIBRARY.                                   *   FILE 360
//*                                                                 *   FILE 360
//*           ASMSPY     THIS MEMBER IS THE JCL TO ASSEMBLE AND     *   FILE 360
//*                      LINKEDIT SPY INTO A LINKLIST LIBRARY.      *   FILE 360
//*                                                                 *   FILE 360
//*           ASMSWP     THIS MEMBER IS THE JCL TO ASSEMBLE AND     *   FILE 360
//*                      LINKEDIT SWAP INTO A LINKLIST LIBRARY.     *   FILE 360
//*                                                                 *   FILE 360
//*           AUTH       THIS MEMBER IS THE SOURCE FOR AUTH         *   FILE 360
//*                      MACRO TO ISSUE A USER SVC THAT GETS AND    *   FILE 360
//*                      RELEASES PROGRAM AUTHORIZATION FOR AN      *   FILE 360
//*                      ASSEMBLER PROGRAM.                         *   FILE 360
//*                                                                 *   FILE 360
//*           BEGIN      THIS MEMBER IS THE SOURCE FOR BEGIN        *   FILE 360
//*                      MACRO TO DO STANDARD ENTRY LINKAGE IN      *   FILE 360
//*                      ASSEMBLER PROGRAMS.                        *   FILE 360
//*                                                                 *   FILE 360
//*           COMMAND    THIS MEMBER IS THE SOURCE FOR COMMAND      *   FILE 360
//*                      VERSION 2.0.  IT WAS ORIGINALLY TAKEN      *   FILE 360
//*                      FROM A FILE ON THE CBT TAPE.  SEE THE      *   FILE 360
//*                      PROGRAM DOCUMENTATION FOR ADDITIONAL       *   FILE 360
//*                      COMMENTS ABOUT THE ORIGIN OF THIS CODE.    *   FILE 360
//*                      COMMAND IS USED BY SPY TO ISSUE            *   FILE 360
//*                      OPERATOR COMMANDS VIA SVC 34.  I ADDED     *   FILE 360
//*                      THE SUPPORT FOR THE BEGIN, FINISH AND      *   FILE 360
//*                      AUTH MACROS.                               *   FILE 360
//*                                                                 *   FILE 360
//*                      Fixed (Feb. 2006) by Mike Tomkins.         *   FILE 360
//*                      email:  mjt6@daimlerchrysler.com           *   FILE 360
//*                                                                 *   FILE 360
//*           DISIMAGE   IBM 3800 PRINTING SUBSYSTEM SUPPORT        *   FILE 360
//*                      UTILITY.  THIS MEMBER WILL ALLOW YOU TO    *   FILE 360
//*                      CREATE AN IEBIMAGE SOURCE DECK FROM ANY    *   FILE 360
//*                      MEMBER OF SYS1.IMAGELIB (EXCEPT            *   FILE 360
//*                      COPYMOD'S) THAT WAS CREATED BY IEBIMAGE    *   FILE 360
//*                      IN THE FIRST PLACE.                        *   FILE 360
//*                                                                 *   FILE 360
//*           DISKMAP    THIS MEMBER WILL LIST THE CONTENTS         *   FILE 360
//*                      OF A VTOC IN SEVERAL USEFUL FORMATS.       *   FILE 360
//*                      ORIGINAL PROGRAM WAS FROM CBT TAPE.        *   FILE 360
//*                      THIS VERSION HAS SEVERAL CHANGES           *   FILE 360
//*                      INCLUDING 3380 SUPPORT.                    *   FILE 360
//*                                                                 *   FILE 360
//*                      (Replaced with newer version - 09/08/24)   *   FILE 360
//*                      Older version was renamed DISKMAP0.        *   FILE 360
//*                                                                 *   FILE 360
//*           DTYP2UNT   THIS SUBROUTINE WILL CONVERT A UCB-TYPE    *   FILE 360
//*                      HEX DEVICE CODE TO A VALID UNIT NAME       *   FILE 360
//*                      USING THE SYSTEM DEVICE NAME TABLE.        *   FILE 360
//*                                                                 *   FILE 360
//*           DYNAM      THIS SUBROUTINE IS CALLED BY DYNAUTIL      *   FILE 360
//*                      TO DO DYNAMIC ALLOCATION AS NEEDED BY      *   FILE 360
//*                      ITS DRIVER.  ORIGINALLY FROM THE           *   FILE 360
//*                      UNIVERSITY OF MANITOBA.                    *   FILE 360
//*                                                                 *   FILE 360
//*           DYNAUTIL   DYNAUTIL IS A REENTRANT, REFRESHABLE,      *   FILE 360
//*                      AND REUSABLE ASSEMBLER LANGUAGE PROGRAM    *   FILE 360
//*                      THAT PROVIDES DYNAMIC ALLOCATION FOR       *   FILE 360
//*                      BATCH PROGRAMS AND UTILITIES.  THIS IS     *   FILE 360
//*                      ACCOMPLISHED BY PASSING CONTROL CARD       *   FILE 360
//*                      IMAGES TO THE UNIVERSITY OF MANITOBA'S     *   FILE 360
//*                      DYNAM SVC 99 INTERFACE.  DYNAUTIL CAN      *   FILE 360
//*                      RUN AS A FRONT-END TO A BATCH TASK OR      *   FILE 360
//*                      CAN BE CALLED BY A BATCH TASK DURING       *   FILE 360
//*                      ITS EXECUTION.                             *   FILE 360
//*                                                                 *   FILE 360
//*           DYNAUTLH   THIS IS THE DOCUMENTATION FOR THE          *   FILE 360
//*                      DYNAUTIL PROGRAM.                          *   FILE 360
//*                                                                 *   FILE 360
//*           FINISH     THIS MEMBER IS THE SOURCE FOR FINISH       *   FILE 360
//*                      MACRO TO DO STANDARD EXIT LINKAGE IN       *   FILE 360
//*                      ASSEMBLER PROGRAMS.                        *   FILE 360
//*                                                                 *   FILE 360
//*           IDCMSGEN   ACCESS METHOD SERVICES (IDCAMS) SUPPORT    *   FILE 360
//*                      UTILITY.  THIS PROGRAM WILL ALLOW YOU      *   FILE 360
//*                      TO CREATE AN IDCAMS SOURCE DECK FROM       *   FILE 360
//*                      MOST OBJECTS IN YOUR VSAM CATALOG.         *   FILE 360
//*                                                                 *   FILE 360
//*           IEFACTRT   SMF EXIT THAT PRODUCES MANY USEFUL         *   FILE 360
//*                      STATISTICS AND MESSAGES AT STEP AND JOB    *   FILE 360
//*                      END.  THESE MESSAGES APPEAR IN AN          *   FILE 360
//*                      ABBREVIATED FORM IN THE JOBLOG AND IN A    *   FILE 360
//*                      MORE DETAILED FORM IN THE JOB MESSAGES     *   FILE 360
//*                      OUTPUT.                                    *   FILE 360
//*                                                                 *   FILE 360
//*           IEFU84     SMF EXIT THAT DOES A GETMAIN FOR AN        *   FILE 360
//*                      AREA THAT BECOMES A LOCAL USER CVT.        *   FILE 360
//*                      THIS AREA IS MAPPED BY WSRCCCVT.           *   FILE 360
//*                                                                 *   FILE 360
//*           IGC0023C   A TYPE 3 SVC THAT IS INVOKED FROM THE      *   FILE 360
//*                      AUTH MACRO TO AUTHORIZE OR UN-AUTHORIZE    *   FILE 360
//*                      TSO COMMANDS, PROGRAMS, ETC.               *   FILE 360
//*                                                                 *   FILE 360
//*           ISPTCM     A MACRO (TCMGEN) AND A MODULE (ISPTCM)     *   FILE 360
//*                      THAT REPLACE THE DISTRIBUTED ISPF          *   FILE 360
//*                      MODULE.  THIS MACRO AND MODULE WERE        *   FILE 360
//*                      WRITTEN IN RESPONSE TO APAR OZ64211.       *   FILE 360
//*                      SEE INFO/MVS ENTRY E130403 FOR             *   FILE 360
//*                      PARTICULARS.                               *   FILE 360
//*                                                                 *   FILE 360
//*           LASTIPL    TSO COMMAND THAT USES THE LOCAL            *   FILE 360
//*                      USER CVT MAPPED BY WSRCCCVT TO             *   FILE 360
//*                      DISPLAY WHEN THE SYSTEM WAS                *   FILE 360
//*                      IPL'ED.                                    *   FILE 360
//*                                                                 *   FILE 360
//*           PRINTOFF   TSO COMMAND ORIGINALLY FROM THE CBT        *   FILE 360
//*                      TAPE AND HEAVILY MODIFIED FOR USE AT       *   FILE 360
//*                      WSRCC HAS SUPPORT FOR THE 3800 PRINTING    *   FILE 360
//*                      SUBSYSTEM VIA CHARS, TRC, MODIFY,          *   FILE 360
//*                      MODTRC, FLASH, FCOUNT, CGROUP AND BRUST    *   FILE 360
//*                      KEYWORDS.  SOME PROBLEMS WITH THE 6670     *   FILE 360
//*                      CODE HAS ALSO BEEN FIXED.                  *   FILE 360
//*                                                                 *   FILE 360
//*           PRINT0FF   TSO HELP FOR THE MODIFIED PRINTOFF         *   FILE 360
//*                      COMMAND.                                   *   FILE 360
//*                                                                 *   FILE 360
//*           SPY        THIS MEMBER IS THE SOURCE FOR SPY          *   FILE 360
//*                      VERSION 3.1 WITH CROSS MEMORY SUPPORT      *   FILE 360
//*                      INCLUDED FOR MVS/SP 1.3.  IT WAS           *   FILE 360
//*                      ORIGINALLY TAKEN FROM FILE 338 ON THE      *   FILE 360
//*                      CBT TAPE.  SEE THE PROGRAM                 *   FILE 360
//*                      DOCUMENTATION FOR ADDITIONAL COMMENTS      *   FILE 360
//*                      ABOUT THE ORIGIN OF THIS CODE.  THE        *   FILE 360
//*                      VAST MAJORITY OF THE XM CODE CAME FROM     *   FILE 360
//*                      THE BANK OF NEW SOUTH WALES.  I ADDED      *   FILE 360
//*                      THE CODE TO SUPPORT THE PFKEYS IN THE      *   FILE 360
//*                      3270 ENVIRONMEMT ALONG WITH THE BEGIN.     *   FILE 360
//*                      FINISH AND AUTH MACROS.                    *   FILE 360
//*                                                                 *   FILE 360
//*           SWAP       THIS MEMBER IS THE SOURCE FOR SWAP         *   FILE 360
//*                      VERSION 4.5.  IT WAS ORIGINALLY TAKEN      *   FILE 360
//*                      FROM A FILE ON THE CBT TAPE.  SEE THE      *   FILE 360
//*                      PROGRAM DOCUMENTATION FOR ADDITIONAL       *   FILE 360
//*                      COMMENTS ABOUT THE ORIGIN OF THIS CODE.    *   FILE 360
//*                      I ADDED THE SUPPORT FOR THE BEGIN,         *   FILE 360
//*                      FINISH AND AUTH MACROS.                    *   FILE 360
//*                                                                 *   FILE 360
//*           UADS       TSO COMMAND THAT WILL ALLOW THOSE USERS    *   FILE 360
//*                      WITH OPERATOR ABILITY TO DYNAMICALLY       *   FILE 360
//*                      CHANGE THEIR UADS ENTRIES IN THE PSCB.     *   FILE 360
//*                      ONCE CHANGED, IT WILL REMAIN IN EFFECT     *   FILE 360
//*                      ACROSS A RELOGON (UNLESS USING ACF2 IN     *   FILE 360
//*                      NOUADS MODE).                              *   FILE 360
//*                                                                 *   FILE 360
//*           UADSHELP   TSO HELP FOR THE UADS COMMAND.             *   FILE 360
//*                                                                 *   FILE 360
//*           VOLS       TSO COMMAND TO LIST FREE SPACE ON ALL      *   FILE 360
//*                      OR SELECTED ONLINE DASD DEVICES.           *   FILE 360
//*                      VOLUME SELECTION INCLUDES DEVICETYPE,      *   FILE 360
//*                      ATTRIBUTE, VOLUME AND UCB.                 *   FILE 360
//*                                                                 *   FILE 360
//*                      (FIXED FOR DYNAMIC UCB'S - G.GORAB 8/95)   *   FILE 360
//*                      (FIXED FOR 4-DIGIT UCB'S AND ALSO 3 DIGIT  *   FILE 360
//*                        UCB'S, BY GORDON B. HAMPTON - 04/98)     *   FILE 360
//*                                                                 *   FILE 360
//*                      (Fixed for large volumes and different     *   FILE 360
//*                        display options by Gordon B. Hampton,    *   FILE 360
//*                        11/2008.  See member $$VOLSUP.)          *   FILE 360
//*                                                                 *   FILE 360
//*                      SEVERAL OLD VERSIONS OF VOLS ARE ALSO      *   FILE 360
//*                      INCLUDED IN THIS FILE, TO MAKE SURE THAT   *   FILE 360
//*                      PEOPLE ON OLDER SYSTEMS CAN STILL USE IT.  *   FILE 360
//*                                                                 *   FILE 360
//*           VOLSHELP   TSO HELP FOR THE VOLS COMMAND.             *   FILE 360
//*                                                                 *   FILE 360
//*           WSRCCCVT   MACRO THAT MAPS THE LOCAL USER CVT THAT    *   FILE 360
//*                      IS GOTTEN AT IPL TIME BY IEFU84.  A        *   FILE 360
//*                      LOCAL USER CVT IS VERY USEFUL FOR MANY     *   FILE 360
//*                      RANDOM USES, WE FIND MANY FOR OURS.        *   FILE 360
//*                                                                 *   FILE 360
//*           ZSORTZ     THIS SUBROUTINE WILL SORT AN IN-CORE       *   FILE 360
//*                      TABLE. ORIGINAL SOURCE UNKNOWN             *   FILE 360
//*                      (PROBABLY EARLY 1970'S SHARE TAPE (?)).    *   FILE 360
//*                                                                 *   FILE 360
```

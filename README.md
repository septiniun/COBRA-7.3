# COBRA 7.1 Source

As of April the 1st.

Following has been changed and updated since 4.46 COBRA 7

[Joonie's Changes]

* Cobra spoofer has been removed again, since this is no longer supporting PSN accesibility since 4.60 OFW update.
* Kakaroto's sig check patch is removed from modulespatch.c since this is one of those pre-applied patches on 4.xx CFW
* unknown E3 patches are removed to fix an issue with XMB, [Originally found by rancid-0, from his PS3ITA 4.50 COBRA]
* Dual VSH supports for REBUG REX / D-REX CFW, proper hash check code was developed by habib and Nzv recently. 
* NPDRM Fself fix for REBUG REX/D-REX, this removed Kakaroto's sig check patch pre-applied in REBUG's debug VSH.

[ Habib's changes ]

* Stage0 Base payload, this clears stage1 when stage2 is not loaded on LV2, which completely disabled COBRA mode
* Ps2netemu work around is discovered, now PS2 ISO can be redirected as ps2classic, this was developed to fix ps2 wireless pad sync issue for non backward compatible PS3 models.
* Syscall 11 is added to support full lv1 peek

[KW's changes]

* webMAN integration on boot. Also disables external webMAN plugin located in dev_hdd0
* PSN Patch stealth mode, it remove custom syscall from the ps3

[ Dean's changes ] 

* Improved map_path, to fix the issue with games like Shadow of Mordor
* Permission protection is disabled to increase game compatiblity and full DEX support.[no more issue with Target Manager or CCAPI]
* 80010017 / 8001002B Error fix is added since 4.60, this was developed to prevent issues with games when game disc is inserted in BD Drive.
* LIC.DAT check is patched to fix the issue with launching homebrew since 4.60

[ Nzv's changes]

* PS3MAPI 1.2.2 support, it is similar feature comparing to CCAPI, but open sourced project and also can unload vsh plugins , attatch process on all type of EBOOT.
   One of those great debugging features.
* Partial disable syscall8 and unhooks all cobra hooks (Part of PS3MAPI)
* Block update from disc
   
[ Aldo's changes ]

* Improved PSX media type support, now it supports following disc types
	* 2048 // 2352 // 2336 // 2448 *
* Improved Video mode patch with proper region detection
 Original COBRA payload was relying on ps1emu's detection method, now COBRA has extra pre-processing that can detect region properly and force apply correct refresh rate depending on the game's region.
 
*STILL IN W.I,P, please let me know if anyone is interested in making changes in this note :)

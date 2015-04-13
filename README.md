;*****************************************************************
;General Use Script: Adding the TargetCouponPrefix setting to the controller.
; Brief Explanation: This script adds the TargetCouponPrefix setting 
; to the controller section that will force the setting to null and resolves
; a duplicate PLU redemption data issue
;Store Systems Mgr is 
;Store Systems Rep is Me
;**********************************************************
;Minimum Software Requirements:
;Awards Version: 6.6.3.X
;OS2 or XPe: 	All Versions
;**********************************************************
;Last Tested and Updated Date: whenever
;Tested and Signed Off By me

; *********************************************************
; Begin StoreFix Script
; *********************************************************
[Commands]
Command1=UpdateSection,ControllerSection
Command2=CleanStore 

[ControllerSection]
All_Stores=USM_Walgreens,ControllerupdateSection

[ControllerupdateSection]
TargetCouponPrefix=""

; *********************************************************
; End StoreFix Script
; *********************************************************

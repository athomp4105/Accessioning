# Container Numbers hook-I.D.

Correct item numbering makes finding aids JavaScript-hook compatible for future mass digitization using CONTENTdm interface. 

Letters can appear in single folder numbers but they cannot appear in ranges. For example, Folder 1a-2, is not allowed. 

For containers with prefixes, write as P-0345/1, P-0345/2 , and P-0345/3, rather than as a range: P-0345/1-3 even if they have the same unit titles. (via Laura Hart, January 2017) 

Do not encode multiple, non-sequential container numbers in the same ```<container>```. For example, if both folder 14 and folder 18 have information on Martians, do not write ```<container type='folder'>14, 18</container>```. In this case, you should encode them separately.(check with Lynn) 

Do not encode multiple unittitles in one c0x. We prefer multiple c0x with a repeating container, which is automatically suppressed so that you end up just seeing the multiple unittitles. 

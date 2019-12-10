# kiosk
Experimental trial. This site has porteus config files for kiosk pcs to be used by tax-preparer volunteers.  

## Intro
I was hoping let tax-preparers use kiosk pcs to fill out taxforms for multiple clients at  https://vita.taxplayerpro.com using only google-chrome (and with a fast secure wired-only connection to internet). Since porteus boots from read-only iso, and runs entirely in ram, I felt this would help ensure no personal information could be left on the kiosk-pc. For example,  Porteus-kiosk cannot mount, and cannot even see any local storage (/dev/sda) and lets you choose to enable/disable usb-flash-drive support.

Typically, you answer questions and fill in info on a tax-prep website, and in the end it generates the filled-in forms to submit. A hopefully rare but problematic issue is if any tax-forms with editable fields need to be downloaded and manually filled out, such as: http://www.irs.gov/pub/irs-pdf/f1120ssk.pdf This taxslayer site says you may need to manually edit that 1120 form https://zen-vita.zendesk.com/hc/en-us/articles/360009289413-Schedule-K-1-Form-1120S-Shareholder-s-Share-of-Income-

> Note: Some items reported on a Schedule K-1 (Form 1120S) may need to be entered directly into a specific form instead of the K-1 entry screen. Please refer to the links above to find out if this is case for any items that do not have an entry field located in the K-1 entry screen. To [do] this ... you must have Adobe Acrobat Reader installed on your computer.

While you can fill out such forms in Chrome, once you print the form to a pdf, you cannot go back and change any fields. And Adobe or other software used by the intended recipient of the filled-out may not be able to extract the values in the filled-out fields (as it seems the field structure/data is lost when printed to a pdf). For details see:
https://support.google.com/chrome/thread/3121696?hl=en  For these reasons, many entities, like ct.gov warn to only use only Adobe Reader to fill out forms: https://www.ct.gov/deep/cwp/view.asp?a=2690&Q=322444&deepNav_GID=1511 They also warn Macintosh users not to use Preview to fill-out forms, as it is well known to not work well, and have problems. Linux folks also seem to have problems finding software to reliably fill out pdf-forms, as Adobe-Reader is no longer available for linux.
One solutions for filling out forms in Linux is a free but non-open-source PDF-Studio-Viewer. It works on almost any platform, including Macintosh, Windows, and lots of flavors of linux, etc: https://www.qoppa.com/pdfstudioviewer/download/

Finally, in the interest of always having more than one way to do thing, note that the Edge-browser included in all non-LTS versions of Windows10 can fill out pdf forms, and the filled-out form retains form fields, can be re-editted, etc! That is, I could fill out pdf forms in Edge browser, and save it, then re-open and further change the form-fields. (I tested with oldest and newest edge I could find:  Edge 44.18362 on Windows-10-1909).


## Todo: step-by-step instructions to be added below... 
* boot lenovo edge (type 0302) from "Porteus Kiosk Cloud 4.9.0" iso from https://porteus-kiosk.org/download.html

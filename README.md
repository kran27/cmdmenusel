# CmdMenuSel (V1.4) 
CmdMenuSel displays a line based menu in the console allowing the user
to select a single option. The menu can be interacted with via the mouse
or keyboard. The menu colours can be choosen or the defaults used(E2F4). An exit code(ErrorLevel) is returned denoting the position the selected option was specified in.
## Usage
  CmdMenuSel FBFB "Option 1" "Option 2" etc.
  All option string are trimmed to the console width. The number of specified
  options must be less than or equal to the number of lines in the console.
  FBFB denotes the colours to be used, they are four hex digits
  (0 - 9 and A - F). The first two digits corrospond to the selected
  menu item and the last two corrospond to the unselected menu items.
  F is the foreground colour and B is the background colour.
Use `color zz` for colour code listings.
The default colours are used if the:
String contains characters outside of 0-9,A-F or a-f.
String isn't exactly four characters.
Selected or unselected background and foreground colours are the same.
Selected and unselected background colours are the same.
If an error occurs the return code will be zero and a string will be set
to the console error stream.

## Usable input
###### Select:
 "SPACE" "ENTER" "LEFT_CLICK"
###### Navigate
 "UP" "DOWN" "TAB" "SHIFT + TAB"
 "HOME" "END" "PAGE_UP"
 "PAGE_DOWN" "MOUSE_HOVER" "SCROLL_WHEEL"

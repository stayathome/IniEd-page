IniEd
-----

TC Lister-plugin for viewing and editing settings files (*.ini, *.inf, *.reg).
Compared to text editors offers the convenience of editing 
and high speed opening large files.

Minimal requirements
--------------------
- Total Commander 5.51

Manual Installation
-------------------
1. Unpack IniEd.wlx into a plugins' directory (f.e., c:\wincmd\plugins).
2. Select "Configuration -> Options" point in the TC menu.
3. Open "View/Edit" page.
4. Press "Configure internal viewer" button, then "LS-plugins" button.
5. Press "Add" button and choose IniEd.wlx. Press "Ok".
6. Enjoy! ;-)

Note. To use the plugin with other file types (* .url, * .log), you can edit 
      the corresponding "_detect" line in the wincmd.ini file and add 
      the extension you want.

Hotkeys
-------
  Tab or Ctrl+Tab   - Switch between the Section and String panels
  Ctrl+Tab          - Toggle key/value selection while string editing
  Enter             - Edit string parameter
  F1                - About plugin...
  F2 or Shift+Enter - Rename string
  F7 or Ctrl+F      - Find
  F3 or F5          - Find next
  F9                - Sort(all) alphabetically
  Ctrl+Del          - Delete string
  Shift+Del         - Delete entire section
  Ctrl+Insert       - Insert a string below the current
  Ctrl+Shift+Insert - Insert a string above the current
  Ctrl+Up           - Move the string down
  Ctrl+Down         - Move the string up
  Ctrl+PgUp         - Go to the next section
  Ctrl+PgDown       - Go to the previous section
  Ctrl+X            - Cut
  Ctlr+C            - Copy
  Ctrl+V            - Paste
  Ctrl+A            - Select whole string (in edit mode)
  Ctrl+D            - Duplicate string
  Ctrl+N            - Add new section below the current
  Ctrl+Shift+N      - Add new section to bottom
  Ctrl+` or
  Ctrl+BackSpace    - Do/undo comment
  Ctrl+S            - Save changes
  Ctrl+Shift+S      - Save as...
  Ctrl+Z            - Undo last change
  Ctrl+Shift+Z or
  Alt+BackSpace     - Redo last change
  Ctrl+P            - Options
  Alt+A             - ANSI Encoding
  Alt+U             - Unicode Encoding
  Alt+T             - UTF-8 Encoding
  Alt+S             - ASCII Encoding (DOS CP-866)


License (everybody has it, why not me? ;-)
--------------------------------------------
This software is a Freeware and is distributed "as is". You can use it
however you want, yet without changing the distribution's contents.
Author doesn't guarantee you fulfillment of all your best wishes.
Also, he doesn't bear responsibility of any damages, caused by the
software. Yet, he will try his best to react to each bug report. :-)

Thanks
------
This plugin was created with the use of TC Help and C. Ghisler's
LS-plugin example's source code.
Author wants to thank the following persons:
- Ajax A.S., Irakly Tchanturia -- for their great advices, beta-testing
- and the current file translation.
- E. Savitch -- for interesting ideas, found in his "Teaching plugin - RTF-viewer".
- All users of wincmd.ru forum and personally Avada and Flasher - for new ideas, patience and beta testing.

Author
------
StayAtHome
Web:    www.stayathome.ho.ua
E-Mail: stayathome@email.ua


Version history
--------------
v. 2.0 - 14.04.2020
  [!] 64-bit support added (Total Commander 8.X)
  [!] Undo history added
  [!] Significantly improved performance of plugin 
  [*] An ability to select multiple lines added
  [*] Plugin settings file (IniEd.ini) can be stored either in the same directory wincmd.ini (default)
      or in the plugin directory (as in the previous version).
  [*] Improved Unicode support also for long file paths (more than 259 characters).
  [*] Improved encoding auto-detection.
  [+] Horisontal layout for REG files (+autoheight).
  [+] Automatic abbreviation of registry hive names (HKEY_CURRENT_USER <-> HKCU).
  [*] Highlighting settings is enhanced (it's recommended to delete old IniEd.ini settings file).
  [+] The restriction on the presence of two sections with the same name has been removed.
  [+] Character settings for section title, comment, separator key/value.
  [+] Ability to select multiple lines and perform standard actions with them.
  [+] Hotkey Shift + Del -- delete the entire section from the lines panel.
  [-] Exit plugin error fixed when IniEd.ini is not writable.
  [+] Ability to delete sections without confirmation (optional).
  [+] Horizontal scroll bar in the sections panel (optional).
  [*] Warning about the duration of sorting large files.
  [-] Invalid filter in the dialog box and double extension on "Save as..."
  [+] Overwrite confirmation of an existing file when on "Save as..."
  [+] The contents of the active TC file panel is updated when saving a file in quick view mode (optional).
  [*] The message about exceding of max line length  disabled. Max. line length is 65536 characters now.
  [-] Fixed display of tab characters.
  [+] The ability to focus by default on the strings panel.
  [+] Hotkey Ctrl+Tab key in line editing mode to switch the key/value selection (optional).

v 1.2 - 12.04.2009
  [*] Now it is possible to save files with attributes "Hidden", "System" or "Read Only".
  [+] Hitkey Ctrl+Shift+S -- "Save as" is added.
  [+] Hints for left panel is added.
  [*] Limit for 1024 symbols in string is removed. Now limit is set in options.
  [+] Word-wrapping is added when editing long strings.
  [+] Background color settings is added for left and right panels.
  [+] Font style and color settings is added for left panel and for sign "=".

v. 1.1 - 13.07.2004
  [-] Fixed the error occured while calling the options window.
  [*] Sections listing font is changed to "MS Sans Serif" as default.
  [-] In some cases the context menu couldn't be called.
  [+] Added "cancel" button which allows to cancel the quiting from plugin
      in file saving request while pressing "Esc".
  [-] Plugin lost the focus while pressing cancel in "Save as" window.
  [+] Double click on divider automaticaly sets the width of sections panel.
  [*] Context menu items order is changed.
  [-] While editing if mouse was clicked on other section 
      the following message: "Section already exists" appeared.
  [-] Double click on "< All sections >" item switched on string editing.
  [+] An ability to sort strings and sections in alphabet order added.
  [+] Unicode support.
  [+] Switches and shows current encoding in status bar.
  [+] Sections now can be copied, cut and pasted together with its content.
  [*] Now plugin handles the files with following extensions: .ini, .inf, .reg.
  [-] Fixed the incorrect displaying of symbols with big font size.
  [*] Now plugin opens null size files.
  [+] UTF-8 support.
  [*] Added error handling, occured if there was string in file with
      more than 1024 symbols.
  [+] The information about strings and sections added to status bar.
  [+] Alternative hotkey for "Comment/Uncomment" (Ctrl+BackSpace).

v. 1.0 - 05.07.2004
  [*] Improved fonts rendering in the Options dialogue.
  [-] Some points in context menu didn't work.
  [*] Small changes in context menu.
  [-] Error occured while working in an empty section.
  [-] The focus didn't move to Section list after the forced call (button "4").

v. 0.4 Beta - 27.06.2004
  [!] Plugin completely rebuilt
  [+] Different hotkeys added
  [+] Added Clipboard support
  [*] Error handling has improved
  [+] Added current cursor position representation (percentage)
  [+] Added Status bar
  [+] Added search
  [-] Zero-sized file opening bug fixed
  [+] Highliting settings dialogue added
  [+] Added horizontal scrollbar
  [+] Menu item "Save As..." added
  [+] Saving Section Panel width added

v. 0.3 Beta - still didn't appear in public for it's slowness
  [!] Syntax highliting rebuid for WinAPI and turned to separate stream
  [*] The Section panel font turned to proportional
  [+] Adeed Current Section Name bar
  [+] Added Ctrl+S hotkey

v. 0.2 Alpha - 31.01.2004
  [!] First working buid. A little bit slow yet almost perfect, surprisingly

v. 0.1 Alpha - Never appeared in public

Legend:
  [!] - Important
  [+] - Added
  [*] - Changed
  [-] - Bug fixed

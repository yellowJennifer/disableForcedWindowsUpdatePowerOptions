# Disable Forced Windows Update Power Options
a simple registry key file that brings the values of the items that show on the power off menu, back to the normal ones "Shut down" and "Restart", with no forced update, for Windows 10 and 11.
<br><br><br><br><br>
**before:** <br>
<img width="307" height="165" alt="image" src="https://github.com/user-attachments/assets/1dfeb6e5-b780-4d63-9f49-7165d2b400fb" /> <img width="308" height="219" alt="image" src="https://github.com/user-attachments/assets/bfc7273d-ac89-48eb-9f75-b2c27f131b70" />



**after:** <br>
<img width="136" height="168" alt="image" src="https://github.com/user-attachments/assets/f6cc914e-8091-4f28-8f44-c875b5aadff6" />
<br><br><br>
all the file does is set `Computer\HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsUpdate\Orchestrator\ShutdownFlyoutOptions` to 0, resetting all power off options back to normal.

if you want a "click and run" option for this, you can get the .reg file that does literally just this 👆, in [the releases.](https://github.com/yellowJennifer/disableForcedWindowsUpdatePowerOptions/releases/tag/initial-releases)
<br>

# Disclaimer:
Windows seems to reset this value upon system restart; or even while the computer is on.... (unconfirmed) <br><br>
as a band-aid fix, I added the file to `shell:startup` or `C:\Users\(YourUser)\AppData\Roaming\Microsoft\Windows\Start Menu\Programs\Startup` (same folder), so it just prompts you to press yes every time you boot up your system. <br><br>
(I bet there's a way to do this better, but I'm trying my best and applying the little knowledge I have ^^")

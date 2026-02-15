# disableForcedWindowsUpdatePowerOptions
a registry key file that brings the values of the items that show on the power off menu, back to the normal ones "Shut down" and "Restart", with no forced update, for Windows 10 and 11.


before: <br>
<img width="307" height="165" alt="image" src="https://github.com/user-attachments/assets/1dfeb6e5-b780-4d63-9f49-7165d2b400fb" /> <img width="308" height="219" alt="image" src="https://github.com/user-attachments/assets/bfc7273d-ac89-48eb-9f75-b2c27f131b70" />



after: <br>
<img width="136" height="168" alt="image" src="https://github.com/user-attachments/assets/f6cc914e-8091-4f28-8f44-c875b5aadff6" />

all it does is set Computer\HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsUpdate\Orchestrator\ShutdownFlyoutOptions to 0, resetting all power off options back to normal.

if you want a "click and run" option for this, you can get the .reg file that does literally just this 👆, in [the releases.](https://github.com/yellowJennifer/disableForcedWindowsUpdatePowerOptions/releases/tag/initial-releases)

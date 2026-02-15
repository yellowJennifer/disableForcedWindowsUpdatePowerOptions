# disableForcedWindowsUpdatePowerOptions
a registry key editor that brings the values of the items that show on the power off menu, back to the normal ones "Shut down" and "Restart", with no forced update, for Windows 10 and 11.

just get the latest .reg file from Releases, and run it.

all it does it set Computer\HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsUpdate\Orchestrator\ShutdownFlyoutOptions to 0, resetting all power off options back to normal.

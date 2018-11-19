# Default Windows 10 applications
To uninstall all windows 10 applications, just run [uninstallWin10Apps.ps1](https://github.com/dojo90/uninstall-windows-10-apps/blob/master/uninstallWin10Apps.ps1) in a WindowsPowershell with admin rights.

---

The default execution policy of PowerShell is called Restricted. In this mode, PowerShell operates as an interactive shell only. It does not run scripts, and loads only configuration files signed by a publisher that you trust. If you are getting the nasty red error the most probable cause is that you are trying to run an unsigned script. The safest thing to do is to change the Execution Policy to unrestricted, run your script and then **change it back to restricted**.

To change it to unrestricted run the following command from an administrative PowerShell:

>     Set-ExecutionPolicy Unrestricted

You will be asked if you are sure that you want to change the Execution Policy hit the enter button again.

You can now run your downloaded scripts without a problem. However, it’s a serious security risk if you forget to set the Execution Policy back to Restricted mode. You could probably guess how to set it back to Restricted, but incase you don’t:

>     Set-ExecutionPolicy Restricted
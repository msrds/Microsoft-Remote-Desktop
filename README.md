## Download Microsoft Remote Desktop

Before you can access your devices or applications from a Windows computer, ensure the following prerequisites are fulfilled:

A reliable internet connection.      
A system running one of the supported Windows editions listed below:

Windows 11      
Windows 10      
Windows Server 2022       
Windows Server 2019      
Windows Server 2016      

* .NET Framework 4.6.2 or newer. You may have to install this on Windows Server 2016, as well as certain editions of Windows 10. To obtain the most recent version, see .NET Framework download.

Below are the steps for installing the Remote Desktop client for Windows using the MSI package. If you plan to roll it out in an enterprise setting, you can use `msiexec` from the command line to deploy the MSI file.

1. Download the Remote Desktop client installer, choosing the correct variant for your device:

* [Windows 64-bit](*) *(most common)*
* [Windows 32-bit](*)
* [Windows ARM64](*)

2. Launch the installer by double-clicking the file you saved.

3. On the welcome page, click **Next**.

4. Accept the end-user license agreement by selecting **I accept the terms in the License Agreement**, then click **Next**.

5. For Installation Scope, choose one of these options:

* **Install just for you**: Remote Desktop will be placed in a per-user folder and available only to your account. No Administrator rights are needed.

* **Install for all users of this machine**: Remote Desktop will be stored in a system-wide folder and accessible to all accounts. Administrator rights are required.

6. Click **Install**.

7. After the setup is finished, click **Finish**.

8. If you left the box for **Launch Remote Desktop when setup exits** selected, the Remote Desktop client will start automatically. Otherwise, you can open it anytime via the Start menu by searching for **Remote Desktop**.

> **Important**
> If both the Remote Desktop client (MSI) and the Azure Virtual Desktop app from Microsoft Store are installed on the same system, you may encounter a message beginning with **A version of this application called Azure Virtual Desktop was installed from the Microsoft Store**. Both applications are valid, and you may choose **Continue anyway**, but using the same remote resource in both can be confusing. It is advisable to stick with just one version at a time.

## Subscribe to a workspace

A workspace aggregates all desktops and applications your admin has assigned to you. To make them visible in the Remote Desktop client, you must subscribe to the workspace as follows:

1. Open the **Remote Desktop** app on your system.

2. The first time you subscribe to a workspace, on the **Let's get started** screen, choose **Subscribe** or **Subscribe with URL**.

* If you choose **Subscribe**, sign in with your user account when prompted, e.g. `user@contoso.com`. Within a few seconds, your workspace will display the desktops and applications made available by your admin.

If you receive the message **No workspace is associated with this email address**, your admin may not have enabled email discovery, or you could be in a non-standard Azure environment (such as Azure for US Government). In such cases, try **Subscribe with URL** instead.

* If you choose **Subscribe with URL**, in the **Email or Workspace URL** field, enter the appropriate URL from the table below. After a few seconds, the message **We found Workspaces at the following URLs** should appear.

3. Click **Next**.

4. When prompted, sign in with your account. Within moments, the workspace will present the desktops and applications that your admin has assigned.

Once you have subscribed to a workspace, its content will refresh automatically on a regular basis and each time the client starts. Resources may be added, modified, or removed according to admin updates.

## Connect to your desktops and applications

To establish a connection to your desktops and applications:

1. Open the **Remote Desktop** client on your device.

2. Double-click an icon to begin a session with Azure Virtual Desktop. Depending on your admin’s configuration, you may be asked to re-enter your account password.

## Insider releases

If you would like to assist us by testing builds before they are officially released, you can download our Insider releases. Organizations may also use Insider releases to validate upcoming versions for their users before they become generally available.

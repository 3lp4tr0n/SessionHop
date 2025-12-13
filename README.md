# SessionHop

SessionHop is a C# tool that utilizes the `IHxHelpPaneServer` COM object, configured to run as an <a href="https://learn.microsoft.com/en-us/windows/win32/com/interactive-user">**Interactive User**</a>, to hijack specified user sessions. By creating a <a href="https://learn.microsoft.com/en-us/windows/win32/termserv/session-to-session-activation-with-a-session-moniker">**session moniker**</a> and utilizing the COM object's `Execute` interface, operators can run arbitrary files within another user's session. This session hijacking technique is an alternative to remote process injection or dumping lsass, and may come in handy when operators need to keylog, screenshot, or access LDAP as the affected user. Credits to James Forshaw for content and code: https://googleprojectzero.blogspot.com/2016/01/raising-dead.html

**Note**: Must be executed from high integrity.

## Usage

```SessionHop.exe <session_id> <executable>```

https://github.com/user-attachments/assets/999a38fe-0240-454d-9dbc-f790d5f7d6c7


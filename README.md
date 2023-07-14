# docker_windows

#### HOST : Windows 10 Home
#### Install WSL2

* PowerShell 관리자모드 실행
```bash
PS C:\Windows\system32> wsl --install
Ubuntu이(가) 이미 설치되어 있습니다.
Ubuntu을(를) 시작하는 중...
Installing, this may take a few minutes...
WslRegisterDistribution failed with error: 0x80004002
Error: 0x80004002 ?? ?????? ???? ????.

Press any key to continue...

PS C:\Windows\system32> Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux
지금 컴퓨터를 다시 시작하여 이 작업을 완료하시겠습니까?
[Y] Yes  [N] No  [?] 도움말 (기본값은 "Y"):
```

* Reboot and install wsl again

```bash
PS C:\Windows\system32> wsl --install
Ubuntu이(가) 이미 설치되어 있습니다.
Ubuntu을(를) 시작하는 중...
Installing, this may take a few minutes...

Please create a default UNIX user account. The username does not need to match your Windows username.
For more information visit: https://aka.ms/wslusers
Enter new UNIX username: tony
New password:
Retype new password:
passwd: password updated successfully
Installation successful!
To run a command as administrator (user "root"), use "sudo <command>".
See "man sudo_root" for details.

Welcome to Ubuntu 22.04.2 LTS (GNU/Linux 5.15.90.1-microsoft-standard-WSL2 x86_64)

 * Documentation:  https://help.ubuntu.com
 * Management:     https://landscape.canonical.com
 * Support:        https://ubuntu.com/advantage


This message is shown once a day. To disable it please create the
/home/tony/.hushlogin file.
tony@LAPTOP-NSESUJOJ:~$
```

#### References
* [윈도우 Docker 설치 완벽 가이드(Home 포함)](https://www.lainyzine.com/ko/article/a-complete-guide-to-how-to-install-docker-desktop-on-windows-10/)


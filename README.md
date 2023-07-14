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


#### References
* [윈도우 Docker 설치 완벽 가이드(Home 포함)](https://www.lainyzine.com/ko/article/a-complete-guide-to-how-to-install-docker-desktop-on-windows-10/)


## 1. 윈도우 터미널 설치  
 
 > 윈도우에서 제공하는 터미널 프로그램
 
1. choco 설치 [홈페이지]([https://chocolatey.org/](https://chocolatey.org/))  
	> choco ? chocolately 윈도우의 cmd, powershell에서 리눅스처럼 프로그램 설치할 수 있게 도와주는 프로그램

```powershell
Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))  
```  
2. choco 홈페이지에서 window terminal 검색 후 명령어 복사해서 power shell에서 실행 & 설치  
```powershell
choco install microsoft-windows-terminal  
```  

## 2. WSL 설치  
[msdn](https://learn.microsoft.com/ko-kr/windows/wsl/install)  
```powershell  
wsl --install  
```  

위 명령으로 설치가 안 될 경우, 수동으로 설치해야 한다. ([공식문서]([이전 버전 WSL의 수동 설치 단계 | Microsoft Learn](https://learn.microsoft.com/ko-kr/windows/wsl/install-manual)))
	- PowerShell 관리자 권한 실행
	- dism 으로 wsl 설치
```shell
dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
```
	- window update (경우에 따라 스킵 가능)

## 3. Linux 커널 업데이트 패키지 다운로드 및 실행

[linux 커널 업데이트 패키지 다운로드 ](https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_x64.msi)


## 4. VM 기능 사용 설정
vm 설치 이후, 재부팅 필수  
```shell
dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart
```

## 5.  Ubuntu 설치
ms store에서 검색하여 설치 (20.04)
 
## 6. wsl2 기본 버전으로 지정

```shell  
wsl -l -v --버전확인  
wsl --set-default-version 2
wsl --set-version Ubuntu-20.04 

```  

#개발환경 #cli  #wsl

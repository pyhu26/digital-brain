1. zsh 설치
```  
sudo apt install zsh  
```  
2. oh my zsh 터미널로 설치  
```  
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```  
5. powerlevel10k theme 설치  
```zsh
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k
```
7. zshroc 설정파일 테마 변경
```
ZSH_THEME="robbyrussell" --> ZSH_THEME="powerlevel10k/powerlevel10k"
```
9. mesloLGS NFS 폰트 설치  
10. zsh 글꼴 변경  
```shell 
--settings.json
{
                "guid": "{c6eaf9f4-32a7-5fdc-b5cf-066e8a4b1e40}",
                "hidden": false,
                "name": "WSL2",
                "source": "Windows.Terminal.Wsl",
                "colorScheme": "Monokai Night",
                "fontFace": "MesloLGS NF"
            },
```
11. 터미널 기본 경로 변경
```shell
   {
                "guid": "{c6eaf9f4-32a7-5fdc-b5cf-066e8a4b1e40}",
                "hidden": false,
                "name": "WSL2",
                "source": "Windows.Terminal.Wsl",
                "colorScheme": "Monokai Night",
                "fontFace": "MesloLGS NF",
                "startingDirectory" : "d://source/"
   },
```
13. vscode 터미널 글꼴 변경 user>features>integrated font family  
  
#cli #zsh #powerlevel10k #mesloLGS 
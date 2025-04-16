# lab04![2025-04-16_08-12-08](https://github.com/user-attachments/assets/16f861d4-7ad6-4fc3-aeef-aff3db8e30dc)
![2025-04-16_08-20-29](https://github.com/user-attachments/assets/4c735c3c-9ee6-4706-a253-044c1fd4ef02)
![2025-04-16_08-21-31](https://github.com/user-attachments/assets/c0855f0b-ed1c-4702-8f6f-f18785ba57b2)

Ангелина@DESKTOP-9PH23VV MINGW64 ~/Documents/GitHub/PRACTICA-2025 (main)
$ #!/bin/bash

Ангелина@DESKTOP-9PH23VV MINGW64 ~/Documents/GitHub/PRACTICA-2025 (main)
$ 

Ангелина@DESKTOP-9PH23VV MINGW64 ~/Documents/GitHub/PRACTICA-2025 (main)
$ # Настройка переменных окружения

Ангелина@DESKTOP-9PH23VV MINGW64 ~/Documents/GitHub/PRACTICA-2025 (main)
$ export GITHUB_USERNAME=Ангелина

Ангелина@DESKTOP-9PH23VV MINGW64 ~/Documents/GitHub/PRACTICA-2025 (main)
$ export GITHUB_EMAIL=<адрес_почтового_ящика>     
bash: syntax error near unexpected token `newline'

Ангелина@DESKTOP-9PH23VV MINGW64 ~/Documents/GitHub/PRACTICA-2025 (main)
$ export GITHUB_TOKEN=<сгенирированный_токен>
bash: syntax error near unexpected token `newline'

Ангелина@DESKTOP-9PH23VV MINGW64 ~/Documents/GitHub/PRACTICA-2025 (main)
$ export EDITOR=<nano|vi|vim|subl>
bash: syntax error near unexpected token `newline'

Ангелина@DESKTOP-9PH23VV MINGW64 ~/Documents/GitHub/PRACTICA-2025 (main)
$

Ангелина@DESKTOP-9PH23VV MINGW64 ~/Documents/GitHub/PRACTICA-2025 (main)
$ # Переход в рабочую директорию

Ангелина@DESKTOP-9PH23VV MINGW64 ~/Documents/GitHub/PRACTICA-2025 (main)
$ cd ${GITHUB_USERNAME}/workspace
bash: cd: Ангелина/workspace: No such file or directory

Ангелина@DESKTOP-9PH23VV MINGW64 ~/Documents/GitHub/PRACTICA-2025 (main)
$ source scripts/activate
bash: scripts/activate: No such file or directory

Ангелина@DESKTOP-9PH23VV MINGW64 ~/Documents/GitHub/PRACTICA-2025 (main)
$

Ангелина@DESKTOP-9PH23VV MINGW64 ~/Documents/GitHub/PRACTICA-2025 (main)
$ # Настройка конфигурации hub

Ангелина@DESKTOP-9PH23VV MINGW64 ~/Documents/GitHub/PRACTICA-2025 (main)
$ mkdir -p ~/.config

Ангелина@DESKTOP-9PH23VV MINGW64 ~/Documents/GitHub/PRACTICA-2025 (main)
$ cat > ~/.config/hub <<EOF
> github.com:
> - user: ${GITHUB_USERNAME}
>   oauth_token: ${GITHUB_TOKEN}
>   protocol: https
> EOF

Ангелина@DESKTOP-9PH23VV MINGW64 ~/Documents/GitHub/PRACTICA-2025 (main)
$ git config --global hub.protocol https






















        #
        #                                                                          # 4. В ветке master измените комментарии
        #                                                                          git checkout master
        #                                                                          cat > hello_world.cpp <<EOF
        #                                                                          #include <iostream>
        #                                                                          #include <string>
        #
        #                                                                          int main() {
        #                                                                              sите pull + rebase, исправьте конфликты
        #                                                                              git checkout patch2
        #                                                                              git pull --rebase origin master
        #                                                                              # Исправьте конфликты вручную, если они есть
        #                                                                              git rebase --continue
        #
        #                                                                              # 6. Сделайте force push в ветку `patch2`        
        #                                                                              git push --force origin patch2
        #
        #                                                                              # 7. Вмержите pull-request `patch2 -> master`    
        #                                                                              hub merge patch2
        #                                                                              hub pr close patch2
        #
        #                                                                              # 8. Удалите локальную ветку `patch2`
        #                                                                              git branch -d patch2
        smudge = git-lfs smudge -- %f
        process = git-lfs filter-process
        required = true
        clean = git-lfs clean -- %f
[user]
        name = Ангелина
        email =
[hub]
        protocol = https
~/.gitconfig[+][RO] [unix] (08:45 16/04/2025)                                                                            175,101-108 Bot-- INSERT --

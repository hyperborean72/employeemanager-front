# Employeemanager front application

Install the Angular CLI globally - глобальная установка Angular CLI:
npm install -g @angular/cli

[or npm uninstall -g @angular/cli to deinstall, then run npm cache clean]

Установка будет произведена в 
C:\Users\<USER>\AppData\Roaming\npm\node_modules

В моем случае установилась CLI v.17.2.0

Однако Angular CLI requires a minimum Node.js version of v18.13

И эти версии Node.js на моем Win 7 не поддержваются

Как установить не последнюю, а предыдущую версию cli:

npm install -g @angular/cli@wished.version.here


Как обновиться:

1) To use the NodeJS update command, first Clear the npm cache:

npm cache clean -f

then install the n, Node's package manager:

npm install -g n

With the n tool installed, type the following command to update to the latest version:

n latest

2) Use the NVM utility to specify the version that you want to install. The following command installs NodeJS version 20.3.0:

npm install 20.3.0

сервис для определенного класса (employee в нашем случае) генерируется следующим образом:
ng generate service employee --skipTests=true


Если скрипт отказывается запускаться в Power Shell, найдите и удалитте 
C:\Users\Stepanov Andrey\AppData\Roaming\npm\ng.ps1
и удалите кэш then try clearing the npm cache at C:\Users\%username%\AppData\Roaming\npm-cache\
(наверное, результат тот же, что и командой npm cache clean -f)

ЛИБО исполнив



# Илья Белоножко, 1 подгруппа  
## Установить пакеты samba bind bind-utils и любой питоновский модуль  
`sudo apt-get install samba`  
`sudo apt-get install bind`  
`sudo apt-get install bind-utils`  
`sudo apt-get install python3-numpy`  
## Вывести: 2.1) Версию 2.2) Файлы пренадлежащие пакету 2.3) Зависимости  
`rpm -q samba`  
`rpm -ql samba`  
`rpm -qR samba`  
  Проверить службы установленных пакетов, еси не запущенны запустить, добавить в автозагрузку 3.1) можно ли включить и добавить в автозагрузку одной командой?  
проверка  
`sudo systemctl status smb`  
запуск  
`sudo systemctl start smb`  
добавить в автозагрузку  
`sudo systemctl enable smb`  
включить и добавить в автозагрузку одной командой  
`sudo systemctl enable --now smb`
## Найти и вывести конфигурационные файлы пакетов у которых они есть  
`rpm -ql bind | grep conf`  

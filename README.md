## Overview:

Cкрипт для бэкапирования и восстановления папок на сервере по SSH тоннелю 

## Installation:

```bash
git clone https://github.com/nn1k1kvn/br.git 
cd br
vi br 
chmod +x br
```
## Running:

```bash
./br -b
```
##  Options:

    -h                      Посмотреть помощь.
    -b                      Сохранить на локальную машину.
    -r                      Восстановить на удаленном сервере.
    
## Configuration:

```bash
LOCAL_PATH_RSA=''               # Путь к id-rsa openSSH на локальной машине
LOCAL_PATH_WORK=''              # Путь к рабочей папке на локальной машине
REMOTE_PATH_WORK=''             # Путь к рабочей папке на удаленном сервере
REMOTE_PATHS=''                 # Пути к папкам через пробел. Папки, которые нужно забэкапить
REMOTE_PATH='' 	                # Путь к текущей папке на удаленном сервере, которую нужно забэкапить
ARCHIVE_SUFFIX='_back'          # Добавляется к названию архива. Например, _back

REMOTE_IP='' 		            # IP адрес или хост удаленного сервера
REMOTE_PORT='22' 	            # Порт SSH на удаленном сервере. Обычно 22, но лучше поменять.     
REMOTE_USER='user'              # Пользователь на удаленном сервере

REMOTE_SUDO_PASS='' 		    # Пароль привелигированного пользователя на удаленном сервере. Чтобы использовать закомментируй в коде вызов функции getsudopass
ARCHIVE_NAME=""                 # Название архива. Конкатенируется из названия папки, суффикса и расширения .tar 
PASSPHRASE=""                   # Парольная фраза к приватному ключу. Чтобы использовать закомментируй в коде вызов функции 
```



## Feedback:
- Contact: [Miksha](https://fb.com/miksha.happy)

## You can show your gratitude to me :)
- Bitcoin wallet: --
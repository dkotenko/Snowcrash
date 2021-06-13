В папке исполняемый файл, к которому у нас нет доступа
В коде файла есть строка:
	strstr("token", "token") = "token"
то есть программа ожидает файл с таким названием.

Если подать аргумент token, появится сообщение: You may not access 'token'
У нас нет доступа к файлу, но мы можем создать ссылку с правами:
ln -sf /home/user/level08/token /tmp/test

token: quif5eloekouj29ke0vouxean
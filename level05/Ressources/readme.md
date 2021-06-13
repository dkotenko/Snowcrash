в папке /var/spool/mail есть письмо с текстом:
	*/2 * * * * su -c "sh /usr/sbin/openarenaserver" - flag05

сам скрипт:

#!/bin/sh

for i in /opt/openarenaserver/* ; do
        (ulimit -t 5; bash -x "$i")
        rm -f "$i"
done

Скрипт выполняет все файлы из папки /opt/openarenaserver. Добавим туда файл с выполнением getflag
Скрипт выполняется автоматически, т.к. добавлен в cron

token: viuaaale9huek52boumoomioc
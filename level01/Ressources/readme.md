Смотрим содержимое /etc/passwd, там лежит хэш пароля flag01:
	flag01:42hDRfypTqqnw:3001:3001::/home/flag/flag01:/bin/bash

Для подбора значения по хэш-сумме используется утилита john (John The Ripper (https://www.openwall.com/john/))
После перебора получаем значение: abcdefg

token: f2av5il02puano7naaf6adaaf
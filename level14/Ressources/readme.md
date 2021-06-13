Пропускаем getflag через ltrace:
	+++ exited (status 1) +++

В коде есть досрочный выход из программы.
Ставим брейкпоинт до выхода, далее делаем переход на строку с получением токена:
	b *main+74
	jump *main+1183

token: 7QiHafiNa3HVozsaXkawuYrTstxbpABHD8CPnHJ
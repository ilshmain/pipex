# yandex_algorithm
## Yandex.Algorithm home works

	Данная инструкция выполнится на Mac Os и Linux.
Pipex это проект , который воспроизводит поведение оболочки трубы |команды в C, используя функции pipe(), fork(), dup2()и execve().
	Общая идея: мы читаем из file1, выполняем cmd1 с file1 на входе, отправляем вывод в cmd2, который будет писать в
Outfile.
	Для запуска программы(основная часть) необходимо склонировать репозиторий. Выполнить команду make.
Создается исполняемый файл pipex, после чего необходимо выполнить ./pipex file1 cmd1 cmd2 outfile, программа будет вести себя точно так же, как эта строка в оболочке < file1 cmd1 | cmd2 > outfile.
Пример для проверки основной части: ./pipex file1 ls "cat -e" outfile.
	Для запуска бонусной части необходимо выполнить команду make bonus. В бонусной части мы можем выполнять множество команд.
Пример для проверки бонусной части: ./pipex file1 ls "cat -e" "cat -e" "cat -e"outfile.

[![forthebadge](https://forthebadge.com/images/badges/made-with-c.svg)](https://forthebadge.com)
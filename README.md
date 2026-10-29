# cicd-test
Используемые инструменты: Fedora Linux, Git, Github, Jenkins, Bash.
Git и Jenkins были установлены на локальном компьютере под управлением Fedora Linux.
Jenkins был запущен и настроен через веб-интерфейс:
http://localhost:8080
Для хранения исходного кода был создан общедоступный репозиторий GitHub. 
<img width="956" height="496" alt="изображение" src="https://github.com/user-attachments/assets/c641b623-49a8-414a-b543-04004f1cbb59" />
<img width="956" height="622" alt="изображение" src="https://github.com/user-attachments/assets/be4f2622-485b-4e82-a718-1a2e0dfeb828" />
Структура проекта:
cicd-test/
  README.md
  file1.txt
  file2.txt
  
1. Выполнение: job которая будет загружать код из мастер ветки Git в локальное хранилище. (скрипт представлен в job_1_download.txt) <img width="956" height="622" alt="изображение" src="https://github.com/user-attachments/assets/d266884c-2ea0-468d-b8bf-e751ea5cf4a5" />

2. Создать Job_2 которая удалит из проекта 1-2 файла. (скрипт представлен в файле job_2_delete.txt)
  
3. Создать Job_3 которая вернет проект в Git. (скрипт представлен в файле job_3_restore.txt)
4. Настройка того, чтобы Job_2 автоматически выполнялось после Job_1 <img width="623" height="424" alt="изображение" src="https://github.com/user-attachments/assets/c790a178-0fde-42fe-b978-4d3c9bc0be44" />
5. Настройка того, чтобы Job_3 автоматически выполнялось после Job_2 <img width="1301" height="388" alt="изображение" src="https://github.com/user-attachments/assets/72a95a39-7abd-4342-bd23-fc39c8a94661" />
6. Создание триггера на запуск Job_1 автоматически каждые 15 минут <img width="1301" height="388" alt="изображение" src="https://github.com/user-attachments/assets/4701719a-baa7-457c-8535-984db8a1da78" />
7. Все задания выполнились автоматически.<img width="1301" height="278" alt="изображение" src="https://github.com/user-attachments/assets/6c39135f-b869-411a-8569-bae1c702dfda" />




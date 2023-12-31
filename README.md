# PZ6_Lr3
Выполнил Панков Никита, ББМО-01-23

# C помощью ifconfig узнаем ip-адрес DVL. Cканируем ip-адрес с помощью nmap

![image](screenshots/1.png)
![image](screenshots/2.png)

# Сканируем DVL при помощи Openvas

![image](screenshots/3.png)

# XSS

1) Запускаем burpsuite. Переходим во вкладуку Proxy и включаем перехват.
2) Переходим на сайт с XSS уязвимостью
![image](screenshots/4.png)
3) После ввода данных и нажатия кнопки Add Comment в burpsuite увидим запрос
4) меняем последнюю строчку на name=Pankov&comment=<script>alert ("Pankov_XSS") </script >
![image](screenshots/5.png)
 
# CSRF

1) Переходим на сайт с CSRF уязвимостью
![image](screenshots/6.png)
3) После ввода данных и нажатия кнопки Add Comment в burpsuite увидим запрос
4) Меняем последнюю строчку на item=pen&quantity=1234567890
![image](screenshots/7.png)


# Устанавливаем и запускаем OWASP ZAP. Запускаем автоматическое сканирование и исследуем результат SQL injection

![image](screenshots/8.png)

# Запускаем metasploit. Настраиваем RHOST, USERNAME, PASS_FILE, STOP_ON_SUCCESS. Запускаем

![image](screenshots/9.png)

# Подключаемся к SSH. Заходим в mysql. Находим файл с логином и паролем в зашифрованном виде. Создаем txt файл в который вписываем зашифрованный пароль. Запускаем JohnTheRipper и ищем пароль 

![image](screenshots/10.png)

# Анализ трафика с помощью wireshark

![image](screenshots/11.png)

# Snort правила

![image](screenshots/12.png)

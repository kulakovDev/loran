## Loran Lab
Емулятор вимірювальної частини LORAN надається у вигляді Docker image під назвою iperekrestov/university/loran-emulation-service. Щоб запустити емулятор, виконайте наступні кроки:
1. Завантажте Docker image з Docker Hub:  
   ````
   docker pull iperekrestov/university:loran-emulation-service
   ````
2. Запустіть Docker контейнер, використовуючи наступну команду:  
   ````
   docker run --name loran-emulator -p 4002:4000 iperekrestov/university:loran-emulation-service 
   ```` 

Веб-додаток підключається до WebSocket сервера та зчитує дані про часи отримання сигналів базовими станціями. Обробляє дані отримані через вебсокет і відображає  положення об'єкта і базових станцій на графіку.  

![Loran1](./screenshots/loran1.png)

![Loran2](./screenshots/loran2.png)

![Code1](./screenshots/code1.png)

Обробка даних

![Code2](./screenshots/code2.png)

Розрахунок позиції об'єкта

![Code3](./screenshots/code3.png)

![Code4](./screenshots/code4.png)

![Code5](./screenshots/code5.png)

Відображення даних на графіку

![Code6](./screenshots/code6.png)

Можливість зміни параметрів вимірювальної частини радара за допомогою API запитів.  

![Code7](./screenshots/code7.png)




# PWR Racing Team Dział Software
## Zadanie rekrutacyjne nr.1
Plik "main.c" z kodem znajduje się w "Core/Src/main.c" <br>
Poniżej znajdują się zrzuty ekranu z konfiguracji/programu

### Zewnętrzne źródło taktowania 16 MHz
![image](https://github.com/user-attachments/assets/6a01e641-aff6-4208-8e57-a35f2ad0eff5)
<br>
![image](https://github.com/user-attachments/assets/9f64ec7e-39c8-4450-b56a-512e6c5f88e9)


### Port PA5 skonfigurowany jako GPIO Output
![image](https://github.com/user-attachments/assets/fa1e9b9d-a3eb-4034-8f83-e2e9e699ba50)

### Konfiguracja TIM6 do mrugania diodą
![image](https://github.com/user-attachments/assets/e43d220f-4b13-4b79-b406-49152cd8035b)

Taktowanie zegara 16 MHz -> Preskaler ustawiamy na 16 000 -> Otrzymujemy 1 KHz -> Rejestr ustawiamy na 100 żeby otrzymać przerwanie co 0,1 sekundy. Każde przerwanie to zmiana stanu, więc dioda miga co 0,2 sekundy, lub z częstotliwością 5 Hz

### Konfiguracja Independent-Watchdoga
![image](https://github.com/user-attachments/assets/bd7cadca-ddd4-4294-ba2d-0fe30648eedb)


### Funkcja zmieniająca stan diody z każdym przerwaniem
![image](https://github.com/user-attachments/assets/c1ec9a43-010b-4e2f-9f38-3bdece1855a4)

### Załączenie timera TIM6
![image](https://github.com/user-attachments/assets/5f0d251e-5e84-4d9e-9e38-c5a59e1ee3fa)

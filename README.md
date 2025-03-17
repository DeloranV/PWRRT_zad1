# PWR Racing Team Dział Software
## Zadanie rekrutacyjne nr.1
Plik "main.c" z kodem znajduje się w "Core/Src/main.c" <br>
Poniżej znajdują się zrzuty ekranu z konfiguracji/programu

### Wewnętrzne źródło taktowania 16 MHz

### Port PA5 skonfigurowany jako GPIO Output

### Konfiguracja TIM6 do mrugania diodą
Taktowanie zegara 16 MHz -> Preskaler ustawiamy na 16 000 -> Otrzymujemy 1 KHz -> Rejestr ustawiamy na 100 żeby otrzymać przerwanie co 0,1 sekundy. Każde przerwanie to zmiana stanu, więc dioda miga co 0,2 sekundy, lub z częstotliwością 5 Hz

### Konfiguracja Independent-Watchdoga

### Funkcja zmieniająca stan diody z każdym przerwaniem

### Załączenie timera TIM6

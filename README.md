# System rozpoznawania typów ubrań 
Projekt przedstawia system do automatycznego rozpoznawania elementów garderoby na obrazach pochodzących z kamery internetowej lub plików graficznych. System wykorzystuje model detekcji obiektów YOLOv8n, umożliwiając wykrywanie i klasyfikację różnych typów ubrań w czasie zbliżonym do rzeczywistego. Projekt został zrealizowany w ramach przedmiotu „Systemy rozpoznawania mowy i obrazu”.

Rozpoznawane klasy odzieży:
- Tshirt
- shirt
- pants
- short
- skirt
- dress
- sweater
- jacket

## Instrukcja uruchomienia

### Część badawcza – trening i analiza
1. Otworzyć notatnik `Analiza_i_Trening.ipynb` w środowisku obsługującym Jupyter Notebook (np. Google Colab lub lokalnie).
2. Uruchomić wszystkie komórki notatnika (opcja „Run all”).
3. Po zakończeniu procesu treningu i walidacji wytrenowane wagi modelu zostaną zapisane do pliku `best.pt`.

### Część demonstracyjna – aplikacja
1. Otworzyć notatnik `Aplikacja_Demo.ipynb` w tym samym środowisku.
2. Upewnić się, że plik `best.pt` znajduje się w katalogu projektu.
3. Uruchomić wszystkie komórki notatnika.
4. Po wykonaniu ostatniej komórki uruchomiony zostanie interfejs użytkownika aplikacji, umożliwiający wgranie obrazu lub użycie kamery internetowej.


## ⚙️ Wymagania i instalacja

Projekt został przygotowany w środowisku **Python 3.x** (zalecane Google Colab).

Wykorzystywane biblioteki:
- ultralytics – implementacja modelu YOLOv8 oraz narzędzia do treningu, walidacji i inferencji,
- roboflow – pobieranie i obsługa zbioru danych,
- gradio – interfejs użytkownika aplikacji demonstracyjnej,
- opencv-python – obsługa obrazów,
- numpy – operacje numeryczne.

Instalacja zależności:
```bash
pip install ultralytics roboflow gradio opencv-python numpy

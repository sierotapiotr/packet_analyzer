# packet_analyzer
Program służący do analizy pakietów:
- Wczytuje plik .pcap jako argument wywołania. 
- Oblicza liczbę pakietów i liczbę bajtów (bez nagłówka warstwy 2) niesionych przez wczytane pakiety z podziałem na protokół warstwy 3.
- Pakiety IPv6 są pomijane (oznaczenie SKIPPED).
- Możliwość szczegółowego logowania DEBUG.
- Możliwość wygenerowania pliku z wykresem typu słupkowego (bar chart), gdzie na osi 0Y są protokoły warstwy 3, a na osi 0X liczba pakietów.

Przykładowe użycie:
python app.py --input example1.pcap --debug --barchart chart.png

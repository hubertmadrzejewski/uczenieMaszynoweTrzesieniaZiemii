# Earthquake Predictor 

Earthquake Predictor to aplikacja napisana w języku Python, która wykorzystuje techniki uczenia maszynowego do przewidywania magnitudy trzęsień ziemi na podstawie danych geograficznych. Zawiera klasę o nazwie EarthquakePredictor, która obejmuje funkcje związane z przygotowaniem danych, treningiem modelu, ewaluacją modelu oraz różnymi metodami analizy danych i wizualizacji.


## Instalacja

Aby korzystać z Earthquake Predictor, musisz mieć zainstalowanego Pythona na swoim komputerze. Zainstaluj wymagane zależności za pomocą poniższej komendy:

```bash
pip install pandas scikit-learn matplotlib seaborn folium
```
## Zastosowanie

**Earthquake Predictor** ma na celu wspomaganie analizy oraz prognozowania trzęsień ziemi na podstawie dostępnych danych geograficznych. Poniżej przedstawiono kilka zastosowań tej aplikacji:

**Przewidywanie Magnitudy**: Umożliwia prognozowanie magnitudy trzęsień ziemi na podstawie danych o lokalizacji geograficznej.

**Analiza Potencjalnych Zagrożeń**: Earthquake Predictor może być używany do analizy obszarów pod kątem potencjalnych zagrożeń związanych z trzęsieniami ziemi.

**Zapobieganie Skutkom Trzęsień Ziemi**: Przewidywanie magnitudy pozwala na przygotowanie się do ewentualnych skutków trzęsień ziemi i podjęcie odpowiednich działań zapobiegawczych.

**Badania Naukowe**: Aplikacja może służyć jako narzędzie badawcze do analizy danych dotyczących trzęsień ziemi i poszukiwania nowych zależności.

**Ostrzeganie Społeczności**: W przypadku potencjalnego zagrożenia trzęsieniem ziemi, Earthquake Predictor może wspomagać proces ostrzegania społeczności.

## Użycie 

Główną klasą, EarthquakePredictor, można wykonywać różne zadania związane z prognozowaniem trzęsień ziemi i analizą danych. Zaimportuj klasę do swojego skryptu Pythona lub notatnika Jupyter i stwórz instancję, podając ścieżkę do swojego zbioru danych o trzęsieniach ziemi
```python
from earthquake_predictor import EarthquakePredictor

# Przykładowe użycie
earthquake_predictor = EarthquakePredictor('ścieżka/do/twojego/zestawu/danych.csv')

# Kontynuuj pracę z dostępnymi metodami, takimi jak analiza danych, trening modelu itp.

```
## Metody klasy
### Metody analizy danych

*'display_summary_statistics'*: Wyświetl podsumowanie statystyk dotyczących zestawu danych o trzęsieniach ziemi.

*'display_info'*: Wyświetl informacje na temat zestawu danych o trzęsieniach ziemi.

*'check_missing_values'*: Sprawdź, czy w zestawie danych występują brakujące wartości.

*'display_data_distribution'*: Wyświetl rozkład magnitud trzęsień ziemi.

### Metody przetwarzania danych

*'remove_not_needed_columns'*: Usuń określone kolumny ze zbioru danych.

### Metody wizualizacji

*'display_box_plots'*: Wyświetl wykresy pudełkowe dla wybranych kolumn.

*'display_correlation_matrix'*: Wyświetl mapę cieplną macierzy korelacji.

### Metody treningu modelu i ewaluacji

*'train_linear_regression'*: Trenuj model regresji liniowej.

*'train_random_forest'*: Trenuj model lasu losowego z określonymi parametrami.

*'gradient boosting'*: Trenuj model w postaci kombinacji słabych modeli, tzw. drzew decyzyjnych.

*'decision tree'*: Trenuj model za pomocą drzewka decyzyjnego.

*'adaptive boosting'* model oparty na trening wielu słabych klasyfikatorów i kombinowanie ich, aby uzyskać silny klasyfikator..

*'compare_models'*: Porównaj wydajność wytrenowanych modeli.


### Dopasowanie modeli
RMSE (Root Mean Square Error)

MAE (Mean Absolute Error)

Niższe wartości RMSE i MAE wskazują na lepsze dopasowanie modelu do danych testowych, czyli na mniejsze błędy przewidywań.

RMSE daje większą wagę większym błędom, więc jeśli Twój model ma niski RMSE, oznacza to, że radzi sobie dobrze z minimalizacją dużych błędów w przewidywaniach.

MAE daje równą wagę wszystkim błędom, więc niski MAE oznacza, że model na ogół dokonuje przewidywań bliskich wartościom rzeczywistym, bez znaczącego wpływu ekstremalnych błędów.
Najlepszy model to ten, który osiąga najniższe wartości RMSE i MAE na zestawie testowym.


### Ręczne testowanie predykcji
*'manual_prediction_test'*: Ręczne testowanie wytrenowanego modelu na nowych danych.


Dla szczegółowych wyjaśnień każdej metody odwołaj się do komentarzy w pliku earthquake_predictor.py.

## Licencja

Ten projekt jest licencjonowany na zasadach [MIT](https://choosealicense.com/licenses/mit/).

### [Metoda self-training](https://scikit-learn.org/stable/modules/generated/sklearn.semi_supervised.SelfTrainingClassifier.html)

#### Eksperyment
1. Weź dowolny zbiór danych dotyczący klasyfikacji.
2. Podziel wybrany zbiór na treningowy i testowy.
3. Dla pewnego procenta _k_ obserwacji w zbiorze treningowym usuwamy etykiety. Rozważ różne wartośći _k_, np. 20%, 50%, 80%, 90%. Czyli 90% oznacza, że 90% obserwacji ma etykietę "?", zaś 10% obserwacji ma etykietę "0" lub "1".
4. Dopasuj modele:
   a) metoda naiwna: model bazujący tylko na obserwacjach gdzie została etykieta
   b) metoda semi-supervised: model bazujący na self-training, który wykorzystuje obserwacje bez etykiety.
5. Sprawdź oba modele na danych testowych.

Cały eksperyment powtórz dla przynajmniej dwóch zbiorów danych. 

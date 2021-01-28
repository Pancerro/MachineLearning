<div>
  <h1>Analiza danych z pakietem Pandas </h1>
  <h2>W tym zadaniu analizowałem dane, za pomocą pakietu pandas </h2>
  <ul>
    <li> Średnia cena samochodow za pomoca funkcji mean() </li>
    <li> Mediana przebiegu samochodow za pomoca funkcju median() </li>
    <li> Wyswietlenie unikatowych wartosci, np. marki za pomoca funkcji drop_duplicates() </li>
    <li> Wykres prezentujaca ilosc samochodow w danej cenie za pomoca .plot.hist() </li>
    <li> Wykres prezentujacy stosunek przebiegu do ceny samochodoów za pmoca plot.scatter(x='przebieg',y='cena) </li>
    <li> Wyswiet;enie trzech losowych wierszy za pomoca sample(3) </li>
    <li> Posortowanie listy samochodow za pomoca sort_values('nazwa_kolumny') </li>
    <li> Wyswietlenie liczby danej wartosci za pomoca value_counts() </li>
    <li> Wyswietlenie wybranych kolumn za pomoca iloc[] </li>
    <li> Uzywanie warunkow do wyswietlania tylko tych wartosc co spelnienia podane warunki za pomoca funkcjji loc[] </li>
  </ul>
</div>
#7 Wyswietlenei listy ssamochodow po cenie
print(df.sort_values('cena'))
#8 Wyswietlenie liczby samochodow nalezacych do danej marki
print(df['marka'].value_counts())
#9 wyswietenie listy tylko z kolumnami 1, 2 i 5
print(df.iloc[:,[1,2,5]])
#10 wyswietlenie marki wojowodztwa i ceny samochodw tanszych niz 1000
print(df.loc[df['cena'] < 1000, ['marka','wojewodztwo','cena']])

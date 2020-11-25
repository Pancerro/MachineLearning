open - służy do otwarcia pliku
close - służy do zamkniecia pliku
try:
finally:
- służą np. do zamkniecia pliku
with open('.txt') as reader: - służy do zamkniecia pliku po opusczeniu with bloku
'r'	- Otwórz do czytania (domyślnie)
'w'	- Otwórz do zapisu, najpierw obcinając (nadpisując) plik
'rb' lub 'wb' -	Otwórz w trybie binarnym (odczyt / zapis przy użyciu danych bajtowych)
type(file) -  zwróci TextIOWrapperobiekt pliku
.read(size=-1) - Odczytuje z pliku na podstawie liczby sizebajtów. Jeśli żaden argument nie jest przekazywana lub Noneczy -1zostanie przyjęta, wtedy cały plik jest odczytywany.
.readline(size=-1)- Odczytuje maksymalnie sizeliczbę znaków z wiersza. To trwa do końca linii, a następnie zawija się z powrotem. Jeśli żaden argument nie jest przekazywana lub Noneczy -1zostanie przyjęta, wtedy cała linia (lub reszta linii) jest odczytywany.
.readlines() - Czyta pozostałe wiersze z obiektu pliku i zwraca je jako listę.
list(f) - zwraca liste obiektow

with open('.txt', 'r') as reader:
     line = reader.readline()
     while line != '': 
         print(line, end='')
         line = reader.readline()
 - iteracja po każdej linii
 
.write(string) - Spowoduje to zapisanie ciągu znaków do pliku.
.writelines(seq) - To zapisuje sekwencję do pliku. Żadne zakończenia linii nie są dołączane do każdego elementu sekwencji. To do Ciebie należy dodanie odpowiednich końcówek linii.

with open('AdrianLawecki.png', 'rb') as byte_reader:
     print(byte_reader.read(1))
     print(byte_reader.read(3))
     print(byte_reader.read(2))
     print(byte_reader.read(1))
     print(byte_reader.read(1))
     
  - przeczytanie pliku nagłowkowego w png
  
    a_writer.write('\nBeagle') - dodowanie nowje linii na koniec pliku
    with open(d_path, 'r') as reader, open(d_r_path, 'w') as writer:
    newLine = reader.readlines()
    writer.writelines(reversed(newLine))
    
    - połaczenie plików 
    

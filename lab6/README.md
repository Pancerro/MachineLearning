open - służy do otwarcia pliku </br>
close - służy do zamkniecia pliku </br>
try:</br>
finally: - służą np. do zamkniecia pliku</br>
with open('.txt') as reader: - służy do zamkniecia pliku po opusczeniu with bloku</br>
'r'	- Otwórz do czytania (domyślnie)</br>
'w'	- Otwórz do zapisu, najpierw obcinając (nadpisując) plik</br>
'rb' lub 'wb' -	Otwórz w trybie binarnym (odczyt / zapis przy użyciu danych bajtowych)</br>
type(file) -  zwróci TextIOWrapperobiekt pliku</br>
.read(size=-1) - Odczytuje z pliku na podstawie liczby sizebajtów. Jeśli żaden argument nie jest przekazywana lub Noneczy -1zostanie przyjęta, wtedy cały plik jest odczytywany.</br>
.readline(size=-1)- Odczytuje maksymalnie sizeliczbę znaków z wiersza. To trwa do końca linii, a następnie zawija się z powrotem. Jeśli żaden argument nie jest przekazywana lub Noneczy -1zostanie przyjęta, wtedy cała linia (lub reszta linii) jest odczytywany.</br>
.readlines() - Czyta pozostałe wiersze z obiektu pliku i zwraca je jako listę.</br>
list(f) - zwraca liste obiektow</br>

with open('.txt', 'r') as reader:</br>
     line = reader.readline()</br>
     while line != '': </br>
         print(line, end='')</br>
         line = reader.readline() - iteracja po każdej linii</br>
 
.write(string) - Spowoduje to zapisanie ciągu znaków do pliku.</br>
.writelines(seq) - To zapisuje sekwencję do pliku. Żadne zakończenia linii nie są dołączane do każdego elementu sekwencji. To do Ciebie należy dodanie odpowiednich końcówek linii.</br>

with open('AdrianLawecki.png', 'rb') as byte_reader:</br>
     print(byte_reader.read(1))</br>
     print(byte_reader.read(3))</br>
     print(byte_reader.read(2))</br>
     print(byte_reader.read(1))</br>
     print(byte_reader.read(1))- przeczytanie pliku nagłowkowego w png</br>
  
a_writer.write('\nBeagle') - dodowanie nowje linii na koniec pliku</br>
with open(d_path, 'r') as reader, open(d_r_path, 'w') as writer:</br>
newLine = reader.readlines()</br>
writer.writelines(reversed(newLine))  - połaczenie plików </br>
    

<h1>Laboratorium 8</h1>

<h6> JSON </h6>
<p> 
  json.dump(data, write_file) - zapisuje dane z jsona, zserializowane, rzutowane na odpowiedni tryb danych  i zapisuje do pliku
</p>
<p> 
  json_string = json.dumps(data) - dziala jak dump, tylko nie zapisuje do pliku, a np. do zmiennej
</p>
json.dumps(data, indent=4) - indent oby okreslic rozmiar wciecia
<p>
  Deserializacja JSON - polega na tym by odkodowac ponownie zakodowany json
</p>
<p> 
  Na danych JSON mozna operowac jak na normalnych danych np.  todos_by_user[todo["userId"]] += 1 - mozna odwolac sie do kolumny userId i dzieki temu policzyc ile razy dany uzytkownik wystapil w tym 
</p>

<h6> CSV </h6>
<p> 
   csv.reader - sluzy do czytania pliku csv - mozemy okreslic separator
</p>
<p> 
  as csv_file - pozwala czytac pliki jako csv
</p>
<p>
  csv.DictReader - robi to co csv.reader, tylko zakłada się, że pierwsza linia pliku CSV zawiera klucze używane do budowania słownika
</p>
<p>
  csv.writer - mozna uzyc do zapisania do pliku 
</p>
<p>
  fieldnames - nazwy kolumn, ktore uzywa csv.DictWriter(csv_file, fieldnames=fieldnames) do zapisu
</p>
<p>
  writerow - sluzy do pisania jednego wiersza, mozna okreslic jkaie pola ma dokladnie napisac np. imie 
</p>
<p>
  pandas.read_csv('hrdata.csv') - sluzy to przeczytania plikow csv
</p>
<p>
   index_col='Name' - dodanie go do  pandas.read_csv sprawi ze zmienimi kolumne po ktorej indeksujemy na np. name
</p>
<p>
            header=0 - uzywa aktualne nazwy kolumn w pliku csv </br>
            names=['Employee', 'Hired','Salary', 'Sick Days']) - nadpisujemy nowe nazwy kolumn
</p>
<p>
  df.to_csv('hrdata_modified.csv') - sluzy do zapisu pliku css
</p>

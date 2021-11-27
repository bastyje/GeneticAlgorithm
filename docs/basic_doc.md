# Genetic Algorithm

## Og�lne za�o�enia

Program Genetic Algorithm implementuje algorytm genetyczny, kt�ry umo�liwia znalezienie maksimum funkcji dopasowania jednej zmiennej w zadanej dziedzinie liczb ca�kowitych.

### Genetic Algorithm implementuje takie operacje jak:
- reprodukcja z u�yciem nieproporcjonalnej ruletki
- krzy�owanie proste
- mutacja r�wnomierna

### U�ytkownik ma wp�yw na:
- wz�r przekazanej funkcji
- rozmiar populacji
- parametry krzy�owania
- parametry mutacji

### Wynik dzia�ania programu jest na bie��co wizualizowany za pomoc� wykres�w:
- �redniego przystosowania
- maksymalnego przystosowania
- minimalnego przystosowania
- wykresu funkcji w zadanym wcze�niej przedziale

## Reprodukcja

1. Na podstwie funkcji przystosowania obliczane jest przystosowanie ka�dego osobnika. *Prawdopodobie�stwo wyboru* danego osobnika do reprodukcji obliczane jest poprzezpodzielenie warto�ci funkcji przystosowania przez sum� warto�ci funkcji przystosowania wszystkich element�w populacji.
2. Ze starej populacji wybierane s� elementy nowej populacji w liczbie r�wnej cz�onkom poprzedniej populacji. Element wybierany jest z prawdopodobie�stwem r�wnym *prawdopodobie�stwu wyboru*.
3. Elementy wybrane zapisywane s� jako populacja tymczasowa.
4. Operacja reprodukcji si� ko�czy.

## Krzy�owanie

1. Z otrzymanej populacji wybierane s� w spos�b losowy pary osobnik�w.
2. Krzy�owanie jest przeprowadzane z prawdopodobie�stwem r�wnym zadanemu prawdopodobie�stwu krzy�owania.
3. Dla ci�gu kodowego o d�ugo�ci l, w spos�b losowy z jednostajnym rozk�adem prawdopodobie�stwa wybierana jest liczba *i* z zakresu 1-(l - 1), kt�ra reprezentuje pierwszy indeks ci�gu kodowego, kt�ry podlega operacji krzy�owania.
4. Elementy ci�gu kodowego z zakresu *i*-(l - 1) zamieniaj� si� pomi�dzy sparowanymi ci�gami kodowymi.
5. Operacja krzy�owania si� ko�czy.

## Mutacja

1. Operacja jest przeprowadzana na ka�dym po kolei ci�gu kodowym (chromosomie) z populacji.
2. Nast�puje iteracja po ka�dym allelu chromosomu.
3. Dla ka�dego allela operacja mutacji jest przeprowadzana z prawdopodobie�stwem r�wnym zadanemu prawdopodobie�stwu mutacji.
4. Warto�� allela zmieniana jest na przeciwn�.
5. Operacja mutacji si� ko�czy
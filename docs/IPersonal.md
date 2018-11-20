# Описание интерфейса IPersonal
Интерфейс предназначен для работы с методами класса Personal

## Реализация интерфейса
* +Add (Personal: [Personal](https://github.com/Tyukhaev/BTP/blob/master/docs/Personal.md "объект класса Personal")): Int — функция, добавляющая работника в базу данных. Параметр «[Personal](https://github.com/Tyukhaev/BTP/blob/master/docs/Personal.md "объект класса Personal")» — работник, 
которую необходимо добавить в БД;
* +Save (Personal: [Personal](https://github.com/Tyukhaev/BTP/blob/master/docs/Personal.md "объект класса Personal")): Bool — функция, редактирующая данные о работнике. Параметр «[Personal](https://github.com/Tyukhaev/BTP/blob/master/docs/Personal.md "объект класса Personal")» — 
работник, которую необходимо редактировать в БД;
* +FindByID(ID: Int): [Personal](https://github.com/Tyukhaev/BTP/blob/master/docs/Personal.md "объект класса Personal")  — функция, осуществляющая поиск работников в базе данных по ID и возвращающая найденный, если такой есть. 
* +Delete(ID:int): Bool – функция удаляет работника.
* +GetPersonals(IDPersonal : int, sorting : String, filtering : String, sortingA : boolean, count : int, page : int) : List<[Personal](https://github.com/Tyukhaev/BTP/blob/master/docs/Personal.md "объект класса Personal")> - функция, возвращающая общее количество работников,удовлетворяющих заданным параметрам.
Параметры:
	* sortintg: string — отвечает, по какому полю будет сортироваться список;
  
	* sortingA: bool — отвечает, по возрастанию или убыванию будут сортироваться элементы;
  
	* filtering: string — отвечает за фильтрацию;
  
	* count: int — отвечает, сколько элементов необходимо показать;
  
	* page: int — отвечает, с какой страницы начинать поиск элементов.
	

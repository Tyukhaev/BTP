# Описание интерфейса IBootcamp
Интерфейс предназначен для работы с методами класса Bootcamp

## Реализация интерфейса
* +Add (Bootcamp: [Bootcamp](https://github.com/Tyukhaev/BTP/blob/master/docs/Bootcamp.md "объект класса Bootcamp")): Int — функция, добавляющая буткемп в базу данных. Параметр «[Bootcamp](https://github.com/Tyukhaev/BTP/blob/master/docs/Bootcamp.md "объект класса Bootcamp")» — буткемп, 
которую необходимо добавить в БД;
* +Save (Procedure: [Bootcamp](https://github.com/Tyukhaev/BTP/blob/master/docs/Bootcamp.md "объект класса Bootcamp")): Bool — функция, редактирующая данные о буткемпе. Параметр «[Bootcamp](https://github.com/Tyukhaev/BTP/blob/master/docs/Bootcamp.md "объект класса Bootcamp")» — 
буткемп, которую необходимо редактировать в БД;
* +FindByID(ID: Int): Bootcamp  — функция, осуществляющая поиск буткемпы в базе данных по ID и возвращающая найденный, если такой есть. 
* +AddPersonal(IDBootcmap : int, IDPersonal : int) - функция добавляет работников на буткемп в БД. Параметр IDBootcmap и IDPersonal – ID по которому будет осуществлен поиск в базе.
* +AddSponsor(IDBootcamp : int, IDSponsor : int) - функция добавляет спонсора на буткемп в БД. Параметр IDBootcmap и IDSponsor – ID по которому будет осуществлен поиск в базе.
* +AddTeam(IDBootcamp : int, IDTeam : int) - функция добавляет команду на буткемп в БД. Параметр IDBootcmap и IDTeam – ID по которому будет осуществлен поиск в базе.
* +Delete(ID:int): Bool – функция удаляет буткемп.
* +DeletePersonal(IDBootcamp : int, ID Personal : int) - удаление работника из буткемпа.
* +DeleteSponsor(IDBootcamp : int, ID Sponsor : int) - удаление спонсора из буткемпа.
* +DeleteTeam(IDBootcamp : int, IDTeam : int) - удаление команды из буткемпа.
* +GetPersonals(IDBootcamp : int, sorting : String, filtering : String, sortingA : boolean, count : int, page : int) : List<(https://github.com/Tyukhaev/BTP/blob/master/docs/Personal.md "объект класса Personal")> - функция, возвращающая общее количество работников, удовлетворяющих заданным параметрам.
* +GetBootcamps(IDBootcamp : int, sorting : String, filtering : String, sortingA : boolean, count : int, page : int) : List<(https://github.com/Tyukhaev/BTP/blob/master/docs/Bootcamp.md "объект класса Bootcamp")> - функция, возвращающая общее количество буткемпов,удовлетворяющих заданным параметрам.
Параметры:
	* sortintg: string — отвечает, по какому полю будет сортироваться список;
  
	* sortingA: bool — отвечает, по возрастанию или убыванию будут сортироваться элементы;
  
	* filtering: string — отвечает за фильтрацию;
  
	* count: int — отвечает, сколько элементов необходимо показать;
  
	* page: int — отвечает, с какой страницы начинать поиск элементов.
	
* +GetSponsors(IDBootcamp : int, sorting : String, filtering : String, sortingA : boolean, count : int, page : int) : List<(https://github.com/Tyukhaev/BTP/blob/master/docs/Sponsor.md "объект класса Sponsor")> - функция, возвращающая список спонсоров буткемпов с заданными параметрами.
* +GetTeams(IDBootcamp : int, sorting : String, filtering : String, sortingA : boolean, count : int, page : int) : List<(https://github.com/gogganesko/Orho/blob/master/docs/Team.md "объект класса Team")> - функция,возвращающая список команд буткемпов с заданным параметрам.

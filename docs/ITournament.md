# Описание интерфейса ITournament
Интерфейс предназначен для работы с методами класса Tournament

## Реализация интерфейса
* +Add (Tournament: [Tournament](https://github.com/Tyukhaev/BTP/blob/master/docs/Tournament.md "объект класса Tournament")): Int — функция, добавляющая турнир в базу данных. Параметр «[Tournament](https://github.com/Tyukhaev/BTP/blob/master/docs/Tournament.md "объект класса Tournament")» — турнир, 
которую необходимо добавить в БД;
* +Save (Tournament: [Tournament](https://github.com/Tyukhaev/BTP/blob/master/docs/Tournament.md "объект класса Tournament")): Bool — функция, редактирующая данные о турнире. Параметр «[Tournament](https://github.com/Tyukhaev/BTP/blob/master/docs/Tournament.md "объект класса Tournament")» — 
турнир, которую необходимо редактировать в БД;
* +FindByID(ID: Int): [Tournament](https://github.com/Tyukhaev/BTP/blob/master/docs/Tournament.md "объект класса Tournament")  — функция, осуществляющая поиск турниров в базе данных по ID и возвращающая найденный, если такой есть. 
* +AddGame(IDTournament : int, IDGame : int) - функция добавляет игру на турнир в БД. Параметр IDTournament и IDGame – ID по которому будет осуществлен поиск в базе.
* +AddTeam(IDTournament : int, IDTeam : int) - функция добавляет команду на турнир в БД. Параметр IDTournament и IDTeam – ID по которому будет осуществлен поиск в базе.
* +Delete(ID:int): Bool – функция удаляет турнир.
* +DeleteGame(IDTournament : int, IDGame : int) - удаление игры у турнира.
* +DeleteTeam(IDTournament : int, IDTeam : int) - удаление команды на турнире.
* +GetTeam(IDTournament : int, sorting : String, filtering : String, sortingA : boolean, count : int, page : int) : List<[Team](https://github.com/gogganesko/Orho/blob/master/docs/Team.md "объект класса Team")> - функция, возвращающая список команд турнира, удовлетворяющих заданным параметрам.
* +GetTournaments(IDTournament : int, sorting : String, filtering : String, sortingA : boolean, count : int, page : int) : List<[Tournament](https://github.com/Tyukhaev/BTP/blob/master/docs/Tournament.md "объект класса Tournament")> - функция, возвращающая общее количество турниров,удовлетворяющих заданным параметрам.
Параметры:
	* sortintg: string — отвечает, по какому полю будет сортироваться список;
  
	* sortingA: bool — отвечает, по возрастанию или убыванию будут сортироваться элементы;
  
	* filtering: string — отвечает за фильтрацию;
  
	* count: int — отвечает, сколько элементов необходимо показать;
  
	* page: int — отвечает, с какой страницы начинать поиск элементов.
	
* +GetGames(IDTournament : int, sorting : String, filtering : String, sortingA : boolean, count : int, page : int) : List<[Game](https://github.com/Tyukhaev/BTP/blob/master/docs/Game.md "объект класса Game")> - функция,возвращающая список игр турнира с заданным параметрам.

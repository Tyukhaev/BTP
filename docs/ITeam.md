# Описание интерфейса ITeam
Интерфейс предназначен для работы с методами класса Team

## Реализация интерфейса
* +Add (Team: [Team](https://github.com/Tyukhaev/BTP/blob/master/docs/Team.md "объект класса Team")): Int — функция, добавляющая команду в базу данных. Параметр «[Team](https://github.com/Tyukhaev/BTP/blob/master/docs/Team.md "объект класса Team")» — команда, 
которую необходимо добавить в БД;
* +Save (Team: [Team](https://github.com/Tyukhaev/BTP/blob/master/docs/Team.md "объект класса Team")): Bool — функция, редактирующая данные о команде. Параметр «[Team](https://github.com/Tyukhaev/BTP/blob/master/docs/Team.md "объект класса Team")» — 
команда, которую необходимо редактировать в БД;
* +FindByID(ID: Int): [Team](https://github.com/Tyukhaev/BTP/blob/master/docs/Team.md "объект класса Team")  — функция, осуществляющая поиск команд в базе данных по ID и возвращающая найденный, если такой есть. 
* +AddGame(IDTeam : int, IDGame : int) - функция добавляет игру к команде в БД. Параметр IDTeam и IDGame – ID по которому будет осуществлен поиск в базе.
* +AddSponsor(IDTeam : int, IDSponsor : int) - функция добавляет спонсора в команду в БД. Параметр IDTeam и IDSponsor – ID по которому будет осуществлен поиск в базе.
* +AddPlayer(IDTeam : int, IDPlayer : int) - функция добавляет игрока в команду в БД. Параметр IDTeam и IDPlayer – ID по которому будет осуществлен поиск в базе.
* +Delete(ID:int): Bool – функция удаляет команду.
* +DeleteGame(IDTeam : int, IDGame : int) - удаление игры у команды.
* +DeleteSponsor(IDTeam : int, IDSponsor : int) - удаление спонсора у команды.
* +DeletePlayer(IDTeam : int, IDPlayer : int) - удаление игрока у команды.
* +GetPlayers(IDTeam : int, sorting : String, filtering : String, sortingA : boolean, count : int, page : int) : List<[Player](https://github.com/Tyukhaev/BTP/blob/master/docs/Player.md "объект класса Player")> - функция, возвращающая список игроков команды, удовлетворяющих заданным параметрам.
* +GetTeams(IDTeam : int, sorting : String, filtering : String, sortingA : boolean, count : int, page : int) : List<[Team](https://github.com/Tyukhaev/BTP/blob/master/docs/Team.md "объект класса Team")> - функция, возвращающая общее количество команд,удовлетворяющих заданным параметрам.
Параметры:
	* sortintg: string — отвечает, по какому полю будет сортироваться список;
  
	* sortingA: bool — отвечает, по возрастанию или убыванию будут сортироваться элементы;
  
	* filtering: string — отвечает за фильтрацию;
  
	* count: int — отвечает, сколько элементов необходимо показать;
  
	* page: int — отвечает, с какой страницы начинать поиск элементов.
	
* +GetSponsors(IDTeam : int, sorting : String, filtering : String, sortingA : boolean, count : int, page : int) : List<[Sponsor](https://github.com/Tyukhaev/BTP/blob/master/docs/Sponsor.md "объект класса Sponsor")> - функция, возвращающая список спонсоров игр с заданными параметрами.
* +GetGames(IDTeam : int, sorting : String, filtering : String, sortingA : boolean, count : int, page : int) : List<[Game](https://github.com/Tyukhaev/BTP/blob/master/docs/Game.md "объект класса Game")> - функция,возвращающая список игр команд с заданным параметрам.

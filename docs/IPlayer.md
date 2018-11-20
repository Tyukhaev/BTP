# Описание интерфейса IPlayer
Интерфейс предназначен для работы с методами класса Player

## Реализация интерфейса
* +Add (Player: [Player](https://github.com/Tyukhaev/BTP/blob/master/docs/Player.md "объект класса Player")): Int — функция, добавляющая игрока в базу данных. Параметр «[Player](https://github.com/Tyukhaev/BTP/blob/master/docs/Player.md "объект класса Player")» — игрок, 
которую необходимо добавить в БД;
* +Save (Player: [Player](https://github.com/Tyukhaev/BTP/blob/master/docs/Player.md "объект класса Player")): Bool — функция, редактирующая данные о игроке. Параметр «[Player](https://github.com/Tyukhaev/BTP/blob/master/docs/Player.md "объект класса Player")» — 
игрок, которую необходимо редактировать в БД;
* +FindByID(ID: Int): [Player](https://github.com/Tyukhaev/BTP/blob/master/docs/Player.md "объект класса Player")  — функция, осуществляющая поиск игроков в базе данных по ID и возвращающая найденный, если такой есть. 
* +Delete(ID:int): Bool – функция удаляет игрока.
* +GetPlayers(IDPlayer : int, sorting : String, filtering : String, sortingA : boolean, count : int, page : int) : List<[Player](https://github.com/Tyukhaev/BTP/blob/master/docs/Player.md "объект класса Player")> - функция, возвращающая общее количество игроков,удовлетворяющих заданным параметрам.
Параметры:
	* sortintg: string — отвечает, по какому полю будет сортироваться список;
  
	* sortingA: bool — отвечает, по возрастанию или убыванию будут сортироваться элементы;
  
	* filtering: string — отвечает за фильтрацию;
  
	* count: int — отвечает, сколько элементов необходимо показать;
  
	* page: int — отвечает, с какой страницы начинать поиск элементов.
	

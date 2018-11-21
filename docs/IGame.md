# Описание интерфейса IGame
Интерфейс предназначен для работы с методами класса Game

## Реализация интерфейса
* +Add (Game: [Game](https://github.com/Tyukhaev/BTP/blob/master/docs/Game.md "объект класса Game")): Int — функция, добавляющая работника в базу данных. Параметр «[Game](https://github.com/Tyukhaev/BTP/blob/master/docs/Game.md "объект класса Game")» — игра, 
которую необходимо добавить в БД;
* +Save (Game: [Game](https://github.com/Tyukhaev/BTP/blob/master/docs/Game.md "объект класса Game")): Bool — функция, редактирующая данные о работнике. Параметр «[Game](https://github.com/Tyukhaev/BTP/blob/master/docs/Game.md "объект класса Game")» — 
игра, которую необходимо редактировать в БД;
* +FindByID(ID: Int): [Game](https://github.com/Tyukhaev/BTP/blob/master/docs/Game.md "объект класса Game")  — функция, осуществляющая поиск игр в базе данных по ID и возвращающая найденный, если такой есть. 
* +Delete(ID:int): Bool – функция удаляет игру.
* +GetGames(IDGame : int, sorting : String, filtering : String, sortingA : boolean, count : int, page : int) : List<[Game](https://github.com/Tyukhaev/BTP/blob/master/docs/Game.md "объект класса Game")> - функция, возвращающает общее количество игр,удовлетворяющих заданным параметрам.
Параметры:
	* sortintg: string — отвечает, по какому полю будет сортироваться список;
  
	* sortingA: bool — отвечает, по возрастанию или убыванию будут сортироваться элементы;
  
	* filtering: string — отвечает за фильтрацию;
  
	* count: int — отвечает, сколько элементов необходимо показать;
  
	* page: int — отвечает, с какой страницы начинать поиск элементов.
	

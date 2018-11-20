# Описание интерфейса ISponsor
Интерфейс предназначен для работы с методами класса Sponsor

## Реализация интерфейса
* +Add (Sponsor: [Sponsor](https://github.com/Tyukhaev/BTP/blob/master/docs/Sponsor.md "объект класса Sponsor")): Int — функция, добавляющая спонсора в базу данных. Параметр «[Sponsor](https://github.com/Tyukhaev/BTP/blob/master/docs/Sponsor.md "объект класса Sponsor")» — спонсор, 
которую необходимо добавить в БД;
* +Save (Sponsor: [Sponsor](https://github.com/Tyukhaev/BTP/blob/master/docs/Sponsor.md "объект класса Sponsor")): Bool — функция, редактирующая данные о работнике. Параметр «[Sponsor](https://github.com/Tyukhaev/BTP/blob/master/docs/Sponsor.md "объект класса Sponsor")» — 
спонсор, которую необходимо редактировать в БД;
* +FindByID(ID: Int): [Sponsor](https://github.com/Tyukhaev/BTP/blob/master/docs/Sponsor.md "объект класса Sponsor")  — функция, осуществляющая поиск спонсоров в базе данных по ID и возвращающая найденный, если такой есть. 
* +Delete(ID:int): Bool – функция удаляет спонсора.
* +GetSponsors(IDSponsor : int, sorting : String, filtering : String, sortingA : boolean, count : int, page : int) : List<[Sponsor](https://github.com/Tyukhaev/BTP/blob/master/docs/Sponsor.md "объект класса Sponsor")> - функция, возвращающая общее количество спонсоров,удовлетворяющих заданным параметрам.
Параметры:
	* sortintg: string — отвечает, по какому полю будет сортироваться список;
  
	* sortingA: bool — отвечает, по возрастанию или убыванию будут сортироваться элементы;
  
	* filtering: string — отвечает за фильтрацию;
  
	* count: int — отвечает, сколько элементов необходимо показать;
  
	* page: int — отвечает, с какой страницы начинать поиск элементов.
	

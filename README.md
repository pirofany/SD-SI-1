# SD-SI-1

Необходимо сделать 4 операции: создание обьекта,изменение,удаление и кенсел/реджект/терминей(в зависимости от обьектоного типа 
и доступных значений  статуса объекта)

1 Crete object: необходимо сделать ограничение по количеству объектов (5штук) под одним биллинг аккаунтом  

2 Update : можно изменять объекто если его статус :
   *  для била (created,pending cancelletion)
   *  для аджастмента (pending ,approved)
   *   для пейментов (pending, posted)
   *   для диспутов (pending ,approved)
   *  Для ots (created,unbilled, billed)

3 delete : пока без ограничений  

4 cancel/reject/terminate: меняет статус обьекта на соответвующий  

ограничения по статусам :
  *  для била (pending cancelletion)
  *    для аджастмента (approved)
  *    для пейментов (posted)
  *    для диспутов (approved)
  *    Для ots ( billed)

05.05.2020
1 Bill Creation: Bill amount =dispute amount+ adj amount+ ots amount , ots переводиться в статус биллед,
так же нельзя создавать bill с amount = 0. 

2 Approve dispute: при апруве диспута создаётся аджастмент с таким же эмаунтов в статусе апрув и в дискрипшене adj должно быть имя
dis 

3 Delete adj : при удалениее adj удаляется так же диспут из которого он был создан 

4 Payment creation: нельзя создавать если нету била, можно создавать до тех пор пока общаю сумма пейментов <= bill amount 

5 delete ots: при удалении создаётся отрицательный пеймент на сумму как и ots




 

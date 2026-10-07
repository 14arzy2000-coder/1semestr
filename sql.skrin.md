<img width="942" height="445" alt="изображение" src="https://github.com/user-attachments/assets/34d71b25-81e2-4a3d-81fd-bf1c6915042a" />

<img width="549" height="347" alt="Снимок экрана 2026-10-07 094658" src="https://github.com/user-attachments/assets/cff48a38-f269-41b0-ac25-14ceafa3c936" />



<img width="1681" height="492" alt="изображение" src="https://github.com/user-attachments/assets/ec1a7e6f-9b35-4536-b2a8-27a9ca68fd5b" />


select s.name, sg.name, g.ocenka, sb.kurator
from students as s,
	 s_groups as sg, 
     grades as g,
     sublects as sb
where sg.name = "рпо 25/2"


use university;

insert into subjects(name, time, teacher)
value ('разработка по', HOUR('2026-10-07 13:35:00'), 'Олег Сергеевич Сабодаш'),
	  ('алгоритмизация', HOUR('2026-10-08 11:35:00'), 'Олег Сергеевич Сабодаш'),
     ('численные методы', HOUR('2026-10-07 18:35:00'), 'Алексей Дмитриевич Фурин'),
      ('вышмат', HOUR('2026-10-07 10:35:00'), 'Алексей Дмитриевич Фурин');



#select c.name, o.name
#from customers as c,
#	 orders as o
#where c.name = "ирина";

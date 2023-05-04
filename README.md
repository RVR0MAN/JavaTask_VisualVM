# Задача "Исследование JVM через VisualVM"  
### График Classes  
![image](https://user-images.githubusercontent.com/120349770/236107516-ebf24a27-338f-404e-9b0c-d49cc4119cb2.png)

Область 1:    
 - Произведена загрузка 1981 класса при выполнении  System.out.println("Please open 'ru.netology.JvmExperience' in VisualVm");   

Область 2:
- Произведена загрузка классов из пэкэджа io.vertx  

Область 3:  
- Произведена загрузка классов из пэкэджа io.netty  

Область 4:    
- Произведена загрузка классов из пэкэджа org.springframework  

### График MetaSpace  
![image](https://user-images.githubusercontent.com/120349770/236115252-616bf007-d3e3-4334-a216-26331fb6f450.png)  

Область 1:    
 - Выделена дополнительная память в MetaSpace и произведена загрузка метаданных классов пэкэджа io.vertx   

Область 2:
- Выделена дополнительная память в MetaSpace и произведена загрузка метаданных классов из пэкэджа io.netty   

Область 3:  
- Выделена дополнительная память в MetaSpace и произведена загрузка метаданных классов из пэкэджа org.springframework  

### График Heap

![image](https://user-images.githubusercontent.com/120349770/236119524-93234070-b514-40a6-bab5-e882563d5d6e.png)  

Область 1:  
- Выделена память под объекты, которые попали в кучу в результате выполнения  System.out.println("Please open 'ru.netology.JvmExperience' in VisualVm");  

Область 2, 6:  
- Отрабатывает GarbageCollector, память освобождается  

Область 3, 4, 5:  
- В кучу попадают объекты загруженные в 3 этапа, объёмом по 5 000 000 экземпляров, за одну загрузку  



 



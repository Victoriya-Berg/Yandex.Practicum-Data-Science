# Обработка фотографий покупателя 

Сетевой супермаркет внедряет систему компьютерного зрения для обработки фотографий покупателей. Фотофиксация в прикассовой зоне поможет определять возраст клиентов, чтобы анализировать покупки и предлагать товары, которые могут заинтересовать покупателей этой возрастной группы и контролировать добросовестность кассиров при продаже алкоголя. Строится модель, которая по фотографии определит приблизительный возраст человека. В вашем распоряжении набор фотографий людей с указанием возраста.

## Анализ модели

* При обучении модели использована сеть ResNet50 с урезанной верхушкой и весами с Imagenet
* Параметры обучения
    * Размер батча 32
    * Оптимизатор Adam
    * Без заморозки весов
    * Количество эпох 10
* Метрика тестовой выборки отличается от метрики тренировочной почти в 3 раза, поэтому можно сказать, что модель переобучена.

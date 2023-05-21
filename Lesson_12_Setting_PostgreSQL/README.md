# Настройка PostgreSQL
## Нагрузочное тестирование и тюнинг PostgreSQL
1. <b>Цель:</b>
    * сделать нагрузочное тестирование PostgreSQL
    * настроить параметры PostgreSQL для достижения максимальной производительности

1. <b>Описание/Пошаговая инструкция выполнения домашнего задания:</b></br>
    * развернуть виртуальную машину любым удобным способом
    * поставить на неё PostgreSQL 15 любым способом
    * настроить кластер PostgreSQL 15 на максимальную производительность не обращая внимание на возможные проблемы с надежностью в случае аварийной перезагрузки виртуальной машины
    * нагрузить кластер через утилиту через утилиту pgbench (https://postgrespro.ru/docs/postgrespro/14/pgbench)
    * написать какого значения tps удалось достичь, показать какие параметры в какие значения устанавливали и почему    
      > Воспользовался pgtune и получил 1/5 производительности в отличии от начальных параметров. Пробовал что то менять самостоятельно но более 2700 tps увеличить не удавалось. Замечательную производительность дает асинхронный комит в журнал.</br>
      > ![pgtune](https://github.com/prowokatorkraft/Otus_PostgreSQL/blob/main/Lesson_12_Setting_PostgreSQL/2023-05-21_19h19_07.png)
# Demos

1.необходимо создать 2 консольных приложения.1-е приложение:бесконечно генерирует случайные числа в диапазоне, рассылает мультикастом по udp, без задержек.Диапазон и мультикаст группа настраивается через отдельный хмл-конфиг.2-е приложение:
принимает данные по юдп, считает: среднее, стандартное отклонение, моду, медиану.
Посчитанные значения выводит по требованию (нажатие энтер)
приложение должно контролировать получение всех пакетов, количество потерянных пакетов должно выводить со статистикой
(для форсирования потери пакетов нужно добавить задержку в прием сообщений)
прием пакетов и счет реализовать в разных потоках с минимальными задержками
мультикаст группа и задержка приема должна настраиваться через отдельный хмл-конфиг.
приложение должно быть максимально оптимизировано по скорости работы
приложение должно мочь работать продолжительное время (неделя-месяц) без падений/ошибок

2.дано 2 таблицы
работники (id, name) - содержит список работников
зарплаты (worker_id, date, value) - содержит список дат и суммы когда работники получали зарплаты
необходимо написать запрос, который вернет список работников которые не получили з.п. за указанный месяц
таблицы могут быть размером более миллиона записей

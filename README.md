Заглушка принимает POST-запрос, содержащий два поля с целочисленными значениями: "firstNumber" и "secondNumber". 
В ответе возвращаются оба переданных поля, а также поле "result", хранящее строку.
Возвращаемая строка является результатом проверки разности двух переданных чисел на простоту. 
Если разность "firstNumber" и "secondNumber" (по модулю) является простым числом, возвращается строка "SIMPLE", если составным - "COMPOSITE". В случае, если получившаяся разность получилась равной 0 или 1, возвращается "0" или "1" соответственно.

Пример тела запроса:
{
    "firstNumber": 0,
    "secondNumber": 11
}

Пример тела ответа:
{
    "firstNumber": 0,
    "secondNumber": 11,
    "result": "SIMPLE"
}

Для запуска программы необходимо распаковать архив и, перейдя в командной строке в папку "demo" запустить следующую команду:
java -jar target\demo-0.0.1-SNAPSHOT.jar

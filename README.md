# Python PARSEC

Библиотека Python PARSEC предоставляет питоновские биндинги библиотеки PARSEC.

Авторы: [Лаборатория 50](http://лаборатория50.рф) team@lab50.net.

## Лицензия

Все материалы распространяются на условиях
стандартной общественной лицензии [GNU (GPL)](http://www.gnu.org/copyleft/gpl.html) версии 3.

Полный текст лицензии находится в файле COPYING.

## PARSEC

Библиотека  PARSEC  содержит  средства  для работы с системой безопасности
PARSEC ОС СН Astra Linux Special Edition, а также с базами данных (БД) системы безопасности
PARSEC. Ниже перечислены функции библиотеки PARSEC, разделенные на группы в соответствии с компонентам
безопасности PARSEC, к которым они относятся:

 *  мандатный механизм разграничения доступа;
 *  расширенный механизм привилегий;
 *  поддержка протоколирования;
 *  работа с журналом аудита и отправка сообщений.

## Пример использования

    import parsec

    if __name__ == "__main__":

        mac = parsec.mac_get_pid(0)

        print "Мандатная метка данного процесса '{}'.".format(
            parsec.mac_to_text(mac))


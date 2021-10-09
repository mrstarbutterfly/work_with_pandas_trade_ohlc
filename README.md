#На вход программе подается файл, содержащий биржевые сделки в формате .csv (тикер, цена акции, количество купленных акций,
# время валидации сделки). (файл - trades.csv)


# На выходе ваша программа предоставляет обработанные данные для построения свечных графиков с масштабами 5 минут , 30 минут и 240 минут(
# ohlc_5min.csv, ohlc_30min.csv, ohlc_240min.csv)



#Детали ТЗ:
#1)Cделки в csv, поданные на вход, отсортированы по времени по возрастанию
#2)Cделки в csv представлены по нескольким акциям, то есть могут встречаться несколько разных тикеров акций
#3)На выходе требуется получить данные, сгруппированные по масштабам, отсортированные по времени по возрастанию
#4)Время проведения торгов: начало в 7 утра каждого дня, торги завершаются в 3 часа ночи следующего дня (по факту, это не так,
# но мы будем ориентироваться на эти цифры)
# Cделки, осуществленные вне времени проведения торгов считаются недействительными, то есть их не учитываем при построении свечных
# аггрегатов

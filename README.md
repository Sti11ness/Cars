# Определение стоимости автомобилей

## Описание проекта
Сервис по продаже автомобилей с пробегом «Не бит, не крашен» разрабатывает приложение, которое позволит пользователям узнать рыночную стоимость их автомобиля. Для этого требуется построить модель машинного обучения, которая будет предсказывать цену автомобиля на основе его технических характеристик и других параметров.

## Цель проекта
Разработать и обучить модель, которая сможет точно предсказывать рыночную стоимость автомобилей. Модель должна обладать высокой точностью, а также быть эффективной по времени обучения и предсказания.

## Задача
- Исследовать и подготовить данные для моделирования.
- Обучить несколько моделей, включая модель градиентного бустинга LightGBM и хотя бы одну простую модель, для сравнения.
- Провести анализ моделей на основе их качества (по метрике RMSE), времени обучения и времени предсказания.
- Выбрать лучшую модель по критериям заказчика.

## Описание данных
Данные находятся в файле `/datasets/autos.csv` и содержат следующие признаки:

- **DateCrawled** — дата скачивания анкеты из базы.
- **VehicleType** — тип автомобильного кузова.
- **RegistrationYear** — год регистрации автомобиля.
- **Gearbox** — тип коробки передач.
- **Power** — мощность (л.с.).
- **Model** — модель автомобиля.
- **Kilometer** — пробег (км).
- **RegistrationMonth** — месяц регистрации автомобиля.
- **FuelType** — тип топлива.
- **Brand** — марка автомобиля.
- **Repaired** — была ли машина в ремонте.
- **DateCreated** — дата создания анкеты.
- **NumberOfPictures** — количество фотографий автомобиля.
- **PostalCode** — почтовый индекс владельца анкеты.
- **LastSeen** — дата последней активности пользователя.
- **Price** — цена автомобиля (целевая переменная, в евро).

## Требования заказчика
- Метрика качества: **RMSE** (Root Mean Squared Error) должна быть **меньше 2500**.
- Время обучения модели и время предсказания должны быть оптимальными для потенциальной интеграции в приложение.
- Рекомендуется исследовать разные модели, включая как бустинг, так и более простые подходы.
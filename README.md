## Сущность модели:
Это демонстрационная модель для системы JointML, которая решает задачу выявления мошеннических банковских транзакций.

Для классификации применяется нейронная сеть, построенная с использованием PyTorch. Эта сеть включает сверточные слои, пакетную нормализацию, слои отключения (dropout) и линейные слои.

Демонстрационные тренировочные данные содержат 30 фичей, 28 из которых -- анонимизированные параметры.


## Принимаемые параметры:
* Параметры модели:
```
model_parameters = {
    'n_features': 30,
    'hidden_dim': 16
}
```
* Параметры для датасета:
```
dataset_parameters = {
    'test_size': 0.1,
    'shuffle': true
}
```
* Параметры для тестирования:
```
отсутствуют
```
* Параметры для тренировки:
```
train_parameters = {
    'epochs': 40,
    'batch_size': 16,
    'lr': 0.0001
}
```

### Тестовые файлы для обучения модели хранятся в папке dataset_examples

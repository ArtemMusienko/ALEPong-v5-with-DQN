![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white)![Google Colab](https://img.shields.io/badge/Google%20Colab-%23F9A825.svg?style=for-the-badge&logo=googlecolab&logoColor=white)![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)	![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)

## ALE/Pong-v5 with DQN

В данном коде используется такая среда обучения, как **ALE/Pong-v5**. 1.  Реализована нейросетевая архитектура на полносвязных слоях, определены классы  `NNModel`  и  `DQN`, реализующие предсказательную и целевую сети, буфер воспроизведения, ε-жадную стратегию, синхронизацию весов и шаг обучения, реализован цикл обучения агента с ε-жадной стратегией и постепенным уменьшением ε, а также график динамики награды по эпизодам.

В финальной части notebook приведён анализ поведения агента и вывод.

> Настоятельно рекомендую код запускать в **Google Colab** с
> использованием **графического ускорителя T4**!

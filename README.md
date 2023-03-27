## HomeWork ([Colab.google.com](https://colab.research.google.com/drive/1hE282AMVT3IRkhcEwEk1KC247hxf2XuI#scrollTo=cGUv-Qif9QPj))
# Домашняя работа по регуляризации и оптимизации

Подобрать методом GD параметры функции:

$f(x, \theta) = x_1 \theta_1 + x_2 \theta_2 + \theta_3.$

Предлагается подобрать параметры $\theta$ минимизируя следующую функцию ошибки:

$\mathcal{L}(\theta) = 0.1 \|\theta\|^2 + \frac{1}{N}\sum\limits_{i=1}^N \max(0, 1 - y_i f(x_i, \theta)).$

Для оптимизации предлагается использовать метод градиентного спуска с 1000 шагами размера $0.1$ из начальной точки $(1, 1, 0)$.

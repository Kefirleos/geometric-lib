# Документация Geometric Lib

Библиотека `geometric_lib` предоставляет набор функций для вычисления геометрических параметров базовых двумерных фигур (планиметрия) и трёхмерных тел (стереометрия).

---

## Описание функций и модулей

### 1. Окружность и круг (`circle.py`)
- `area(r)`: Вычисляет площадь круга по формуле $S = \pi r^2$.
  - Параметры: `r (int/float)` - радиус круга.
  - Возвращает: `float` - площадь круга.
  - Пример: `area(5)` $\to$ `78.53981633974483`
- `perimeter(r)`: Вычисляет длину окружности по формуле $P = 2\pi r$.
  - Параметры: `r (int/float)` - радиус круга.
  - Возвращает: `float` - длина окружности.
  - Пример: `perimeter(5)` $\to$ `31.41592653589793`

### 2. Квадрат (`square.py`)
- `area(a)`: Вычисляет площадь квадрата по формуле $S = a^2$.
  - Параметры: `a (int/float)` - длина стороны квадрата.
  - Возвращает: `int/float` - площадь квадрата.
  - Пример: `area(3)` $\to$ `9`
- `perimeter(a)`: Вычисляет периметр квадрата по формуле $P = 4a$.
  - Параметры: `a (int/float)` - длина стороны квадрата.
  - Возвращает: `int/float` - периметр квадрата.
  - Пример: `perimeter(3)` $\to$ `12`

### 3. Прямоугольник (`rectangle.py`)
- `area(a, b)`: Вычисляет площадь прямоугольника по формуле $S = a \cdot b$.
  - Параметры: `a (int/float)`, `b (int/float)` - стороны прямоугольника.
  - Возвращает: `int/float` - площадь прямоугольника.
  - Пример: `area(3, 5)` $\to$ `15`
- `perimeter(a, b)`: Вычисляет периметр прямоугольника по формуле $P = 2(a + b)$.
  - Параметры: `a (int/float)`, `b (int/float)` - стороны прямоугольника.
  - Возвращает: `int/float` - периметр прямоугольника.
  - Пример: `perimeter(3, 5)` $\to$ `16`

### 4. Треугольник (`triangle.py`)
- `area(a, h)`: Вычисляет площадь треугольника по формуле $S = \frac{a \cdot h}{2}$. Если результат целый, возвращает `int`, иначе `float`.
  - Параметры: `a (int/float)` - основание, `h (int/float)` - высота.
  - Возвращает: `int/float` - площадь треугольника.
  - Пример: `area(4, 5)` $\to$ `10`
  - Пример: `area(3, 3)` $\to$ `4.5`
- `perimeter(a, b, c)`: Вычисляет периметр треугольника по формуле $P = a + b + c$.
  - Параметры: `a, b, c (int/float)` - стороны треугольника.
  - Возвращает: `int/float` - периметр треугольника.
  - Пример: `perimeter(3, 4, 5)` $\to$ `12`

### 5. Сфера (`sphere.py`) - 3D Стереометрия
- `area(r)`: Вычисляет площадь поверхности сферы по формуле $S = 4\pi r^2$.
  - Параметры: `r (int/float)` - радиус сферы.
  - Возвращает: `float` - площадь поверхности.
  - Пример: `area(4)` $\to$ `201.06192982974676`
- `volume(r)`: Вычисляет объём сферы по формуле $V = \frac{4}{3}\pi r^3$.
  - Параметры: `r (int/float)` - радиус сферы.
  - Возвращает: `float` - объём сферы.
  - Пример: `volume(4)` $\to$ `268.082573106329`

---

## История изменений проекта (Commit History)

| Хеш коммита | Сообщение коммита                                                  |
| :---------- | :----------------------------------------------------------------- |
| `8ba9aeb`   | L-03: Circle and square added                                      |
| `d078c8d`   | L-03: Docs added                                                   |
| `c7d1c57`   | feat(rectangle): add area and perimeter calculations               |
| `3fc94a4`   | feat(triangle): add area and perimeter calculations                |
| `1956a14`   | feat(sphere): add 3d sphere surface area and volume calculations   |
| `41b2743`   | docs(circle): add docstrings with parameters and usage examples    |
| `c8ddeab`   | fix(circle): remove debug print call                               |
| `0e06a71`   | docs(square): add docstrings with parameters and usage examples    |
| `92480e2`   | docs(rectangle): add docstrings with parameters and usage examples |
| `96a08de`   | docs(triangle): add docstrings with parameters and using examples  |
| `943c11c`   | docs(sphere): add docstrings with parameters and usage examples    |
| `1d15e3c`   | refactor(triangle): return int if area is whole number             |

*(Примечание: коммит добавления текущей документации является последней записью в репозитории и не включён в таблицу ввиду невозможности рекурсивной фиксации собственного хэша).*
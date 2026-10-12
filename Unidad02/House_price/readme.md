```python
import pandas as pd

df = pd.read_csv("Casa_toluca_2.csv")
print("Columns:", df.columns.tolist())
print("\nShape:", df.shape)
print("\nHead:\n", df.head(3))
print("\nInfo/Data Types:\n")
print(df.info())
print("\nSummary Statistics:\n", df.describe(include='all'))
print("\nMissing values:\n", df.isnull().sum())


```

```text
Traceback (most recent call last):
  File "<xbox-string>", line 3, in <module>
    df = pd.read_csv("Casa_toluca_2.csv")
  File "readers.py", line 912, in read_csv
    return _read(filepath_or_buffer, kwds)
  File "readers.py", line 577, in _read
    parser = TextFileReader(filepath_or_buffer, **kwds)
  File "readers.py", line 1407, in __init__
    self._engine = self._make_engine(f, self.engine)
  File "readers.py", line 1661, in _make_engine
    self.handles = get_handle(
  File "common.py", line 859, in get_handle
    handle = open(
FileNotFoundError: [Errno 2] No such file or directory: 'Casa_toluca_2.csv'


```

```python
import os
print(os.listdir('.'))


```

```text
['Casa_toluca.csv']


```

```python
import pandas as pd

df = pd.read_csv("Casa_toluca.csv")

# Clean unnamed columns
cols_to_drop = [c for c in df.columns if 'Unnamed' in c]
df_clean = df.drop(columns=cols_to_drop)

print("Columns:", df_clean.columns.tolist())
print("Shape:", df_clean.shape)
print("\nMissing values:\n", df_clean.isnull().sum())
print("\nDescriptive Stats:\n", df_clean.describe())
print("\nSample Data:\n", df_clean.head(5))


```

```text
Columns: ['Ubicación', 'Area', 'Baños', 'Habitaciones', 'Precio']
Shape: (2004, 5)

Missing values:
 Ubicación         0
Area            283
Baños            54
Habitaciones     73
Precio            5
dtype: int64

Descriptive Stats:
                Area        Baños  Habitaciones        Precio
count   1721.000000  1950.000000   1931.000000  1.999000e+03
mean     229.525857     2.496923      3.306059  1.690472e+05
std      337.245195     3.093504      1.512319  4.067087e+05
min       10.000000     1.000000      1.000000  1.065305e+04
25%      113.000000     2.000000      3.000000  5.162500e+04
50%      165.000000     2.000000      3.000000  9.075000e+04
75%      250.000000     3.000000      4.000000  1.600000e+05
max    11111.000000   124.000000     40.000000  1.000000e+07

Sample Data:
                                                          Ubicación   Area  Baños  Habitaciones    Precio
0            Casa en Venta Los Serrados\n, Toluca De Lerdo, México  105.0    2.0           3.0  130000.0
1  Casa en Venta Tierra Y Libertad #114\n, Toluca De Lerdo, México  115.0    2.0           3.0   50800.0
2                            Casa en Venta Toluca De Lerdo, México  700.0    3.0           3.0  325000.0
3                           Casa en Venta Granjas, Toluca De Lerdo  390.0    3.0           4.0  275000.0
4                            Casa en Venta Toluca De Lerdo, México  300.0    4.0           3.0  215000.0


```

I voy a generar la documentación completa y descripción de la base de datos en formato Markdown.

He generado la descripción en formato Markdown para que puedas copiarla e incluirla en el archivo `README.md` de tu repositorio de GitHub.

¿Quieres que agregue secciones adicionales, como estadísticas descriptivas o instrucciones de instalación/uso en Python o R?

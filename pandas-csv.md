---
layout: default
---

# Jugando con Pandas y ficheros JSON y .CSV

## El fichero CSV
csv: 
atributo > valor
1 atributo por columna


## El fichero JSON


## Introducción a Pandas
Como en cualquier código Python, el primer paso es importar la librería que queremos utilizar
```python
import pandas as pd
```

En Python, las estructuras llamadas diccionarios nos ayudan a estructurar información que esté compuesta por columnas y filas de información. En Pandas, la estructura que se acopla perfectamente a la de diccionario se llama DataFrame. 

```python
dict_ = {'user': [], 'user_location': [], 'date_created': [], 'text': [], 'retweet_count': [], 'favorite_count': [], 'hashtags': [], 'user_mentions': [], 'urls': []}        

df = pd.DataFrame(dict_)  

```

### Checklist para una correcta extracción de información

* Keywords, dominio, problema
* Número de datos (instancias)
* Atributos
* Tipo de datos
* Salida (si/no)
* Idioma
* Localización
* Rango de fechas
* Encoding: utf-8 (emojis)


### Volcar la información a un fichero .CSV


```python
df.to_csv(path_or_buf = "twitter_stream.csv", mode="a", header=False, encoding="utf-8")
```



<div class="center">

<blockquote class="twitter-tweet"><p lang="en" dir="ltr">PROTIP: wanna get data from your Google Sheet into Python/R/etc? Don&#39;t mind if the data has a public link? It&#39;s as easy as this: <a href="https://t.co/DBlewp8XVF">pic.twitter.com/DBlewp8XVF</a></p>&mdash; Chris Holdgraf (@choldgraf) <a href="https://twitter.com/choldgraf/status/1141436794359046144?ref_src=twsrc%5Etfw">June 19, 2019</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

</div>


[Volver a inicio](./)

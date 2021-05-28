# POC Mis Datos en Spotify

Visualización de Un Dataset generado a partir de los datos que se pueden obtener en Spotify

## Requisitos 📋
Tener una cuenta Premiun (con abono pago) en Spotify
Obtener los datos a visualizar desde https://www.spotify.com/ar/account/privacy/ (sitio para Argentina)
En su defecto entrar a la página de Spotify Developers, iniciar sesión y crear una aplicación. De esta manera se genera automáticamente el Client ID y el Client Secret.
https://developer.spotify.com/ (este fue mi caso)

### Herramientas 🔧

Google Colab - Python
Se deben instalar en el colab :
  spotipy https://spotipy.readthedocs.io/en/2.18.0/
  ijson para parsear el archivo json

Flourish para Visualizaciones (algo de Vega Lite https://vega.github.io/vega-lite/) 

https://public.flourish.studio/visualisation/6236780/
https://public.flourish.studio/visualisation/6269068/
https://public.flourish.studio/visualisation/6266292/

https://app.flourish.studio/@flourish/vega-lite/3 (template con Vega Lite)

## Archivos ⚙️
*spot1.json* generado en la consola web de spotify "Get User's Top Artists and Tracks" https://developer.spotify.com/console/get-current-user-top-artists-and-tracks/?type=tracks&time_range=medium_term&limit=10&offset=5 

*spotify2020b.csv* Este lo genere en pandas y fue el que genere en el colab en pandas.
Corresponde a la playlist generada automaticamente por Spotify "100 canciones favoritas del 2020"
https://open.spotify.com/playlist/37i9dQZF1EM0WTjT3czb99


### pruebas  🔩
El archivo JSON si se lo carga directamente en PANDAS no muestra bien los datos hay que parsearlo y procesarlo opte por realizar
la consulta de la playlist con mis 100 tracks favoritos en 2020. Haciendo la consulta con la libreria spotity 
primero visualice los campos, columnas, listas que me devolvia luego las recupere usando listas [] de python y eso lo volque en un dataframe
de pandas 
_Explica que verifican estas pruebas y por qué_

```
Da un ejemplo
```

### Y las pruebas de estilo de codificación ⌨️

_Explica que verifican estas pruebas y por qué_

```
Da un ejemplo
```

## Despliegue 📦




## Expresiones de Gratitud 🎁

* Comenta a otros sobre este proyecto 📢
* Invita una cerveza 🍺 o un café ☕ a alguien del equipo. 
* Da las gracias públicamente 🤓.
* etc. 



---
(https://github.com/gusper01) 😊

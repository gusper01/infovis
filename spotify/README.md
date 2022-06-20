# POC Mis Datos en Spotify

Visualización de Datos Personales. generado a partir de los datos que se pueden obtener en Spotify

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

*spot1.json* generado en la consola web de spotify "Get User's Top Artists and Tracks" 
https://developer.spotify.com/console/get-current-user-top-artists-and-tracks/?type=tracks&time_range=medium_term&limit=10&offset=5 

*spotify2020b.csv* Este lo genere en pandas y fue el que genere en el colab en pandas.
Corresponde a la playlist generada automaticamente por Spotify "100 canciones favoritas del 2020"
https://open.spotify.com/playlist/37i9dQZF1EM0WTjT3czb99

*POC_Spotify.ipynb* notebook Colab


### pruebas  🔩

El archivo JSON si se lo carga directamente en PANDAS no muestra bien los datos hay que parsearlo y procesarlo opte por realizar
la consulta de la playlist con mis 100 tracks favoritos en 2020. Usando la libreria spotity 
la respuesta a la consulta de la playlist es un diccionario de python donde primero visualice los campos, columnas luego eso lo volque en dataframes 
de pandas y finalmente genera un nuevo dataframe con los datos que me intersaban desde el colab baje el archivo *spotify2020b.csv*.  
Este archivo csv lo abri con Excel lo copie y lo pegue en flourish. 


## Despliegue 📦

finalmente publique https://gusper01.github.io/infovis/spotify/misdatos2.html


## Referencias e inspiraciones  📢

En esas páginas encontre muchas cosas y todavia me queda probar el JSON 
https://stmorse.github.io/journal/spotify-api.html
https://ichi.pro/es/un-analisis-del-gusto-musical-utilizando-spotify-api-y-python-251981846132220
https://github.com/plamere/spotipy/commit/63eebfa9300203e9a50d1ecd2ab3e4502639c21f
http://harpolea.github.io/2018-05-09-spotipy
https://developer.spotify.com/documentation/web-api/reference/#endpoint-get-users-top-artists-and-tracks
https://tomasezequielrau.medium.com/clustering-forecasting-spotify-songs-audio-features-5b2c21f0a6b9
https://web.stanford.edu/~kjytay/courses/stats32-aut2018/Session%208/Spotify_final.html
y muuuuchosss mas !

(https://github.com/gusper01) 😊

# EventsHome

Página de visualización de eventos de intercambio de idiomas en formato de lista y de mapa

## Methods

<!-- @vuese:EventsHome:methods:start -->
|Method|Description|Parameters|
|---|---|---|
|createEvent|Redirige a la página de creación de un evento|-|
|onScroll|Detecta cuando se ha realizado scroll en la página|-|
|toTop|Realiza un scroll automático al inicio de la página|-|
|getMonth|Devuelve el mes en formato i18n de texto abreviado de la fecha pasada como parámetro|El parámetro es un Date que representa la fecha del evento|
|getDay|Devuelve el día del mes de la fecha pasada como parámetro|El parámetro es un Date que representa la fecha del evento|
|getYear|Devuelve el año de la fecha pasada como parámetro|El parámetro es un Date que representa la fecha del evento|
|listEvents|Obtiene los eventos a presentar en la vista de lista de eventos que cumplen con lo requerido por el usuario autenticado de forma paginada|-|
|openEventDescription|Redirige a la página de visualización del evento con el ID pasado como parámetro|El parámetro es un String que representa el ID del evento seleccionado por el usuario|

<!-- @vuese:EventsHome:methods:end -->


## Computed

<!-- @vuese:EventsHome:computed:start -->
|Computed|Type|Description|From Store|
|---|---|---|---|
|userRole|-|Devuelve el rol del usuario (admin o user)|No|
|userPinIcon|-|Devuelve el pin a situar en el mapa del usuario autenticado|No|
|eventPinIcon|-|Devuelve el pin del evento a situar en el mapa|No|
|userLocation|-|Devuelve la geolocalización del usuario autenticado|No|

<!-- @vuese:EventsHome:computed:end -->


## Watch

<!-- @vuese:EventsHome:watch:start -->
|Name|Description|Parameters|
|---|---|---|
|mapEvents|Observa los eventos a presentar en el mapa para controlar si ya se han cargado|-|
|eventsTabs|Devuelve la tab seleccionada de entre las dos disponibles y que se corresponden con la vista de mapa y la vista de lista de los eventos|-|
|languageInvolvedFilter|Controla la coherencia en el filtrado de los idiomas del evento|-|

<!-- @vuese:EventsHome:watch:end -->



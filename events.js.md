# events.js

## Getters

<!-- @vuese:events.js:getters:start -->
|Getter|Description|
|---|---|
|getLanguageInvolvedFilter|Devuelve el filtro de idioma implicado en los eventos a mostrar en la vista de lista de eventos|
|getFilters|Devuelve los filtros aplicados sobre los eventos a mostrar en la vista de lista de eventos|
|getEvents|Devuelve los eventos obtenidos de la base de datos|
|getEventsTab|Devuelve el modo de vista de eventos seleccionado|
|getEventByID|Utilizado para obtener los datos de un evento por su identificador|
|getEventsToShow|Utilizado para obtener los datos de los eventos a mostrar en la vista de lista|
|getMapEventsToShow|Utilizado para obtener los datos de los eventos a mostrar en la vista de mapa|
|getLastEventShowed|Utilizado para obtener la referencia al último evento mostrado en la lista de vista|
|amIParticipating|Devuelve si el usuario autenticado está apuntado o no a un evento|

<!-- @vuese:events.js:getters:end -->


## Actions

<!-- @vuese:events.js:actions:start -->
|Action|Description|Parameters|
|---|---|---|
|initState|Inicia el state con los datos apropiados|El context del events store|
|resetEventsToShowIDs|Resetea la lista de los identificadores de los eventos a mostrar en la vista de lista|El context del events store|
|createEvent|Crea y almacena un nuevo evento pasado como parámetro|El context del events store data {date, description, headerImg, location, involvedLanguages, name}|
|removeEvent|Borra y elimina un evento|El context del events store ID del evento a borrar|
|updateEvent|Actualiza un evento evento existente con los datos pasados como parámetro|El context del events store data {date, description, headerImg, location, involvedLanguages, name}|
|getEvents|Obtiene los eventos de base de datos  con fecha mayor a la actual de forma paginada|El context del events store|
|getAllEvents|Obtiene todos los eventos de base de datos con fecha mayor a la actual|El context del events store|
|getEventParticipants|Obtiene de la base de datos los datos de los usuarios implicados en un evento y los almacena|El context del events store El ID del evento|
|resetState|Resetea el estado del events store|El context del events store|
|addParticipantToEvent|Añade al usuario autenticado como participante en un evento|El ID del evento|
|removeParticipantFromEvent|Elimina al usuario autenticado como participante en un evento|El ID del evento|
|getEventByID|Obtiene un evento de la base de datos por su ID|ID del evento|

<!-- @vuese:events.js:actions:end -->


## Mutations

<!-- @vuese:events.js:mutations:start -->
|Mutation|Description|Parameters|
|---|---|---|
|setLanguageInvolvedFilter|Actualiza el valor del filtro de idiomas implicados en los eventos de la vista de lista|El state del events store El identificador del idioma por el que filtrar los eventos|
|setEventsTab|Actualiza el modo de vista de los eventos seleccionado|El state del events store Modo de vista de los eventos seleccionado: 0 o 1|
|removeEventByID|Elimina un evento de la lista de eventos obtenidos por su ID|El state del events store ID del evento a eliminar|
|resetState|Restablece todas las variables del state a sus valores por defecto|El state del events store|
|resetEventsToShowIDs|Restablece la lista de identificadores de eventos a mostrar a su valor por defecto|El state del events store|
|addEvent|Añade un evento a la lista de eventos obtenidos|El evento a añadir|
|addParticipantToEvent|Añade al usuario autenticado como participante en un evento almacenado|data{eventID, userID}|
|removeParticipantFromEvent|Elimina al usuario autenticado como participante en un evento almacenado|El state del events store data{eventID, userID}|
|addEventToShow|Añade un evento de la lista de eventos obtenidos a la lista de eventos a mostrar en la vista de lista|El state del events store ID del evento a mostrar|
|addMapEventToShow|Añade un evento de la lista de eventos obtenidos a la lista de eventos a mostrar en la vista de mapa|El state del events store ID del evento a mostrar|
|setLastEventShowed|Actualiza la referencia al último evento mostrado en la vista de lista|El state del events store Referencia al último evento mostrado en la vista de lista|

<!-- @vuese:events.js:mutations:end -->


## State

<!-- @vuese:events.js:state:start -->
|Name|Description|
|---|---|
|events|Almacena todos los eventos obtenidos de la base de datos|
|eventsToShowIDs|Almacena los identificadores de los eventos a mostrar en la vista de lista de eventos|
|mapEventsToShowIDs|Almacena los identificadores de los eventos a mostrar en la vista de lista de mapa|
|lastEventShowed|Almacena una referencia al último evento mostrado en la vista de lista de eventos|
|languageInvolvedFilter|Almacena el filtro de idioma implicado en los eventos a mostrar en la vista de lista de eventos|
|eventsTab|Almacena el modo de vista de eventos seleccionado: 0 o 1|

<!-- @vuese:events.js:state:end -->



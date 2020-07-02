# EventDescription

Página de visualización de un evento de intercambio de idiomas

## Methods

<!-- @vuese:EventDescription:methods:start -->
|Method|Description|Parameters|
|---|---|---|
|wantToRemoveEvent|Abre un diálogo pidiendo confirmación para borrar el evento|-|
|deleteEvent|Borra el evento|-|
|editEvent|Redirige a la página de edición del evento|-|
|setEventInfo|Inicializa la información del evento|-|
|openUserProfile|Redirige a la página de visualización del perfil del usuario con el ID pasado como parámetro|Este parámetro es un String que representa el ID del usuario seleccionado por el usuario autenticado|
|getParticipants|Obtiene la información de perfil de los participantes en el evento|-|
|addParticipant|Apunta al usuario autenticado al evento|-|
|removeParticipant|Desapunta al usuario autenticado del evento|-|

<!-- @vuese:EventDescription:methods:end -->


## Computed

<!-- @vuese:EventDescription:computed:start -->
|Computed|Type|Description|From Store|
|---|---|---|---|
|eventPinIcon|-|Devuelve el pin del evento a situar en el mapa|No|
|youSureYouWantToRemoveEventText|-|Devuelve el texto de preguntar si quiere borrar el evento en formato i18n|No|
|aboutToRemoveEventText|-|Devuelve el texto de proceder a borrar el evento en formato i18n|No|
|userRole|-|Devuelve el rol del usuario (admin o user)|No|
|editText|-|Devuelve el texto de editar en formato i18n|No|
|cancelText|-|Devuelve el texto de cancelar en formato i18n|No|
|confirmText|-|Devuelve el texto de confirmar en formato i18n|No|

<!-- @vuese:EventDescription:computed:end -->



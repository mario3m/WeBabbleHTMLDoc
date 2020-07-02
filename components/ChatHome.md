# ChatHome

Página de visualicación de los chats del usuario autenticado

## Methods

<!-- @vuese:ChatHome:methods:start -->
|Method|Description|Parameters|
|---|---|---|
|openChatWithUser|Redirige al usuario al chat seleccionado|El parámetro es un String que representa el ID del chat seleccionado|
|listChatsByUsername|Obtiene los chats que cumplen con las características requeridas por el usuario|-|

<!-- @vuese:ChatHome:methods:end -->


## Computed

<!-- @vuese:ChatHome:computed:start -->
|Computed|Type|Description|From Store|
|---|---|---|---|
|items|-|Devuelve los chats que cumplen con las características requeridas por el usuario ordenados descendentemente por la fecha de su último mensaje|No|
|numberOfChats|-|Devuelve el número de chats que cumplen con las características requeridas por el usuario|No|

<!-- @vuese:ChatHome:computed:end -->



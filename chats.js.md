# chats.js

## Getters

<!-- @vuese:chats.js:getters:start -->
|Getter|Description|
|---|---|
|getChatByID|Utilizado para obtener el chat con el ID pasado como parámetro con todos sus datos|
|getChatsToShowIDs|Utilizado para obtener los identificadores de los chats a mostrar|
|getChatMessagesByChatID|Utilizado para obtener los mensajes del chat con el ID pasado como parámetro|
|getUnreadMessagesByChatID|Utilizado para obtener los mensajes no leídos del chat con el ID pasado como parámetro|
|getUnreadMessages|Utilizado para obtener el número de mensajes no leídos por el usuario autenticado|
|getChatsToShow|Utilizado para obtener los chats a mostrar|
|getUserByChatID|Getter utilizado para obtener el otro usuario involucrado en el chat con el ID pasado como parámetro|
|getNotReadMessagesCountByChatID|Getter utilizado para obtener el número de mensajes no leídos del chat con el ID pasado como parámetro|

<!-- @vuese:chats.js:getters:end -->


## Actions

<!-- @vuese:chats.js:actions:start -->
|Action|Description|Parameters|
|---|---|---|
|resetState|Resetea el estado del chats store|El context del chats store|
|initState|Inicia el state con los datos apropiados|El context del chats store|
|manageChatListChange|Obtiene y gestiona los cambios en la lista de chats del usuario|El context del chats store Usuario cuya lista de chats se gestiona: user{chats[], ...}|
|manageChatMessagesChange|Obtiene y gestiona los cambios en los mensajes de un chat|El context del chats store Información del chat cuyos mensajes se gestionan: chatMessages{id, listener, messages[], ...}|
|setChatMessagesToReadByChatID|Actualiza los mensajes no leidos de un chat a estado leido|El context del chats store El ID del chat cuyos mensajes se van a poner a estado leido|
|sendNewChatMessage|Envía un mensaje en un chat, creando este último si todavía no existe|El context del chats store data{chatID, users, messageText}|
|createChatListeners|Crea los listeners para los chats del usuario|El context del chats store|

<!-- @vuese:chats.js:actions:end -->


## Mutations

<!-- @vuese:chats.js:mutations:start -->
|Mutation|Description|Parameters|
|---|---|---|
|resetState|Restablece todas las variables del state a sus valores por defecto|El state del chats store|
|addChatMessagesListener|Añade un listener pasado como parámetro a la lista de listeners de mensajes de chats del usuario|El state del chats store El listener a añadir|
|addChat|Añade un chat pasado como parámetro a la lista de chats obtenidos|El state del chats store El chat a añadir|
|updateChatMessages|Actualiza los mensajes pasados como parámetro de un chat con el identificador pasado como parámetro|El state del chats store data{chatID, messages}|
|addChatToShow|Añade el identificador pasado como parámetro a la lista de identificadores de chats a mostrar|El state del chats store El ID del chat a añadir|
|sortChatsToShowByLastMessage|Ordena la lista de identificadores de chats a mostrar por la fecha de su último mensaje en orden descendente|El state del chats store|
|setUsernameFilter|Actualiza el valor del filtro de nombre de usuario con el valor pasado como parámetro|El state del chats store El nombre de usuario por el que filtrar|
|setChatListListener|Actualiza el valor del listener de chats del usuario con el valor pasado como parámetro|El state del chats store El listener de chats del usuario|
|pushChatMessages|Añade los mensajes pasados como parámetros al chat con el ID pasado como parámetro|El state del chats store data{chatID, messages}|

<!-- @vuese:chats.js:mutations:end -->


## State

<!-- @vuese:chats.js:state:start -->
|Name|Description|
|---|---|
|chats|Almacena todos los chats del usuario obtenidos de la base de datos|
|chatsToShowIDs|Almacena los identificadores de los chats del usuario a mostrar|
|chatListListener|Almacena el listener de la lista de chats del usuario|
|chatMessagesListeners|Almacena los listeners de los mensajes de cada chat del usuario|
|usernameFilter|Controla el filtro por nombre de usuarios sobre la lista de chats|

<!-- @vuese:chats.js:state:end -->



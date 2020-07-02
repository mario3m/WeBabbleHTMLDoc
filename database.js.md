# database.js

## Actions

<!-- @vuese:database.js:actions:start -->
|Action|Description|Parameters|
|---|---|---|
|isUserAuth|Comprueba si el usuario está autenticado|-|
|setAccount|Establece en base de datos la información de cuenta del usuario autenticado|El context del database store data {email, password, name, lastName, role}|
|setAccountLanguage|Establece en base de datos el idioma de aplicación seleccionado por el usuario autenticado|El context del database store Identificador del idioma|
|askForMessagingPermission|Pide permiso para mostrar notificaciones de la aplicación en el navegador|-|
|generatePushNotificationToken|Genera y guarda en base de datos un token de notificación|-|
|getAccount|Obtiene de base de datos la información de cuenta del usuario autenticado|-|
|createAccountListener|Crea el listener de los datos de cuenta de un usuario en la base de datos|El context del database store ID del usuario|
|createAccount|Crea una cuenta de Firebase con los datos pasados como parámetro|El context del database store data {email, password, name, lastName}|
|setPersistance|Establece la persistencia de la sesión del usuario autenticado|El context del database store|
|login|Inicia sesión con los datos pasados como parámetro|El context del database store data {email, password}|
|removePushNotificationToken|Elimina el token de notificación del navegador y la base de datos|-|
|logout|Cierra sesión del usuario|El context del database store|
|sendEmailVerification|Envía E-mail de verificación al usuario autenticado|El context del database store|
|isEmailVerified|Comprueba si el E-mail del usuario autenticado está verificado|-|
|sendPasswordResetEmail|Envía E-mail de reseteo de contraseña al correo electrónico pasado com parámetro|El context del database store email|
|updateAccountData|Actualiza en base de datos la información de cuenta del usuario autenticado|El context del database store data {database.js, [lastName], [email]}|
|updateAccountEmail|Actualiza en base de datos el E-mail del usuario autenticado|El context del database store email|
|updateAccountPassword|Actualiza la contraseña del usuario autenticado|El context del database store Contraseña|
|getProfileByUID|Obtiene de base de datos la información de perfil de un usuario|El context del database store ID del usuario|
|getProfile|Obtiene de base de datos la información de perfil del usuario autenticado|El context del database store|
|getMultipleProfilesByUID|Obtiene de base de datos la información de varios perfiles de usuario|El context del database store IDs de usuario|
|getProfileByUsername|Obtiene de base de datos la información de perfil de un usuario|El context del database store Nombre de usuario|
|setProfile|Establece en base de datos la información de perfil del usuario autenticado|El context del database store data {username, birthDate, gender, description}|
|setRegistrationCompleted|Establece en base de datos el estado de registro del usuario autenticado como completado|-|
|updateProfile|Actualiza en base de datos la información de perfil del usuario autenticado|El context del database store data {[username], [birthDate], [gender], [description], [knownLanguages], [languagesToLearn]}|
|setLanguages|Establece en base de datos los idiomas del usuario autenticado|El context del database store data {knownLanguages, languagesToLearn}|
|uploadProfileImg|Almacena en Firebase la imagen de perfil del usuario autenticado|El context del database store img|
|uploadImg|Almacena en Firebase una imagen|El context del database store data {path, img}|
|setProfileImg|Establece en base de datos la imagen de perfil del usuario autenticado|El context del database store URL de la imagen en Firebase|
|updateUserLocation|Actualiza en base de datos la localización del usuario autenticado|El context del database store Localización del usuario|
|getLocation|Obtiene de base de datos la localización del usuario autenticado|El context del database store|
|getRatings|Obtiene de base de datos las valoraciones realizadas por el usuario autenticado|El context del database store ratingsInfo/null|
|setRating|Establece una nueva valoración en la base de datos|El context del database store data{id, rating}|
|isNextUsersPageEmpty|Comprueba en la base de datos si la siguiente página en la obtención de usuarios está vacía|El context del database store data{lastUserShowed, limit, filters}|
|getNextUsersPage|Obtiene de la base de datos la siguiente página de usuarios|El context del database store data{lastUserShowed, limit, filters}|
|getNearbyUserIDs|Obtiene de la base de datos los usuarios cercanos al usuario autenticado|El context del database store data{location, maxDistance}|
|getEventByID|Obtiene de la base de datos la información de un evento|El context del database store ID del evento|
|uploadEventHeaderImg|Almacena en Firebase la imagen de cabecera de un evento|El context del database store data{img, eventID}|
|createEvent|Crea y establece en base de datos un evento|El context del database store data {date, description, headerImg, location, involvedLanguages, name}|
|removeEvent|Elimina de la base de datos un evento|El context del database store ID del evento|
|updateEvent|Actualiza en la base de datos la información de un evento|El context del database store data {[date], [description], [headerImg], [location], [involvedLanguages], database.js}|
|getNextEventsPage|Obtiene de la base de datos la siguiente página de eventos|El context del database store data{lastEventShowed, limit}|
|getEventsToBeCelebrated|Obtiene de la base de datos todos los eventos con fecha posterior a la actual|-|
|isNextEventsPageEmpty|Comprueba en la base de datos si la siguiente página de eventos está vacía|El context del database store data{lastEventShowed, limit}|
|addParticipantToEvent|Añade en la base de datos un participante a un evento|El context del database store ID del evento|
|removeParticipantFromEvent|Elimina de un evento a un participante en la base de datos|El context del database store ID del evento|
|createChatMessagesListener|Crea los listeners de los mensajes de un chat en la base de datos|El context del database store ID del chat|
|setMessagesToRead|Actualiza en la base de datos todos los mensajes sin leer de un chat a estado leido|El context del database store data {chatID, messages}|
|addMessagesToChat|Añade en la base de datos un mensaje a un chat|El context del database store data {chatID, message}|
|addChat|Añade en la base de datos un nuevo chat|El context del database store chat {id, users[]}|
|getChatByID|Obtiene de la base de datos la información de un chat|El context del database store ID del chat|
|getTop100RankingUsers|Obtiene de la base de datos el top 100 de los usuarios del ranking|-|

<!-- @vuese:database.js:actions:end -->



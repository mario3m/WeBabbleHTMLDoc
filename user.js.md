# user.js

## Getters

<!-- @vuese:user.js:getters:start -->
|Getter|Description|
|---|---|
|getName|Devuelve el nombre del usuario autenticado|
|getID|Devuelve el ID del usuario autenticado|
|getLastName|Devuelve los apellidos del usuario autenticado|
|getEmail|Devuelve el E-mail del usuario autenticado|
|getRole|Devuelve el rol del usuario autenticado|
|getChats|Devuelve los identificadores de los chats del usuario autenticado|
|getProfile|Devuelve la información de perfil del usuario autenticado|
|getBirthDate|Devuelve la fecha de nacimiento del usuario autenticado|
|getGender|Devuelve el género del usuario autenticado|
|getDescription|Devuelve la descripción del usuario autenticado|
|getProfileImg|Devuelve la imagen de perfil del usuario autenticado|
|getKnownLanguages|Devuelve los idiomas conocidos por el usuario autenticado|
|getLanguagesToLearn|Devuelve los idiomas a practicar por el usuario autenticado|
|getGenderImgByID|Obtiene la imagen asociada a un género|
|getGenderDefaultProfileImgByUserGender|Devuelve la imagen de perfil por defecto|
|getGenderOptionsAsArray|Devuelve los géneros disponibles en la aplicación en forma de Array|
|getLanguageImgByID|Devuelve la imagen correspondiente un idioma|
|getLanguageOptionsAsArray|Devuelve los idiomas disponibles en la aplicación en forma de Array|
|getLanguageFromLanguageOptionsByID|Devuelve la información de un idioma|
|getLocation|Devuelve la localización del usuario|
|getRatings|Devuelve las valoraciones realizadas por el usuario|
|getRating|Devuelve la información de una valoración realizada por el usuario|

<!-- @vuese:user.js:getters:end -->


## Actions

<!-- @vuese:user.js:actions:start -->
|Action|Description|Parameters|
|---|---|---|
|initState|Inicia el state con los datos apropiados|El context del user store|
|resetState|Resetea el estado del user store|El context del user store|
|createAccount|Crea una cuenta de usuario con los datos pasados como parámetro|El context del user store data {email, password, name, lastName}|
|setLanguage|Actualiza y guarda el idioma de la aplicación -----------------------------------------------------------------------------> ~ setLanguage ~                                                             > To set app language for that user                                           > parameters required: lang                                                   > ----------------------------------------------------------------------------->|El context del user store Identificador del idioma|
|generateNotificationToken|Genera un token de notificación y lo guarda|El context del user store|
|updateAccountNameAndLastName|Actualiza y guarda el nombre y apellidos del usuario con los datos pasados como parámetro|El context del user store data {user.js, [lastName]}|
|updateAccountEmail|Actualiza y guarda el E-mail del usuario pasado como parámetro|El context del user store E-mail|
|updateAccountPassword|Actualiza y guarda la contraseña con la pasada como parámetro|El context del user store Contraseña|
|login|Realiza el login del usuario con los datos pasados como parámetro|El context del user store data {email, password}|
|isUserLogged|Comprueba si el usuario está loggeado|El context del user store|
|logout|Cierra la sesión del usuario|El context del user store|
|sendEmailVerification|Envía un correo electrónico de verificación al E-mail del usuario|El context del user store|
|sendPasswordResetEmail|Envía un correo electrónico de reseteo de contraseña al E-mail pasado como parámetro|El context del user store E-mail|
|checkIfEmailIsVerified|Comprueba si el E-mail del usuario está verificado|El context del user store|
|checkIfUsernameIsAlreadyRegistered|Comprueba si un nombre de usuario está registrado en la aplicación|El context del user store Nombre de usuario|
|createProfile|Crea y almacena el perfil del usuario con los datos pasados como parámetro|El context del user store data {username, birthDate, gender, description}|
|updateProfile|Actualiza y guarda el perfil del usuario con los datos pasados como parámetro|El context del user store data {[username], [birthDate], [gender], [description], [knownLanguages], [languagesToLearn]}|
|setLanguages|Actualiza y guarda los idiomas conocidos y a practicar del usuario|El context del user store data {knownLanguages, languagesToLearn}|
|setProfileImg|Actualiza y guarda la imagen de perfil con la pasada como parámetro|El context del user store img|
|setRegistrationCompleted|Actualiza y guarda el estado de registro del usuario como completado|El context del user store|
|getRegistrationState|Obtiene el estado de registro del usuario|El context del user store|
|checkRegistrationState|Evalúa el estado de registro del usuario|El context del user store data {username, gender, description, avgRating, numRatings, knownLanguages, languagesToLearn, profileImg}|
|getCurrentLocation|Obtiene y almacena la localización actual del usuario|-|
|getRatings|Obtiene las valoraciones realizadas por el usuario y las almacena|El context del user store|
|rateUser|Actualiza y guarda una valoración realizada por el usuario con los datos pasados como parámetro|El context del user store data {id, rating}|
|getLocation|Obtiene y almacena la localización del usuario|El context del user store|

<!-- @vuese:user.js:actions:end -->


## Mutations

<!-- @vuese:user.js:mutations:start -->
|Mutation|Description|Parameters|
|---|---|---|
|setName|Actualiza el valor del nombre del usuario autenticado|El state del user store Nombre|
|setLanguage|Actualiza el idioma seleccionado para la aplicación por el usuario autenticado|El state del user store Nombre|
|setLastName|Actualiza el valor de los apellidos del usuario autenticado|El state del user store Apellidos|
|setEmail|Actualiza el valor del E-mail del usuario autenticado|El state del user store E-mail|
|setAccount|Actualiza los valores de los campos de la cuenta del usuario autenticado|El state del user store accountInfo{[email], user.js, [lastName], [profileImg], [id], [chats], [role], [language]}|
|setUsername|Actualiza el valor del nombre de usuario del usuario autenticado|El state del user store Nombre de usuario|
|setBirthDate|Actualiza el valor de la fecha de nacimiento del usuario autenticado|El state del user store Fecha de nacimiento|
|setGender|Actualiza el valor del género del usuario autenticado|El state del user store Género|
|setDescription|Actualiza el valor del descripción del usuario autenticado|El state del user store Descripción|
|setAvgRating|Actualiza el valor de la valoración media del usuario autenticado|El state del user store Valoración media|
|setNumRatings|Actualiza el valor del número de valoraciones al usuario autenticado|El state del user store Número de valoracione|
|setKnownLanguages|Actualiza el valor de los idiomas conocidos por el usuario autenticado|El state del user store Idiomas conocidos|
|setLanguagesToLearn|Actualiza el valor del idiomas a practicar por el usuario autenticado|El state del user store Idiomas a practicar|
|setProfileImg|Actualiza el valor de la imagen de perfil del usuario autenticado|El state del user store Imagen de perfil|
|setRatings|Actualiza el valor de las valoraciones del usuario autenticado|El state del user store Valoraciones|
|setRating|Actualiza el valor de una valoración del usuario autenticado|El state del user store data{id, rating}|
|setProfile|Actualiza los valores de los campos del perfil del usuario autenticado|El state del user store accountInfo{[username], [birthDate], [gender], [description], [avgRating], [numRatings], [knownLanguages], [languagesToLearn], [profileImg]}|
|resetState|Restablece todas las variables del state a sus valores por defecto|El state del user store|
|setLocation|Actualiza el valor de la localización del usuario autenticado|El state del user store Localización|

<!-- @vuese:user.js:mutations:end -->


## State

<!-- @vuese:user.js:state:start -->
|Name|Description|
|---|---|
|id|User account info ID del usuario autenticado|
|undefined|Nombre del usuario autenticado|
|lastName|Apellidos del usuario autenticado|
|email|E-mail del usuario autenticado|
|chats|Lista de identificadores de los chats del usuario autenticado|
|role|Rol del usuario autenticado en la aplicación|
|language|Language seleccionado por el usuario autenticado para la aplicación|
|username|User profile 1st part Nombre de usuario del usuario autenticado|
|birthDate|Fecha de nacimiento del usuario autenticado|
|gender|Género del usuario autenticado|
|description|Descripción del usuario autenticado|
|avgRating|Valoración media del usuario autenticado|
|numRatings|Número de valoraciones realizadas al usuario autenticado|
|knownLanguages|2nd part Idiomas conocidos del usuario autenticado|
|languagesToLearn|Idiomas a practicar del usuario autenticado|
|profileImg|3rd part Imagen de perfil del usuario autenticado|
|location|Geolocation info Localización del usuario autenticado|
|ratings|Ratings info Valoraciones realizadas por el usuario autenticado|
|genderOptions|Constants Géneros disponibles en al aplicación|
|languageOptions|Idiomas disponibles en al aplicación|

<!-- @vuese:user.js:state:end -->



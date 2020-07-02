# users.js

## Getters

<!-- @vuese:users.js:getters:start -->
|Getter|Description|
|---|---|
|getLanguagesByUserID|Devuelve los idiomas conocidos y a practicar de un usuario|
|getGenderFilter|Devuelve el filtro de género en la búsqueda de usuarios|
|getAgeRangeFilter|Devuelve el filtro de edad en la búsqueda de usuarios|
|getLanguageFilter|Devuelve el filtro de idiomas en la búsqueda de usuarios|
|getSearchByUsernameFilter|Devuelve el filtro de nombre de usuario en la búsqueda de usuarios|
|getMaxDistanceFilter|Devuelve el filtro de máxima distancia en la búsqueda de usuarios|
|getMaxDistanceRangesText|Devuelve el texto de los rangos del filtro de máxima distancia en la búsqueda de usuarios|
|getUserByID|Devuelve la informacion de un usuario|
|getNearbyUsersIDs|Devuelve la lista de identificadores de usuarios cercanos|
|getNearbyUsersIDsLength|Utilizado para obtener los datos de los eventos a mostrar en la vista de lista|
|areThereFiltersOn|Devuelve la presencia o no de filtros establecidos|
|getFilters|Devuelve los filtros en un objeto|
|getLastUserShowed|Devuelve la referencia al último usuario mostrado en la búsqueda|
|getSearchedUsers|Devuelve los usuarios a mostrar con toda su información|

<!-- @vuese:users.js:getters:end -->


## Actions

<!-- @vuese:users.js:actions:start -->
|Action|Description|Parameters|
|---|---|---|
|resetState|Resetea el estado del users store|El context del users store|
|getSearchedUsers|Obtiene los usuarios de base de datos que cumplen con los filtros de forma paginada|El context del users store|
|areThereMoreNearbyUsers|Comprueba si quedan usuarios en base de datos que cumplan con los filtros y no hayan sido mostrados ya|El context del users store|
|getNearbyUsersProfiles|Obtiene los usuarios cercanos al usuario autenticado de base de datos que cumplen con los filtros de forma paginada|El context del users store|
|resetSearchedUsers|Resetea la lista de los usuarios almacenados|El context del users store|
|setFilters|Establece todos los filtros de búsqueda|El context del users store filters{gender, ageRange, language, maxDistance, location}|
|getUserByID|Obtiene y almacena la información de un usuario|El context del users store ID del usuario|
|resetFilters|Resetea los filtros de búsqueda de usuarios a sus valores por defecto|El context del users store|

<!-- @vuese:users.js:actions:end -->


## Mutations

<!-- @vuese:users.js:mutations:start -->
|Mutation|Description|Parameters|
|---|---|---|
|resetState|Restablece todas las variables del state a sus valores por defecto|El state del users store|
|setGenderFilter|Actualiza el filtro de género almacenado|El state del users store Identificador de género|
|setAgeRangeFilter|Actualiza el filtro de edad almacenado|El state del users store Filtro de edad|
|setNearbyUsersIDs|Actualiza la lista de identificadores de usuarios a mostrar|El state del users store Lista de identificadores de usuarios a mostrar|
|setLanguageFilter|Actualiza el filtro de idiomas almacenado|El state del users store Filtro de idiomas|
|setLocationFilter|Actualiza el filtro de localización almacenado|El state del users store Filtro de localización|
|setSearchByUsernameFilter|Actualiza el filtro de nombre de usuario almacenado|El state del users store Nombre de usuario|
|setMaxDistanceFilter|Actualiza el filtro de máxima distancia almacenado|El state del users store Filtro de máxima distancia|
|addUser|Añade un usuario a la lista de usuarios almacenados|El state del users store Usuario|
|addSearchedUserID|Añade un ID de usuario a la lista de usuarios a mostrar|El state del users store ID del usuario|
|resetSearchedUsersIDs|Restablece la lista de identificadores de usuarios a mostrar a su valor por defecto|El state del users store|
|setLastUserShowed|Actualiza la referencia al último usuario mostrado en la búsqueda|El state del users store Referencia al último usuario mostrado en la búsqueda|
|addRating|Actualiza los valores agragados de la valoración de un usuario a partir de los valores pasados como parámetro|El state del users store data {id, rating}|

<!-- @vuese:users.js:mutations:end -->


## State

<!-- @vuese:users.js:state:start -->
|Name|Description|
|---|---|
|users|All users retrieved Almacena todos los usuarios obtenidos de la base de datos|
|searchedUsersIDs|User IDs result of the searching process Almacena los identificadores de los usuarios a mostrar|
|lastUserShowed|Almacena una referencia al último usuario mostrado en la búsqueda|
|genderFilter|Filtro de género en la búsqueda de usuarios|
|ageRangeFilter|Filtro de edad en la búsqueda de usuarios|
|languageFilter|Filtro de idiomas en la búsqueda de usuarios|
|searchByUsernameFilter|Filtro de nombre de usuario en la búsqueda de usuarios|
|maxDistanceFilter|Máxima distancia en el filtro de distancia en la búsqueda de usuarios|
|maxDistanceRanges|Rangos en el filtro de distancias en la búsqueda de usuarios|
|maxDistanceRangesText|Texto de los rangos en el filtro de distancias en la búsqueda de usuarios|
|locationFilter|Filtro de distancia con la localización del usuario en la búsqueda de usuarios|
|nearbyUsersIDs|Almacena los identificadores de los usuarios cercanos al usuario autenticado|

<!-- @vuese:users.js:state:end -->



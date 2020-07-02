# permissions.js

## Getters

<!-- @vuese:permissions.js:getters:start -->
|Getter|Description|
|---|---|
|getIsGeolocationPermissionGranted|Utilizado para obtener el estado de concesión del permiso de geolocalización|
|getIsPushNotificationPermissionGranted|Utilizado para obtener el estado de concesión del permiso de notificaciones|

<!-- @vuese:permissions.js:getters:end -->


## Actions

<!-- @vuese:permissions.js:actions:start -->
|Action|Description|Parameters|
|---|---|---|
|resetState|Resetea el estado del permissions store|El context del permissions store|
|checkForGeolocationPermission|Comprueba el estado del permiso de geolocalización y pide su concesión si todavía no se ha requerido al usuario|El context del permissions store|
|checkForPushNotificationsPermission|Comprueba el estado del permiso de notificaciones y pide su concesión si todavía no se ha requerido al usuario|El context del permissions store|

<!-- @vuese:permissions.js:actions:end -->


## Mutations

<!-- @vuese:permissions.js:mutations:start -->
|Mutation|Description|Parameters|
|---|---|---|
|resetState|Restablece todas las variables del state a sus valores por defecto|El state del permissions store|
|setIsGeolocationPermissionGranted|Actualiza el valor del estado de concesión del permiso de geolocalización con el valor pasado como parámetro|El state del permissions store El estado de concesión del permiso de geolocalización|
|setIsPushNotificationPermissionGranted|Actualiza el valor del estado de concesión del permiso de notificaciones con el valor pasado como parámetro|El state del permissions store El estado de concesión del permiso de notificaciones|

<!-- @vuese:permissions.js:mutations:end -->


## State

<!-- @vuese:permissions.js:state:start -->
|Name|Description|
|---|---|
|isGeolocationPermissionGranted|Almacena el estado de concesión del permiso de geolocalización|
|isPushNotificationPermissionGranted|Almacena el estado de concesión del permiso de notificaciones|

<!-- @vuese:permissions.js:state:end -->



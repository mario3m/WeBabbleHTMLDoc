# PublicProfile

Componente de representación de un usuario para visualizar tanto el perfil del usuario que está utilizando la aplicación como el de los usuarios con los que puede interactuar, cada uno con sus respectivas funcionalidades

## Props

<!-- @vuese:PublicProfile:props:start -->
|Name|Description|Type|Required|Default|
|---|---|---|---|---|
|profileImage|Imagen de perfil|`String`|`true`|-|
|username|Nombre de usuario|`String`|`true`|-|
|knownLanguages|Idiomas conocidos|`Array`|`true`|-|
|languagesToLearn|Idiomas a practicar|`Array`|`true`|-|
|birthDate|Fecha de nacimiento|`Date`|`true`|-|
|description|Descripción|`String`|`true`|-|
|avgRating|Valoración media|`Number`|`false`|-|
|numRatings|Número de valoraciones|`Number`|`false`|-|
|myRatingIsVisible|Indicación de si mostrar o no valoración|`Boolean`|`true`|-|
|myRating|Valoración media|`Number`|`true`|-|
|uid|Identificador de usuario a representar|`String`|`true`|-|
|myUID|Identificador de usuario autenticado|`String`|`true`|-|

<!-- @vuese:PublicProfile:props:end -->


## Events

<!-- @vuese:PublicProfile:events:start -->
|Event Name|Description|Parameters|
|---|---|---|
|update-user-rating|Se genera al actualizar la valoración al usuario representado por el usuario autenticado|El parámetro es un Number representa la nueva valoración|

<!-- @vuese:PublicProfile:events:end -->


## Methods

<!-- @vuese:PublicProfile:methods:start -->
|Method|Description|Parameters|
|---|---|---|
|openRateUserDialog|Abre el diálogo de valoración del usuario representado|-|
|removeUserRating|Elimina la valoración realizada al usuario representado por el usuario autenticado|-|
|setUserRating|Establece la valoración seleccionada por el usuario autenticado para el usuario representado|-|
|openChatWithUser|Prepara y redirige al usuario autenticado a su de chat con el usuario representado|-|

<!-- @vuese:PublicProfile:methods:end -->



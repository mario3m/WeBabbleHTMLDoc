# SearchHome

Página de búsqueda de usuarios

## Methods

<!-- @vuese:SearchHome:methods:start -->
|Method|Description|Parameters|
|---|---|---|
|onScroll|Detecta cuando se ha realizado scroll en la página|-|
|toTop|Realiza un scroll automático al inicio de la página|-|
|getLanguagesByUserID|Devuelve los idiomas del usuario con el ID pasado como parámetro|El parámetro es un String que representa el ID del usuario a mostrar|
|listUsers|Obtiene los usuarios a presentar de forma paginada y que cumplen con lo requerido por el usuario autenticado|-|
|listUsersByUsername|Obtiene los usuarios a presentar de forma paginada y cuyo nombre de usuario coincide total o parcialmente con el especificado por el usuario autenticado|-|
|resetSearchingFilters|Elimina los filtros establecidos para la búsqueda de usuarios|-|
|openUserProfile|Redirige a la página de visualización del perfil del usuario con el ID pasado como parámetro|El parámetro es un String que representa el ID del usuario seleccionado por el usuario autenticado|
|openSearchFilter|Redirige a la página de establecimiento de filtros para la búsqueda de usuarios|-|
|initUsers|Carga usuarios hasta llenar la pantalla|-|

<!-- @vuese:SearchHome:methods:end -->


## Watch

<!-- @vuese:SearchHome:watch:start -->
|Name|Description|Parameters|
|---|---|---|
|searchByUsernameField|Observa el campo de búsqueda por nombre de usuario para borrar el filtro cuando el usuario autenticado resetea dicho campo|-|

<!-- @vuese:SearchHome:watch:end -->



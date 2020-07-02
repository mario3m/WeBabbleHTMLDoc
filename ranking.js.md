# ranking.js

## Getters

<!-- @vuese:ranking.js:getters:start -->
|Getter|Description|
|---|---|
|getRankingUsersToShow|Utilizado para obtener los usuarios a mostrar con todos sus datos|
|getLastUserShowed|Utilizado para obtener el último usuario del ranking mostrado|
|getRankedUserByIndex|Utilizado para obtener los datos de un usuario según su posición en el ranking|
|getRankingUsers|Utilizado para devolver todos los usuarios del ranking obtenidos de base de datos|

<!-- @vuese:ranking.js:getters:end -->


## Actions

<!-- @vuese:ranking.js:actions:start -->
|Action|Description|Parameters|
|---|---|---|
|initState|Inicia el state con los datos apropiados|El context del ranking store|
|getRankingUsers|Obtiene el top 100 de los usuarios del ranking|El context del ranking store|
|getPagedRankingUsers|Añade los siguientes usuarios a mostrar (tantos como el tamaño de página establecido)|El context del ranking store|
|areThereMoreRankingUsersToShow|Determina si hay usuarios del ranking por mostrar|El context del ranking store|
|resetState|Resetea el estado del ranking store|El context del ranking store|

<!-- @vuese:ranking.js:actions:end -->


## Mutations

<!-- @vuese:ranking.js:mutations:start -->
|Mutation|Description|Parameters|
|---|---|---|
|resetState|Restablece todas las variables del state a sus valores por defecto|El state del ranking store|
|setRankingUsers|Asigna los usuarios pasados como parámetro a la variable del estado rankingUsers|El state del ranking store Array con los usuarios del ranking a añadir|
|setLastUserShowed|Guarda la referencia al último usuario del ranking mostrado|El state del ranking store Referencia al último usuario del ranking mostrado|
|addRankingUserID|Añade un nuevo ID de usuario a mostrar a rankingUsersIDs|El state del ranking store ID del usuario a añadir a rankingUsersIDs|

<!-- @vuese:ranking.js:mutations:end -->


## State

<!-- @vuese:ranking.js:state:start -->
|Name|Description|
|---|---|
|lastUserShowed|Referencia al último usuario mostrado en el ranking y se utiliza para la paginación del mismo|
|rankingUsers|Almacena todos los usuarios del ranking obtenidos de la base de datos|
|rankingUsersIDs|Almacena los identificadores de los usuarios del ranking a mostrar|

<!-- @vuese:ranking.js:state:end -->



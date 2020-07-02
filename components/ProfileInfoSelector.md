# ProfileInfoSelector

Selector de información de perfil

## Props

<!-- @vuese:ProfileInfoSelector:props:start -->
|Name|Description|Type|Required|Default|
|---|---|---|---|---|
|showUsernameField|Indicación de si mostrar o no el campo para introducir el nombre de usuario|`Boolean`|`false`|-|
|birthDateInitialValue|Indicación de si mostrar o no el campo para introducir el nombre de usuario|`Date`|`true`|-|
|genderInitialValue|Indicación de si mostrar o no el campo para introducir el nombre de usuario|`String`|`false`|-|
|descriptionInitialValue|Indicación de si mostrar o no el campo para introducir el nombre de usuario|`String`|`false`|-|

<!-- @vuese:ProfileInfoSelector:props:end -->


## Events

<!-- @vuese:ProfileInfoSelector:events:start -->
|Event Name|Description|Parameters|
|---|---|---|
|dataValidityUpdate|Se genera al actualizar la información|El parámetro es un Objeto que representa la información del formulario y la validez de la misma|

<!-- @vuese:ProfileInfoSelector:events:end -->


## Methods

<!-- @vuese:ProfileInfoSelector:methods:start -->
|Method|Description|Parameters|
|---|---|---|
|formUpdated|Evalúa la validez de los datos introducidos|-|
|validBirthDate|Evalúa si la fecha de nacimiento introducida cumple con las condiciones de usuario de la aplicación|-|

<!-- @vuese:ProfileInfoSelector:methods:end -->


## Computed

<!-- @vuese:ProfileInfoSelector:computed:start -->
|Computed|Type|Description|From Store|
|---|---|---|---|
|localeLang|-|Devuelve el idioma local en i18n para aplicarlo al selector de fecha|No|

<!-- @vuese:ProfileInfoSelector:computed:end -->


## Watch

<!-- @vuese:ProfileInfoSelector:watch:start -->
|Name|Description|Parameters|
|---|---|---|
|birthDate|Observa la fecha de nacimiento y cuando se actualiza, guarda su representación en texto i18n|-|

<!-- @vuese:ProfileInfoSelector:watch:end -->



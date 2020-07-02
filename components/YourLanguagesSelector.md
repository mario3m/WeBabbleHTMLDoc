# YourLanguagesSelector

Selector de lenguages conocidos y a practicar

## Props

<!-- @vuese:YourLanguagesSelector:props:start -->
|Name|Description|Type|Required|Default|
|---|---|---|---|---|
|knownLanguagesInitialValue|Indicación de si mostrar o no el campo para introducir el nombre de usuario|`Array`|`true`|-|
|languagesToLearnInitialValue|Indicación de si mostrar o no el campo para introducir el nombre de usuario|`Array`|`false`|-|

<!-- @vuese:YourLanguagesSelector:props:end -->


## Events

<!-- @vuese:YourLanguagesSelector:events:start -->
|Event Name|Description|Parameters|
|---|---|---|
|dataValidityUpdate|Se genera al actualizar los idiomas seleccionados|El parámetro  es un Objeto que representa los idiomas seleccionados|

<!-- @vuese:YourLanguagesSelector:events:end -->


## Methods

<!-- @vuese:YourLanguagesSelector:methods:start -->
|Method|Description|Parameters|
|---|---|---|
|removeKnownLanguage|Elimina el idioma seleccionado por el usuario como 'a practicar' de las opciones de idiomas 'conocidos'|El parámetro es el idioma seleccionado|
|removeLanguageToLearn|Elimina el idioma seleccionado por el usuario como 'conocido' de las opciones de idiomas 'a practicar'|El parámetro es el idioma seleccionado|
|validLanguages|Evalúa la validez de los lenguages seleccionados|-|
|filterItemsKnownLanguages|Inicializa los idiomas conocidos|-|
|filterItemsLanguagesToLearn|Inicializa los idiomas a practicar|-|

<!-- @vuese:YourLanguagesSelector:methods:end -->


## Watch

<!-- @vuese:YourLanguagesSelector:watch:start -->
|Name|Description|Parameters|
|---|---|---|
|chips_known_languages|Observa los idiomas seleccionados como conocidos por el usuario y realiza las actualizaciones oportunas|-|

<!-- @vuese:YourLanguagesSelector:watch:end -->



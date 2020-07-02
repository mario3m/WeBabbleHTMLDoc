# EmailVerification

Página de registro verificación de E-mail

## Methods

<!-- @vuese:EmailVerification:methods:start -->
|Method|Description|Parameters|
|---|---|---|
|sendUserEmailVerification|Envía un E-mail de verificación al usuario|-|
|wantToLogout|Abre un diálogo advirtiendo al usuario pidiéndole confirmar que desea cerrar sesión|-|
|logoutUser|Para la ejecución periódica de intervalCheckEmailVerified y cierra la sesión del usuario|-|
|checkEmailVerified|Comprueba si el usuario ha verificado su E-mail y si lo ha hecho, actualiza su estado y lo redirige al siguiente paso del proceso de registro|-|

<!-- @vuese:EmailVerification:methods:end -->



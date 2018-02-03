  Creación del formulario
  =======================
El formulario comienza con la etiqueta
el formulario obtendrá la función restringir(), que atreves de un js restringiremos los campos. -action: le indicas la localización -metod: con que método http se envía la información (“get”, ”pos”). El formulario contiene 11 campos cada una con un label. 
-El campo de nombre, apellidos y dirección serán de tipo texto. 
-e-mail será de texto simple de tipo email, que aceptara solo una dirección de correo electrónico. -Hay dos campos para que serán de tipo “password”, donde introduciremos la contraseña y habrá un segundo campo donde confirmaremos la contraseña. La contraseña deberá contener 8 o más caracteres por lo que deberá contener una letra mayúscula una minúscula un número y un valor alfanumérico obligatoriamente (?=.[A-Z])(?=.[a-z])(?=.*[\w]).{8,}. -Hay un campo de tipo fecha donde introduciremos la fecha de nacimiento. -Un campo de tipo “select” donde se elegirá el país -Hay dos campos de tipo “checkbox”, que tendremos que dar check para continuar. -Un botón puede ser de varios tipos:
Un botón que se llama “Crear cuenta” que será de tipo submit que tomar la función registro().

Un botón que se llama “Reiniciar” que será e tipo reset.

  Implementación de la Cookie
  ===========================
Se crearía la cookie en un función llama setCookie(nombre,valores,fechaExpiracion), donde se le pasar al nombre un valor y la fecha en la que expirara la cookie.

GetCookie() toma como parámetro nombreCookie, crea una variable con el texto a buscar y no se encuentra la cookie te devuelve vacio.

-Hay una función inicio() donde se comprobara si la cookie, del perfil logiado se mantiene abierta se mantendrá abierta hasta cerrar sesión. -Habrá una función registro(), donde extraeremos el nombre y la contraseña y se la asignaremos al setCookie().

-En la función login(), comprueba si la contraseña no es la correcta o no se ha introducido nada; o si es correcta. Si es así haremos login.

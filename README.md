================================================================================
                    GUIA DE USO DEL SISTEMA
                    SISTEMA DE GESTION DE STOCK
================================================================================

Este documento explica como usar el sistema, que opciones posee el menú
y que valores debe ingresar en cada momento.

================================================================================
                    INICIO DEL PROGRAMA
================================================================================

Al ejecutar el programa, aparecerá el MENU DE LOGIN:

   ==================================================
   SISTEMA DE LOGIN
   ==================================================
   1. Login
   2. Registrar
   3. Salir
   ==================================================

Opción 1 - LOGIN:
  - Ingrese su nombre de usuario
  - Ingrese su contraseña
  - Si las credenciales son correctas, ingresara al menú principal
  - Si son incorrectas, se mostrara un mensaje de error

Opción 2 - REGISTRAR:
  - Se le pedirá que ingrese un nombre de usuario
    * Debe ser alfanumérico (solo letras y números, sin espacios)
    * Si presiona Enter sin escribir nada, se cancela el registro
  - Se le pedirá que ingrese una contraseña
    * Debe ser alfanumérica (solo letras y números, sin espacios)
  - Si el usuario ya existe, se mostrara un mensaje de error
  - Si se registro correctamente, podrá hacer login

Opción 3 - SALIR:
  - Termina el programa


================================================================================
                    MENU PRINCIPAL
================================================================================

Una vez que ingresa al sistema, verá el MENU PRINCIPAL:

   ==================================================
   MENU PRINCIPAL
   ==================================================
   1. Ejecutar procesamiento completo
   2. Generar archivos de entrada
   3. Ver productos por categoría
   4. Ver productos con bajo stock
   5. Ver próximos vencimientos
   6. Ver estadísticas
   7. Gestionar usuarios
   8. Salir
   ==================================================

Debe ingresar un numero del 1 al 8 para seleccionar una opción.

OPCION 1 - Ejecutar procesamiento completo:
  - Genera automáticamente todos los archivos (categorías, productos, movimientos)
  - Procesa todos los datos
  - Genera todos los reportes y archivos de salida
  - Muestra el total de productos procesados
  - No requiere ningún input adicional
  - Presione Enter para continuar

OPCION 2 - Generar archivos de entrada:
  - Genera los archivos CSV básicos: categorias.csv, productos.csv, movimientos.csv
  - No requiere ningún input adicional
  - Presione Enter para continuar

OPCION 3 - Ver productos por categoría:
  - Muestra en pantalla todos los productos organizados por categoría
  - Muestra: código, nombre, stock, nivel de stock, tiempo (días), ubicación
  - No requiere ningún input adicional
  - Presione Enter para continuar

OPCION 4 - Ver productos con bajo stock:
  - Le pedirá que ingrese un UMBRAL DE STOCK
    * Ingrese un numero entero (por ejemplo: 20)
    * Si presiona Enter sin escribir nada, se usa el valor por defecto: 20
    * El sistema generara el archivo bajoStock.csv con productos que tengan
      stock menor al umbral ingresado
  - Presione Enter para continuar

OPCION 5 - Ver próximos vencimientos:
  - Le pedirá que ingrese DIAS DE ANTICIPACION
    * Ingrese un numero entero (por ejemplo: 30)
    * Si presiona Enter sin escribir nada, se usa el valor por defecto: 30
    * El sistema generara el archivo proximoVencimiento.csv con productos
      que estén próximos a vencer en los días ingresados
  - Presione Enter para continuar

OPCION 6 - Ver estadísticas:
  - Muestra en pantalla un resumen estadístico por categoría:
    * Menor stock
    * Mayor stock
    * Promedio de stock
    * Top 3 productos con mayor stock
    * Top 3 productos con menor stock
  - Genera el archivo resumen_estadistico.csv
  - No requiere ningún input adicional
  - Presione Enter para continuar

OPCION 7 - Gestionar usuarios:
  - Abre un submenú para gestionar usuarios
  - Vea la sección "MENU DE GESTION DE USUARIOS" mas abajo

OPCION 8 - Salir:
  - Cierra la sesión y termina el programa
  - Muestra mensaje "Hasta luego!"


================================================================================
                    MENU DE GESTION DE USUARIOS
================================================================================

Si selecciona la opción 7 del menú principal, vera:

   ==================================================
   GESTION DE USUARIOS
   ==================================================
   1. Listar usuarios
   2. Modificar contraseña
   3. Eliminar usuario
   4. Volver al menú principal
   ==================================================

Debe ingresar un numero del 1 al 4 para seleccionar una opción.

OPCION 1 - Listar usuarios:
  - Muestra la lista de todos los usuarios registrados (máximo 20)
  - No requiere ningún input adicional
  - Presione Enter para continuar
  - Después vuelve al menú de gestión de usuarios

OPCION 2 - Modificar contraseña:
  - Le pedirá que ingrese el NOMBRE DE USUARIO a modificar
    * Ingrese el nombre del usuario cuya contraseña quiere cambiar
    * Si presiona Enter sin escribir nada, se cancela la operación
  - Le pedirá que ingrese la NUEVA CONTRASENA
    * Debe ser alfanumérica (solo letras y números, sin espacios)
  - Si el usuario existe, se modificara la contraseña
  - Presione Enter para continuar
  - Después vuelve al menú de gestión de usuarios

OPCION 3 - Eliminar usuario:
  - Le pedirá que ingrese el NOMBRE DE USUARIO a eliminar
    * Ingrese el nombre del usuario que desea eliminar
  - Le pedirá CONFIRMACION
    * Ingrese 's' para confirmar la eliminación
    * Ingrese 'n' para cancelar la operación
  - Si confirma, el usuario será eliminado permanentemente
  - Presione Enter para continuar
  - Después vuelve al menú de gestión de usuarios

OPCION 4 - Volver al menú principal:
  - Regresa al menú principal sin hacer ninguna accion
  - No requiere ningún input adicional


================================================================================
                    TIPOS DE ENTRADA VALIDOS
================================================================================

NOMBRE DE USUARIO:
  - Solo letras y números (alfanumérico)
  - NO puede tener espacios
  - Ejemplos validos: "gerardo123", "Usuario1", "admin2025"
  - Ejemplos inválidos: "gerardo 123", "usuario@", "mi usuario"

CONTRASENA:
  - Solo letras y números (alfanumérico)
  - NO puede tener espacios
  - Ejemplos validos: "clave123", "Password1", "abc456"
  - Ejemplos inválidos: "clave 123", "pass@word", "mi clave"

NUMEROS ENTEROS:
  - Para opciones de menú: debe ser un numero del rango permitido
  - Para umbral de stock: debe ser un numero entero positivo (ej: 20, 50, 100)
  - Para días de anticipación: debe ser un numero entero positivo (ej: 30, 60, 90)
  - Si ingresa algo invalido o presiona Enter sin escribir, se usa el valor por defecto

CONFIRMACION:
  - Para eliminar usuario: ingrese 's' (si) o 'n' (no)
  - No importa si es mayúscula o minúscula


================================================================================
                    MENSAJES Y NAVEGACION
================================================================================

Después de cada operación, vera el mensaje:
  "aprete enter para seguir"

Esto significa que debe presionar la tecla Enter para continuar al siguiente paso.

ERRORES COMUNES:
  - "Error: Debe ingresar un numero valido"
    * Usted ingreso algo que no es un numero cuando se esperaba un numero
    * Intente nuevamente ingresando un numero

  - "Usuario o contraseña incorrectos"
    * Las credenciales ingresadas no coinciden con ningún usuario registrado
    * Verifique que escribió correctamente usuario y contraseña

  - "El usuario X ya existe"
    * Intento registrar un usuario que ya esta registrado
    * Use otro nombre de usuario o haga login si ya tiene cuenta

  - "Error: Opción X no valida"
    * Ingreso un numero que no corresponde a ninguna opción del menú
    * Verifique que el numero este en el rango permitido


================================================================================
                    ARCHIVOS GENERADOS
================================================================================

El sistema genera los siguientes archivos CSV:

ARCHIVOS DE ENTRADA (generados por opción 2 o 1):
  - categorias.csv: Lista de categorías de productos
  - productos.csv: Lista de productos con sus datos
  - movimientos.csv: Registro de movimientos de stock

ARCHIVOS DE SALIDA (generados automáticamente):
  - porcentajeCategoria.csv: Porcentaje de productos por categoría
  - porcentajeStockMayor20.csv: Porcentaje de productos con stock mayor a 20
  - bajoStock.csv: Productos con stock bajo (umbral configurable)
  - proximoVencimiento.csv: Productos próximos a vencer
  - resumen_estadistico.csv: Resumen estadístico por categoría

ARCHIVO DE LOG:
  - bitacora.log: Registro de todas las acciones del sistema


================================================================================
                    FIN DE LA GUIA
================================================================================

Si tiene dudas sobre el uso del sistema, consulte esta guía o contacte
al administrador del sistema.



1. ~Joomprosubs > option~
    * No se ven las acciones
    * Probablemente esté mal el archivo access.xml


2. ~Incluir language traducciones~
    * Hay que meterlas en el build

3. ~Añadir opciones del menú componentes en el manifiesto~

4. Aspecto del componente: formulario "New"
    * Guiarse por cómo se hace en com_users o com_categories
    * tmpl/default.php

5. Aspecto del componente: Manager
    * Guiarse por cómo se hace en com_users o com_categories
    * tmpl/default.php

6. Arreglar los botones de selección para acciones en submanager
    * Guiarse por cómo se hace en com_users o com_categories

7. JoomprosubsHelper::getActions()
    * Usar forma estándar (ver dudas)

8. JoomprosubsViewSubmanager::addToolbar
    * Botón New no se visualiza => Se necesita crear una categoría primero. why ?
    * Puede ser cuestión de permisos (ver punto 1)


9. Acciones en Submanager sin efecto
    * No ordena
    * No filtra



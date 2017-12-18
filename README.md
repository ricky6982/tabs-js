# tabs-js

Interfaz de usuario para ordenar los formularios en varias pestañas de tal forma que mejore la experiencia del usuario y se evite la creación de formularios muy extensos.

## Descripción
La cantidad de tabs estará definida por el desarrollador, cada tab contendra un formulario relaciónado con el objeto de Dominio.
Por ejemplo la carga de un Producto podria estar compuesta por las siguientes Caracteristicas:
   - Nombre
   - Codigo de Barra
   - Descripción
   - Imagen 
   - Precio en diferentes listas de precios
   - Proveedores
   - Precios en Proveedores
   - ...

La motivación principal es tener formularios enfocados a caracteristicas principales, en el caso anterior se puede tener 3 Tabs
 - Tab 1: Datos del Producto 
    - Nombre
    - Código de Barra
    - Descripción
    - Imagen
 - Tab 2: Lista de Precios
    - Precios del mismo producto en diferentes listas de precios
 - Tab 3: Proveedores
    - Proveedores
    - Precios en Proveedores
    
### Características

  - Guardar formulario actual y cambiar al siguiente Tab.
  - Verifica si el formulario actual ha cambiado y preguntar al usuario si desea guardarlo.
  - Navegabilidad por tabs (siguiente, anterior, tab especifico, url)
  
### Methods (Draft)

```
var cardTabs = new CardTabs('#menu');

cardTabs.CurrentTab(): Returns de id tab
cardTabs.NextTab(): Hide Current tab and show the next tab
cardTabs.BackTab(): Hide Current tab and show the previous tab
```

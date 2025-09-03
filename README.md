# git remote add origin https://github.com/asesorsordos/Contabilidad-IPUC.git

Una aplicación web simple y de una sola página para llevar un registro de ingresos y egresos. Diseñada para ser fácil de usar, funciona completamente en el navegador sin necesidad de un servidor o base de datos externa.

## Características Principales

- **Gestión de Asientos:** Crear, editar y visualizar asientos contables (ingresos y egresos).
- **Resumen Financiero:** Visualiza totales de ingresos, egresos y el saldo actual en tiempo real.
- **Filtrado por Fondos:** Filtra los asientos y los totales por fondos específicos (Fondo Local, Misiones, Jóvenes, etc.).
- **Generación de Recibos:** Genera e imprime recibos detallados para cada transacción.
- **Arqueo de Caja:** Una herramienta para facilitar el conteo de efectivo físico y compararlo con el saldo del sistema para el "Fondo Local".
- **Exportación a CSV:** Exporta la vista actual de los asientos a un archivo `.csv` para respaldos o análisis en hojas de cálculo.
- **Persistencia de Datos:** Todos los datos se guardan localmente en tu navegador usando `localStorage`.

## ¿Cómo usarlo?

Simplemente abre el archivo `Index.html` en cualquier navegador web moderno (como Google Chrome, Mozilla Firefox, Microsoft Edge, etc.). No se requiere instalación ni conexión a internet una vez cargado.

1.  Descarga el archivo `Index.html`.
2.  Haz doble clic sobre él para abrirlo en tu navegador predeterminado.
3.  ¡Listo! Comienza a registrar tus movimientos contables.

## ¡Importante! Sobre el Almacenamiento de Datos

Esta aplicación utiliza `localStorage` del navegador para guardar toda la información. Esto tiene algunas implicaciones importantes:

- **Los datos son locales:** La información se almacena **únicamente en la computadora y el navegador** que estás utilizando. No se sincroniza entre diferentes dispositivos o navegadores.
- **Riesgo de pérdida de datos:** Si limpias los datos de tu navegador (caché, cookies, historial de sitio), **perderás toda la información contable registrada**.
- **Respaldo manual:** Se recomienda encarecidamente utilizar la función **"Exportar a CSV"** de forma regular para crear copias de seguridad de tus datos.

## Funcionalidades Detalladas

### Nuevo Asiento Contable
- **Fecha:** La fecha en que se realizó la transacción.
- **Concepto:** Una descripción breve de la transacción.
- **Recibido de / Pagado a:** Nombre opcional de la persona o entidad involucrada.
- **Tipo de Movimiento:** Ingreso o Egreso.
- **Monto:** El valor de la transacción.
- **Fondo Asignado:** El fondo o departamento al que pertenece el movimiento.

### Historial de Asientos
- Muestra una lista de todas las transacciones, las más recientes primero.
- Permite **editar** cualquier asiento existente.
- Permite generar un **recibo** para cualquier transacción.

### Arqueo de Caja
- Esta función está diseñada para el **"Fondo Local"**.
- Muestra el saldo que debería haber en caja según los registros del sistema.
- Proporciona una tabla para que ingreses la cantidad de billetes y monedas que tienes físicamente.
- Calcula el total físico y muestra la diferencia (sobrante, faltante o si cuadra).

## Tecnologías Utilizadas

- **HTML5**
- **CSS3**
- **Bootstrap 5.3** para el diseño y los componentes de la interfaz.
- **JavaScript (Vanilla)** para toda la lógica de la aplicación.
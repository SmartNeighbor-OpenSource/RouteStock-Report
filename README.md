<div align="center">

# **Universidad Peruana de Ciencias Aplicadas**

[![UPC Logo](https://media.discordapp.net/attachments/610911183339388978/1497066255251804221/UPC_logo_transparente.png?ex=69ec2b19&is=69ead999&hm=ced69157a843edd5c74c1d049127a66e70fd728125fb2a4694bd219328da7de9&=&format=webp&quality=lossless)](https://www.upc.edu.pe)

### **Informe de Trabajo Final**

**Carrera**: Ingeniería de Software

**Curso**: Desarrollo de Aplicaciones Open Source

**Sección**: 1ASI0729-2610-10155

**Profesor**: Hugo Allan Mori Paiva

**Ciclo**: 2026-1

**Startup:** SmartNeighbor

**Nombre del Producto**: RouteStock

**Integrantes**:

Luis Angel Cisneros Salas (U20211B198)
<br>Luis German Tello Quispe (U202317767)
<br>Alison Arrieta (U202312031)
<br>Alfaro Coveñas, Louis Piero (u20191b299)

**Abril del 2026**

</div>

**Contenido**  
[Contenido	4](#contenido)

[Registro de Versiones del Informe	4](#registro-de-versiones-del-informe)

[Project Report Collaboration Insights	4](#project-report-collaboration-insights)

[Contenido	4](#contenido-1)

[Student Outcome	4](#student-outcome)

[1\.	Capítulo I: Introducción	4](#capítulo-i:-introducción)

[1.1	Startup Profile	4](#startup-profile)

[1.1.1	Descripción de la Startup	4](#descripción-de-la-startup)

[1.1.2	Perfiles de integrantes del equipo	4](#perfiles-de-integrantes-del-equipo)

[1.2	Solution Profile	4](#solution-profile)

[1.2.1	Antecedentes y problemática	4](#antecedentes-y-problemática)

[1.2.2	Lean UX Process	4](#lean-ux-process)

[1.3	Segmentos objetivo	4](#segmentos-objetivo)

[2\.	Capítulo II: Requirements Elicitation & Analysis	4](#capítulo-ii:-requirements-elicitation-&-analysis)

[2.1	Competidores	4](#competidores)

[2.1.1	Análisis competitivo	4](#análisis-competitivo)

[2.1.2	Estrategias y tácticas frente a competidores	4](#estrategias-y-tácticas-frente-a-competidores)

[2.2	Entrevistas	5](#entrevistas)

[2.2.1	Diseño de entrevistas	5](#diseño-de-entrevistas)

[2.2.2	Registro de entrevistas	5](#registro-de-entrevistas)

[2.2.3	Análisis de entrevistas	5](#análisis-de-entrevistas)

[2.3	Needfinding	5](#needfinding)

[2.3.1	User Personas	5](#user-personas)

[2.3.2	User Task Matrix	5](#user-task-matrix)

[2.3.3	User Journey Mapping	5](#user-journey-mapping)

[2.3.4	Empathy Mapping	5](#empathy-mapping)

[2.4	Big Picture Event Storming	5](#big-picture-event-storming)

[2.5	Ubiquitous Language	5](#ubiquitous-language)

 ## **3.Capítulo III: Requirements Specification**

## **3.1 User Stories**

| Epic / Story ID | Título | Descripción | Criterios de Aceptación | Relacionado con(Epic ID) |
| :---- | :---- | :---- | :---- | :---- |
| **EP01** | Información del producto en Landing Page | Como visitante, quiero entender qué ofrece RouteStock para decidir si me registro para buscar productos cercanos o para empezar a digitalizar y ofrecer el inventario de mi pequeño negocio. | **Escenario 1: Comprender la propuesta de valor central**  Given el visitante accede a la landing page del sitio web When explora el contenido principal Then comprende que la plataforma conecta a consumidores con bodegas, comercios locales y vendedores ambulantes para encontrar productos en su zona de manera rápida y confiable.  **Escenario 2: Diferenciación y beneficios del servicio**  Given el visitante compara RouteStock con la búsqueda tradicional u otras aplicaciones de delivery When evalúa los beneficios destacados en la página Then identifica que el servicio se enfoca exclusivamente en el comercio de cercanía, permitiendo a los negocios ganar visibilidad sin gran inversión tecnológica y a los usuarios ahorrar tiempo localizando inventario real. |  |
| **EP02** | Crear cuenta como usuario  | Como usuario (comerciante o consumidor), quiero crear una cuenta en RouteStock para acceder a la plataforma y utilizar sus funcionalidades, ya sea para registrar productos y gestionar mi inventario o para buscar productos cercanos de manera rápida y confiable. | **Escenario 1: Iniciar proceso de registro** Given el usuario accede al flujo de creación de cuenta en RouteStockWhen ingresa sus datos básicos (nombre, correo electrónico, contraseña y tipo de usuario: comerciante o consumidor)Then el sistema registra la información y envía un correo de verificación para activar la cuenta **Escenario 2: Confirmar cuenta** Given el usuario recibe el correo de verificación When hace clic en el enlace de activación Then su cuenta queda validada y lista para ser utilizada **Escenario 3: Acceder por primera vez según tipo de usuario** Given el usuario ha confirmado su cuenta When inicia sesión por primera vez Then accede a funcionalidades personalizadas según su perfil: Comerciante: opción para registrar productos e inventario Consumidor: opción para buscar productos cercanos **Escenario 4: Validación de datos obligatorios** Given el usuario se encuentra en el formulario de registro When intenta registrarse sin completar los campos obligatorios o con datos inválidos Then el sistema muestra mensajes de error y no permite continuar con el registro |  |
| **EP03** | Gestión de Inventario (Comerciante)  | Como comerciante (bodega, negocio local o vendedor ambulante), quiero gestionar mi inventario dentro de RouteStock para registrar, actualizar y mantener visibles mis productos, de manera que los usuarios puedan encontrarlos fácilmente y mejorar mis oportunidades de venta. | **Escenario 1: Registrar productos** Given el comerciante ha iniciado sesión en la plataforma When ingresa la información de un producto (nombre, precio, disponibilidad u otros datos básicos) Then el sistema guarda el producto y lo muestra como disponible en su inventario **Escenario 2: Actualizar inventario** Given el comerciante tiene productos registrados When modifica la información de un producto (precio, stock o disponibilidad) Then el sistema actualiza los datos y refleja los cambios en la plataforma **Escenario 3: Visualizar productos registrados** Given el comerciante ha registrado productos en su inventario When accede a la sección de inventario Then el sistema muestra la lista de productos disponibles con su información actualizada |  |
| **EP04** | Búsqueda y Exploración (Consumidor) | Como consumidor, quiero buscar y explorar productos cercanos en RouteStock para encontrar de manera rápida y confiable lo que necesito, considerando la disponibilidad en negocios locales y mi ubicación. | **Escenario 1: Buscar producto** Given el consumidor ha ingresado a la plataforma When realiza la búsqueda de un producto específico Then el sistema muestra una lista de resultados con los productos disponibles en negocios cercanos **Escenario 2: Visualizar detalles del producto** Given el consumidor obtiene resultados de búsqueda When selecciona un producto Then el sistema muestra información relevante como nombre, precio, disponibilidad y negocio que lo ofrece **Escenario 3: Filtrar resultados** Given el consumidor visualiza los resultados de búsqueda When aplica filtros (por cercanía, disponibilidad u otros criterios) Then el sistema actualiza los resultados mostrando opciones más relevantes según su necesidad |  |
| **EP05** | Gestión de Pedidos y Carrito | Como consumidor, quiero gestionar un carrito de compras y realizar pedidos en RouteStock para seleccionar productos de negocios cercanos, confirmar mi compra y acceder a opciones de entrega o recojo de manera práctica. | **Escenario 1: Agregar productos al carrito** Given el consumidor visualiza un producto disponible When decide agregarlo al carrito Then el sistema incluye el producto en su carrito con la información correspondiente **Escenario 2: Gestionar carrito** Given el consumidor tiene productos en su carrito When modifica la cantidad o elimina productos Then el sistema actualiza el carrito reflejando los cambios realizados **Escenario 3: Confirmar pedido** Given el consumidor tiene productos en su carrito When confirma la compra Then el sistema genera el pedido y registra la información para su procesamiento **Escenario 4: Visualizar estado del pedido** Given el consumidor ha realizado un pedido When accede a sus pedidos Then el sistema muestra el estado del pedido (pendiente, en proceso u otros estados definidos) |  |
| **EP06** | Interacción y Contacto | Como consumidor, quiero poder interactuar y contactar a los comerciantes a través de RouteStock para resolver dudas, confirmar disponibilidad de productos o coordinar detalles de compra, mejorando así la confianza y la experiencia de compra. | **Escenario 1: Iniciar contacto con el comerciante** Given el consumidor visualiza un producto o negocio When decide contactar al comerciante Then el sistema permite enviar un mensaje o solicitud de contacto con la información necesaria **Escenario 2: Recepción de mensajes** Given el comerciante ha sido contactado por un consumidor When accede a sus mensajes Then el sistema muestra la información enviada para que pueda responder o gestionar la solicitud |  |
| **EP07** | API Y Backend | Como desarrollador, quiero implementar la API y la lógica de backend de RouteStock para gestionar de manera segura, eficiente y centralizada la información de usuarios, inventario, búsquedas, pedidos e interacciones, permitiendo el correcto funcionamiento de la plataforma. | **Escenario 1: Gestión de datos desde la API** Given el sistema requiere procesar información de usuarios, productos, inventario o pedidos When el frontend realiza una solicitud al backend Then la API procesa la solicitud y devuelve una respuesta estructurada con los datos correspondientes **Escenario 2: Validación de solicitudes** Given el backend recibe información desde la aplicación When los datos enviados están incompletos, son inválidos o no cumplen las reglas definidas Then el sistema rechaza la solicitud y devuelve un mensaje de validación correspondiente   Given una operación válida es procesada por la API When el backend registra, actualiza o consulta información Then los datos quedan almacenados y disponibles de forma consistente en la base de datos |  |
| **US01** | Ver propuesta de valor | Como visitante, deseo visualizar la propuesta de RouteStock para entender sus beneficios. | **1\.** **Dado** que un visitante ingresa al Landing Page, **Cuando** la página carga, **Entonces** el sistema muestra el Hero principal.  **2\.** **Dado** que el visitante explora, **Cuando** visualiza la sección de beneficios, **Entonces** el sistema presenta iconos descriptivos. | **EP-01** |
| **US02** | Navegar a los planes | Como visitante comerciante, deseo ver los beneficios de la red para evaluar mi registro. | **1\.** **Dado** que un visitante está en el Landing Page, **Cuando** hace clic en "Para Negocios", **Entonces** el sistema lo desplaza a la sección informativa.  **2\.** **Dado** que el visitante lee la sección, **Cuando** revisa las características, **Entonces** el sistema muestra los pasos para digitalizar. | **EP-01** |
| **US03** | Redirección a la app | Como visitante, deseo un botón de acceso directo para iniciar sesión o registrarme. | **1\.** **Dado** que un visitante hace clic en "Ingresar a la App", **Cuando** la redirección se completa, **Entonces** el sistema muestra el Login.  **2\.** **Dado** que el usuario entra por el Landing Page, **Cuando** carga la app, **Entonces** la URL cambia al dominio de la Web Application. | **EP-01** |
| **US04** | Ver Términos y Cond. | Como visitante, deseo leer los Términos y Condiciones para conocer mis derechos. | **1\.** **Dado** que un visitante está en el Footer, **Cuando** hace clic en "Términos y Condiciones", **Entonces** el sistema muestra la vista legal.  **2\.** **Dado** que el usuario lee el documento, **Cuando** revisa el texto, **Entonces** este abarca normas de responsabilidad y ética. | **EP-01** |
| **US05** | Cambiar idioma (i18n) | Como usuario, deseo poder cambiar el idioma de la plataforma entre Español e Inglés. | **1\.** **Dado** que el usuario hace clic en el selector de idioma, **Cuando** elige "English", **Entonces** la interfaz traduce sus etiquetas.  **2\.** **Dado** que el idioma está en Inglés, **Cuando** el usuario recarga la página, **Entonces** el sistema recuerda su preferencia de idioma. | **EP-01** |
| **US06** | Accesibilidad teclado | Como usuario con discapacidad, deseo navegar por la web usando la tecla Tab. | **1\.** **Dado** que el usuario presiona "Tab", **Cuando** navega por el menú, **Entonces** el foco visual resalta el elemento seleccionado.  **2\.** **Dado** que el usuario utiliza un lector de pantalla, **Cuando** pasa por un botón, **Entonces** el sistema lee el atributo ARIA correspondiente. | **EP-01** |
| **US07** | Registro de consumidor | Como consumidor, deseo crear una cuenta para poder buscar productos cercanos. | **1\.** **Dado** que un consumidor ingresa sus datos válidos, **Cuando** hace clic en "Registrar", **Entonces** el sistema crea la cuenta.  **2\.** **Dado** que el usuario intenta registrarse, **Cuando** deja campos vacíos, **Entonces** el sistema muestra alertas de validación. | **EP-02** |
| **US08** | Registro de comerciante | Como comerciante, deseo registrar mi negocio para digitalizar mi inventario. | **1\.** **Dado** que un comerciante llena el formulario, **Cuando** envía los datos, **Entonces** el sistema registra el perfil.  **2\.** **Dado** que el sistema detecta que el RUC/DNI ya existe, **Cuando** procesa el envío, **Entonces** muestra un mensaje de error por duplicidad. | **EP-02** |
| **US09** | Inicio de sesión | Como usuario registrado, deseo iniciar sesión para acceder a mis funcionalidades. | **1\.** **Dado** que un usuario ingresa credenciales correctas, **Cuando** hace clic en "Entrar", **Entonces** el sistema otorga acceso.  **2\.** **Dado** que el usuario ingresa datos erróneos, **Cuando** intenta autenticarse, **Entonces** el sistema muestra "Credenciales incorrectas". | **EP-02** |
| **US10** | Cerrar sesión | Como usuario autenticado, deseo poder cerrar mi sesión para proteger mi información. | **1\.** **Dado** que un usuario hace clic en "Cerrar sesión", **Cuando** el sistema procesa la orden, **Entonces** invalida el token de acceso.  **2\.** **Dado** que la sesión se cierra, **Cuando** el proceso termina, **Entonces** redirige al usuario a la vista de Login. | **EP-02** |
| **US11** | Checkbox de Términos | Como visitante, deseo aceptar explícitamente los TyC al registrarme. | **1\.** **Dado** que un usuario llena el registro, **Cuando** no marca el checkbox de TyC, **Entonces** el sistema deshabilita el botón de enviar.  **2\.** **Dado** que el usuario marca el checkbox, **Cuando** hace clic en registrar, **Entonces** el sistema permite la transacción. | **EP-02** |
| **US12** | Auth API Google | Como visitante, deseo iniciar sesión usando mi cuenta de Google mediante una API externa. | **1\.** **Dado** que el usuario hace clic en "Continuar con Google", **Cuando** autoriza la app, **Entonces** el sistema consume la API y crea la sesión.  **2\.** **Dado** que el usuario cancela el flujo de Google, **Cuando** la ventana se cierra, **Entonces** el sistema muestra un mensaje de cancelación. | **EP-02** |
| **US13** | Notificación email API | Como usuario, deseo recibir un correo de confirmación al registrarme usando un API externo. | **1\.** **Dado** que el usuario completa su registro, **Cuando** el backend procesa la solicitud, **Entonces** consume una API de correos (ej. SendGrid) para enviar la confirmación.  **2\.** **Dado** que el correo se envía, **Cuando** el usuario lo abre, **Entonces** visualiza un diseño responsivo de bienvenida. | **EP-02** |
| **US14** | Editar perfil de negocio | Como comerciante, deseo editar la información de mi negocio para mantenerla actualizada. | **1\.** **Dado** que un comerciante modifica su horario, **Cuando** guarda los cambios, **Entonces** el sistema actualiza la base de datos.  **2\.** **Dado** que los cambios son guardados, **Cuando** un cliente visita el perfil, **Entonces** visualiza los datos actualizados. | **EP-03** |
| **US15** | Añadir nuevo producto | Como comerciante, deseo agregar un producto a mi inventario para que sea visible. | **1\.** **Dado** que el comerciante ingresa nombre y precio, **Cuando** guarda, **Entonces** el sistema lo añade al inventario.  **2\.** **Dado** que se añade un producto, **Cuando** no se incluye un precio válido, **Entonces** el sistema impide el guardado. | **EP-03** |
| **US16** | Editar precio | Como comerciante, deseo modificar el precio de un producto para ajustarme al mercado. | **1\.** **Dado** que el comerciante actualiza el campo de precio y confirma, **Cuando** el sistema procesa, **Entonces** guarda el nuevo valor.  **2\.** **Dado** que el precio cambia, **Cuando** finaliza, **Entonces** muestra una notificación de éxito. | **EP-03** |
| **US17** | Eliminar producto | Como comerciante, deseo eliminar un producto que ya no ofrezco. | **1\.** **Dado** que el comerciante pulsa "Eliminar", **Cuando** el sistema detecta la acción, **Entonces** pide una confirmación previa.  **2\.** **Dado** que el usuario confirma, **Cuando** se ejecuta la orden, **Entonces** el producto desaparece del inventario. | **EP-03** |
| **US18** | Marcar sin stock | Como comerciante, deseo cambiar el estado a "agotado" para informar a mis clientes. | **1\.** **Dado** que un producto se queda sin unidades, **Cuando** se activa "Agotado", **Entonces** el sistema cambia la etiqueta visual.  **2\.** **Dado** que un ítem está agotado, **Cuando** un consumidor busca, **Entonces** el sistema lo oculta de los resultados. | **EP-03** |
| **US19** | Buscar por nombre | Como consumidor, deseo usar una barra de búsqueda para encontrar productos. | **1\.** **Dado** que un consumidor escribe un producto y presiona enter, **Cuando** el sistema busca, **Entonces** muestra los negocios que lo ofrecen.  **2\.** **Dado** que no hay coincidencias, **Cuando** termina la búsqueda, **Entonces** el sistema muestra "No se encontraron resultados". | **EP-04** |
| **US20** | Explorar por categoría | Como consumidor, deseo filtrar comercios por tipo para elegir dónde comprar. | **1\.** **Dado** que el consumidor elige "Bodega", **Cuando** se aplica el filtro, **Entonces** el sistema muestra solo esos negocios.  **2\.** **Dado** que se cambia a "Ambulante", **Cuando** procesa la solicitud, **Entonces** actualiza la lista con vendedores registrados. | **EP-04** |
| **US21** | Ver detalle de comercio | Como consumidor, deseo entrar al perfil de un negocio para ver su catálogo completo. | **1\.** **Dado** que el consumidor hace clic en un comercio, **Cuando** carga la vista, **Entonces** el sistema muestra el catálogo.  **2\.** **Dado** que la vista de detalle carga, **Cuando** el usuario hace scroll, **Entonces** muestra la información de contacto. | **EP-04** |
| **US22** | Ver ubicación en Mapa | Como consumidor, deseo ver la ubicación exacta del comercio en un mapa interactivo. | **1\.** **Dado** que el consumidor visualiza el perfil del negocio, **Cuando** carga la sección de ubicación, **Entonces** el sistema carga un mapa vía API externa.  **2\.** **Dado** que el usuario interactúa con el mapa, **Cuando** hace zoom, **Entonces** la API renderiza el mapa sin perder el pin del local. | **EP-04** |
| **US23** | Ver promedio de estrellas | Como consumidor, deseo ver la calificación promedio de un comercio antes de comprar. | **1\.** **Dado** que el consumidor busca locales, **Cuando** aparecen los resultados, **Entonces** el sistema muestra las estrellas junto al nombre del local.  **2\.** **Dado** que un negocio no tiene reseñas, **Cuando** se visualiza su perfil, **Entonces** el sistema muestra el texto "Nuevo negocio". | **EP-04** |
| **US24** | Añadir ítem al carrito | Como consumidor, deseo agregar productos a un carrito virtual. | **1\.** **Dado** que el consumidor hace clic en "Agregar", **Cuando** el sistema procesa, **Entonces** incrementa el contador del carrito.  **2\.** **Dado** que se agrega un ítem repetido, **Cuando** se actualiza, **Entonces** incrementa la cantidad sin duplicar la fila. | **EP-05** |
| **US25** | Confirmar pedido | Como consumidor, deseo enviar mi lista de compra al comerciante. | **1\.** **Dado** que el consumidor confirma el pedido, **Cuando** se completa la transacción, **Entonces** el sistema genera una orden "Pendiente".  **2\.** **Dado** que el pedido se confirma, **Cuando** se crea la orden, **Entonces** el sistema limpia automáticamente el carrito. | **EP-05** |
| **US26** | Ver pedidos entrantes | Como comerciante, deseo ver los pedidos de los clientes para prepararlos. | **1\.** **Dado** que el comerciante accede a "Pedidos", **Cuando** la vista carga, **Entonces** el sistema muestra las solicitudes nuevas primero.  **2\.** **Dado** que hay pedidos pendientes, **Cuando** los revisa, **Entonces** el sistema muestra el detalle de productos. | **EP-05** |
| **US27** | Aceptar pedido | Como comerciante, deseo marcar un pedido como "Listo" para avisar al cliente. | **1\.** **Dado** que un pedido ha sido preparado, **Cuando** el comerciante pulsa "Marcar como listo", **Entonces** el sistema actualiza el estado.  **2\.** **Dado** que el estado cambia, **Cuando** se refresca, **Entonces** el sistema marca el pedido con un color distintivo. | **EP-05** |
| **US28** | Ver estado de mis pedidos | Como consumidor, deseo revisar mis pedidos para saber si puedo ir a recogerlos. | **1\.** **Dado** que el consumidor revisa "Mis Compras", **Cuando** carga el historial, **Entonces** el sistema muestra el estado de cada pedido.  **2\.** **Dado** que un pedido cambia a "Listo", **Cuando** el usuario ingresa, **Entonces** el sistema actualiza la etiqueta visualmente. | **EP-05** |
| **US29** | Elegir tipo de entrega | Como consumidor, deseo poder elegir entre Delivery o Recojo en tienda para mi pedido. | **1\.** **Dado** que el consumidor confirma el carrito, **Cuando** selecciona la opción de entrega, **Entonces** el sistema habilita el campo de "Dirección" si elige Delivery.  **2\.** **Dado** que elige Recojo, **Cuando** avanza, **Entonces** el sistema omite el cobro por envío. | **EP-05** |
| **US30** | Añadir dirección | Como consumidor, deseo registrar mi dirección de entrega para recibir mi pedido. | **1\.** **Dado** que el consumidor selecciona Delivery, **Cuando** ingresa su calle y distrito, **Entonces** el sistema guarda la dirección en la orden.  **2\.** **Dado** que el campo de dirección está vacío, **Cuando** intenta confirmar, **Entonces** el sistema exige llenarlo. | **EP-05** |
| **US31** | Contactar al comerciante | Como consumidor, deseo un botón de WhatsApp para coordinar detalles. | **1\.** **Dado** que el consumidor pulsa el botón de WhatsApp, **Cuando** el sistema procesa, **Entonces** abre la aplicación de mensajería externa.  **2\.** **Dado** que se inicia el contacto, **Cuando** genera el enlace, **Entonces** incluye un mensaje predefinido con el pedido. | **EP-06** |
| **US32** | Historial de ventas | Como comerciante, deseo visualizar un registro de ventas pasadas. | **1\.** **Dado** que el comerciante selecciona un rango de fechas, **Cuando** aplica el filtro, **Entonces** el sistema muestra las ventas del periodo.  **2\.** **Dado** que visualiza el historial, **Cuando** hace clic en una venta, **Entonces** despliega el detalle de los productos. | **EP-06** |
| **US33** | Calificar comercio | Como consumidor, deseo dejar una calificación de 1 a 5 estrellas luego de mi compra. | **1\.** **Dado** que el pedido se marca como completado, **Cuando** el usuario lo revisa, **Entonces** el sistema habilita la opción de calificar.  **2\.** **Dado** que el usuario selecciona 4 estrellas y guarda, **Cuando** el sistema procesa, **Entonces** la calificación se guarda en la base de datos. | **EP-06** |
| **US34** | Endpoint de listado | Como Developer, deseo implementar un endpoint GET de productos. | **1\.** **Dado** que se solicita GET a la ruta de productos, **Cuando** el ID del negocio es correcto, **Entonces** devuelve JSON con código HTTP 200\.  **2\.** **Dado** que el ID de negocio no existe, **Cuando** se consulta, **Entonces** retorna un código HTTP 404\. | **EP-07** |
| **US35** | Endpoint de creación | Como Developer, deseo implementar un endpoint POST para registrar órdenes. | **1\.** **Dado** que la petición POST llega al servidor, **Cuando** los datos son válidos, **Entonces** crea el registro y devuelve código HTTP 201\.  **2\.** **Dado** que el cuerpo del mensaje está incompleto, **Cuando** procesa la orden, **Entonces** retorna un código HTTP 400\. | **EP-07** |
| **US36** | Endpoint de registro | Como Developer, deseo crear un endpoint de registro que asegure los datos. | **1\.** **Dado** que se reciben datos de un nuevo usuario, **Cuando** el servidor procesa, **Entonces** encripta la contraseña antes de guardarla.  **2\.** **Dado** que el correo ya está registrado, **Cuando** intenta crear la cuenta, **Entonces** devuelve un error HTTP 409\. | **EP-07** |
| **US37** | Endpoint External API | Como Developer, deseo implementar un endpoint backend para orquestar el envío de correos. | **1\.** **Dado** que el sistema requiere enviar un correo, **Cuando** se llama al servicio interno, **Entonces** este se comunica con el API externa gestionando los tokens.  **2\.** **Dado** que el API externa falla (HTTP 500), **Cuando** el sistema lo detecta, **Entonces** registra el error en los logs sin romper la app. | **EP-07** |
| **US38** | Endpoint Maps Integration | Como Developer, deseo que el frontend consuma correctamente la API de mapas para calcular distancias. | **1\.** **Dado** que el frontend requiere distancia, **Cuando** pasa las coordenadas a la API externa, **Entonces** recibe la respuesta y la muestra en la UI.  **2\.** **Dado** que el usuario deniega el permiso de GPS, **Cuando** la API externa lo solicita, **Entonces** el sistema asume una ubicación genérica de la ciudad. | **EP-07** |
| **US39** | Endpoint i18n config | Como Developer, deseo configurar los diccionarios de traducciones en el frontend. | **1\.** **Dado** que la app inicializa, **Cuando** detecta el idioma del navegador, **Entonces** carga el archivo JSON correspondiente (es o en).  **2\.** **Dado** que falta una llave de traducción, **Cuando** Angular la renderiza, **Entonces** hace fallback al idioma inglés por defecto. | **EP-07** |
| **US40** | Endpoint ARIA tags | Como Developer, deseo asegurar que todos los componentes modales tengan etiquetas ARIA. | **1\.** **Dado** que se abre un modal de producto, **Cuando** el DOM se renderiza, **Entonces** el contenedor principal incluye aria-modal="true".  **2\.** **Dado** que hay botones de cierre de iconos, **Cuando** se inspeccionan, **Entonces** cuentan con un aria-label descriptivo. | **EP-07** |



## **3.2 Impact Mapping**


![](https://media.discordapp.net/attachments/610911183339388978/1497080169888743484/Aspose.Words.096d6980-861d-4cc1-82a4-7999e6da2609.018.png?ex=69ec380e&is=69eae68e&hm=3254221fabc30c35e525ace6f692d3d9604d0f42155dc94fbae0f7a8aaa27b1e&=&format=webp&quality=lossless)



## **3.3 Product Backlog**





| \# Orden | ID | Título | Descripción | Story Points | Sprint |
| :---- | :---- | :---- | :---- | :---- | :---- |
| 1 | **US01** | Ver propuesta de valor | Como visitante, deseo visualizar la propuesta principal de RouteStock para entender los beneficios de la plataforma. | 1 | 1 |
| 2 | **US02** | Navegar a los planes | Como visitante comerciante, deseo ver los beneficios de unirme a la red para evaluar mi registro. | 1 | 1 |
| 3 | **US03** | Redirección a la app | Como visitante, deseo tener un botón de acceso directo para poder iniciar sesión o registrarme rápidamente. | 2 | 1 |
| 4 | **US04** | Ver Términos y Cond. | Como visitante, deseo leer los Términos y Condiciones para conocer mis derechos y responsabilidades. | 1 | 1 |
| 5 | **US05** | Cambiar idioma (i18n) | Como usuario, deseo poder cambiar el idioma de la plataforma entre Español e Inglés para facilitar mi navegación. | 3 | 1 |
| 6 | **US06** | Accesibilidad teclado | Como usuario con discapacidad, deseo navegar por la web usando la tecla Tab para acceder a la información sin mouse. | 3 | 1 |
| 7 | **US07** | Registro de consumidor | Como consumidor, deseo crear una cuenta en la plataforma para poder buscar productos cercanos. | 3 | 1 |
| 8 | **US08** | Registro de comerciante | Como comerciante, deseo registrar mi negocio en la plataforma para poder digitalizar mi inventario. | 5 | 2 |
| 9 | **US09** | Inicio de sesión | Como usuario registrado, deseo iniciar sesión con mis credenciales para acceder a mis funcionalidades personalizadas. | 3 | 2 |
| 10 | **US10** | Cerrar sesión | Como usuario autenticado, deseo poder cerrar mi sesión para proteger mi información personal y de negocio. | 1 | 2 |
| 11 | **US11** | Checkbox de Términos | Como visitante, deseo aceptar explícitamente los TyC al registrarme para cumplir con las normas de seguridad. | 1 | 2 |
| 12 | **US12** | Auth API Google | Como visitante, deseo iniciar sesión usando mi cuenta de Google para agilizar mi acceso a la plataforma. | 8 | 2 |
| 13 | **US13** | Notificación email API | Como usuario, deseo recibir un correo de confirmación al registrarme para validar que mi cuenta fue creada. | 5 | 2 |
| 14 | **US14** | Editar perfil de negocio | Como comerciante, deseo editar la información de mi negocio para mantener mis datos de contacto actualizados. | 3 | 2 |
| 15 | **US15** | Añadir nuevo producto | Como comerciante, deseo agregar un producto a mi inventario para que los clientes locales puedan visualizarlo. | 3 | 2 |
| 16 | **US16** | Editar precio | Como comerciante, deseo modificar el precio de un producto existente para ajustarme a los cambios del mercado. | 2 | 3 |
| 17 | **US17** | Eliminar producto | Como comerciante, deseo eliminar un producto que ya no ofrezco para mantener mi catálogo limpio. | 2 | 3 |
| 18 | **US18** | Marcar sin stock | Como comerciante, deseo cambiar el estado de un producto a "agotado" para no generar falsas expectativas al cliente. | 2 | 3 |
| 19 | **US19** | Buscar por nombre | Como consumidor, deseo usar una barra de búsqueda para encontrar rápidamente un producto específico en mi zona. | 5 | 3 |
| 20 | **US20** | Explorar por categoría | Como consumidor, deseo filtrar los comercios por tipo para elegir entre una bodega o un vendedor ambulante. | 3 | 3 |
| 21 | **US21** | Ver detalle de comercio | Como consumidor, deseo entrar al perfil de un negocio para ver su catálogo completo de productos disponibles. | 3 | 3 |
| 22 | **US22** | Ver ubicación en Mapa | Como consumidor, deseo ver la ubicación exacta del comercio en un mapa interactivo para llegar sin perder tiempo. | 5 | 3 |
| 23 | **US23** | Ver promedio de estrellas | Como consumidor, deseo ver la calificación promedio de un comercio para decidir basándome en la reputación. | 3 | 3 |
| 24 | **US24** | Añadir ítem al carrito | Como consumidor, deseo poder agregar productos de un comercio a un carrito virtual para organizar mi compra. | 3 | 4 |
| 25 | **US25** | Confirmar pedido | Como consumidor, deseo enviar mi lista de compra al comerciante para asegurar que los productos me esperen. | 5 | 4 |
| 26 | **US26** | Ver pedidos entrantes | Como comerciante, deseo ver una lista de los pedidos realizados por los clientes para poder prepararlos con tiempo. | 3 | 4 |
| 27 | **US27** | Aceptar pedido | Como comerciante, deseo marcar un pedido como "Listo" para que el cliente sepa que puede pasar por él. | 2 | 4 |
| 28 | **US28** | Ver estado de pedidos | Como consumidor, deseo revisar el estado de mis pedidos actuales para confirmar si ya están listos para recojo. | 2 | 4 |
| 29 | **US29** | Elegir tipo de entrega | Como consumidor, deseo poder elegir entre Delivery o Recojo en tienda para mayor comodidad en mi compra. | 3 | 4 |
| 30 | **US30** | Añadir dirección | Como consumidor, deseo registrar mi dirección de entrega para que el repartidor sepa dónde llevar mi pedido. | 2 | 4 |
| 31 | **US31** | Contactar al comerciante | Como consumidor, deseo un botón directo para enviar un WhatsApp al vendedor y coordinar detalles finales. | 3 | 4 |
| 32 | **US32** | Historial de ventas | Como comerciante, deseo visualizar un registro de mis ventas pasadas para llevar un control financiero de mi negocio. | 3 | 4 |
| 33 | **US33** | Calificar comercio | Como consumidor, deseo dejar una calificación de 1 a 5 estrellas luego de mi compra para ayudar a otros usuarios. | 3 | 4 |
| 34 | **US34** | Endpoint de listado | Como Developer, deseo implementar un endpoint GET de productos para alimentar la vista del catálogo en el frontend. | 3 | 4 |
| 35 | **US35** | Endpoint de creación | Como Developer, deseo implementar un endpoint POST para registrar nuevas órdenes de compra en la base de datos. | 5 | 4 |
| 36 | **US36** | Endpoint de registro | Como Developer, deseo crear un endpoint de registro que asegure los datos mediante encriptación de contraseñas. | 5 | 4 |
| 37 | **US37** | Endpoint External API | Como Developer, deseo implementar un servicio backend para orquestar el envío de correos mediante una API de terceros. | 5 | 4 |
| 38 | **US38** | Endpoint Maps Integration | Como Developer, deseo que el sistema consuma la API de mapas externa para mostrar las ubicaciones de los negocios. | 5 | 4 |
| 39 | **US39** | Endpoint i18n config | Como Developer, deseo configurar los diccionarios de traducciones en el frontend para soportar múltiples idiomas. | 3 | 4 |
| 40 | **US40** | Etiquetas ARIA | Como Developer, deseo asegurar que todos los componentes tengan etiquetas ARIA para cumplir con los estándares a11y. | 2 | 4 |



[image1]: <data:image/png;base64,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>

[4\.	Capítulo IV: Product Design	5](#capítulo-iv:-product-design)

[4.1	Style Guidelines	5](#style-guidelines)

[4.1.1	General Style Guidelines	5](#general-style-guidelines)

[4.1.2	Web Style Guidelines	5](#web-style-guidelines)

[4.2	Information Architecture	5](#information-architecture)

[4.2.1	Organization Systems	5](#organization-systems)

[4.2.2	Labeling Systems	5](#labeling-systems)

[4.2.3	SEO Tags and Meta Tags	5](#seo-tags-and-meta-tags)

[4.2.4	Searching Systems	6](#searching-systems)

[4.2.5	Navigation Systems	6](#navigation-systems)

[4.3	Landing Page UI Design	6](#landing-page-ui-design)

[4.3.1	Landing Page Wireframe	6](#landing-page-wireframe)

[4.3.2	Landing Page Mock-up	6](#landing-page-mock-up)

[4.4	Web Applications UX/UI Design	6](#web-applications-ux/ui-design)

[4.4.1	Web Applications Wireframes	6](#web-applications-wireframes)

[4.4.2	Web Applications Wireflow Diagrams	6](#web-applications-wireflow-diagrams)

[4.4.3	Web Applications Mock-ups	6](#web-applications-mock-ups)

[4.4.4	Web Applications User Flow Diagrams	6](#web-applications-user-flow-diagrams)

[4.5	Web Applications Prototyping	6](#web-applications-prototyping)

[4.6	Domain-Driven Software Architecture	6](#domain-driven-software-architecture)

[4.6.1	Design-Level Event Storming	6](#design-level-event-storming)

[4.6.2	Software Architecture Context Diagram	6](#software-architecture-context-diagram)

[4.6.3	Software Architecture Container Diagrams	6](#software-architecture-container-diagrams)

[4.6.4	Software Architecture Component Diagrams	6](#software-architecture-component-diagrams)

[4.7	Software Object-Oriented Design	6](#software-object-oriented-design)

[4.7.1	Class Diagrams	6](#class-diagrams)

[4.8	Database Design	6](#database-design)

[4.8.1	Database Diagrams	6](#database-diagrams)

[5\.	Capítulo V: Product Implementation, Validation & Deployment	6](#capítulo-v:-product-implementation,-validation-&-deployment)

[5.1	Software Configuration Management	6](#software-configuration-management)

[5.1.1	Software Development Environment Configuration	6](#software-development-environment-configuration)

[5.1.2	Source Code Management	6](#source-code-management)

[5.1.3	Source Code Style Guide & Conventions	7](#source-code-style-guide-&-conventions)

[5.1.4	Software Deployment Configuration	7](#software-deployment-configuration)

[5.2	Landing Page, Services & Applications Implementation	7](#landing-page,-services-&-applications-implementation)

[5.3	Validation Interviews	7](#validation-interviews)

[5.3.1	Diseño de Entrevistas	7](#diseño-de-entrevistas-1)

[5.3.2	Registro de Entrevistas	7](#registro-de-entrevistas-1)

[5.3.3	Evaluaciones según heurísticas	7](#evaluaciones-según-heurísticas)

[5.4	Video About-the-Product	7](#video-about-the-product)

[Conclusiones	7](#conclusiones)

[Bibliografía	7](#bibliografía)

[Anexos	7](#anexos)

# **Contenido** {#contenido}

# **Registro de Versiones del Informe** {#registro-de-versiones-del-informe}

# **Project Report Collaboration Insights** {#project-report-collaboration-insights}

# **Contenido** {#contenido-1}

# **Student Outcome** {#student-outcome}

1. # **Capítulo I: Introducción** {#capítulo-i:-introducción}

   1. ## **Startup Profile** {#startup-profile}

      1. ### **Descripción de la Startup** {#descripción-de-la-startup}

      2. ### **Perfiles de integrantes del equipo** {#perfiles-de-integrantes-del-equipo}

   2. ## **Solution Profile** {#solution-profile}

      1. ### **Antecedentes y problemática** {#antecedentes-y-problemática}

      2. ### **Lean UX Process** {#lean-ux-process}

         1. #### ***Lean UX Problem Statements***

         2. #### ***Lean UX Assumptions***

         3. #### ***Lean UX Hypothesis Statements***

         4. #### ***Lean UX Canvas***

   3. ## **Segmentos objetivo** {#segmentos-objetivo}

2. # **Capítulo II: Requirements Elicitation & Analysis** {#capítulo-ii:-requirements-elicitation-&-analysis}

   1. ## **Competidores** {#competidores}

      1. ### **Análisis competitivo** {#análisis-competitivo}

      2. ### **Estrategias y tácticas frente a competidores** {#estrategias-y-tácticas-frente-a-competidores}

   2. ## **Entrevistas** {#entrevistas}

      1. ### **Diseño de entrevistas** {#diseño-de-entrevistas}

      2. ### **Registro de entrevistas** {#registro-de-entrevistas}

      3. ### **Análisis de entrevistas** {#análisis-de-entrevistas}

   3. ## **Needfinding** {#needfinding}

      1. ### **User Personas** {#user-personas}

      2. ### **User Task Matrix** {#user-task-matrix}

      3. ### **User Journey Mapping** {#user-journey-mapping}

      4. ### **Empathy Mapping** {#empathy-mapping}

   4. ## **Big Picture Event Storming** {#big-picture-event-storming}

   5. ## **Ubiquitous Language** {#ubiquitous-language}

3. # **Capítulo III: Requirements Specification** {#capítulo-iii:-requirements-specification}

   1. ## **User Stories** {#user-stories}

   2. ## **Impact Mapping** {#impact-mapping}

   3. ## **Product Backlog** {#product-backlog}

4. # **Capítulo IV: Product Design** {#capítulo-iv:-product-design}

   1. ## **Style Guidelines** {#style-guidelines}

      1. ### **General Style Guidelines** {#general-style-guidelines}

      2. ### **Web Style Guidelines** {#web-style-guidelines}

   2. ## **Information Architecture** {#information-architecture}

      1. ### **Organization Systems** {#organization-systems}

      2. ### **Labeling Systems** {#labeling-systems}

      3. ### **SEO Tags and Meta Tags** {#seo-tags-and-meta-tags}

      4. ### **Searching Systems** {#searching-systems}

      5. ### **Navigation Systems** {#navigation-systems}

   3. ## **Landing Page UI Design** {#landing-page-ui-design}

      1. ### **Landing Page Wireframe** {#landing-page-wireframe}

      2. ### **Landing Page Mock-up** {#landing-page-mock-up}

   4. ## **Web Applications UX/UI Design** {#web-applications-ux/ui-design}

      1. ### **Web Applications Wireframes** {#web-applications-wireframes}

      2. ### **Web Applications Wireflow Diagrams** {#web-applications-wireflow-diagrams}

      3. ### **Web Applications Mock-ups** {#web-applications-mock-ups}

      4. ### **Web Applications User Flow Diagrams** {#web-applications-user-flow-diagrams}

   5. ## **Web Applications Prototyping** {#web-applications-prototyping}

   6. ## **Domain-Driven Software Architecture** {#domain-driven-software-architecture}

      1. ### **Design-Level Event Storming** {#design-level-event-storming}

      2. ### **Software Architecture Context Diagram** {#software-architecture-context-diagram}

      3. ### **Software Architecture Container Diagrams** {#software-architecture-container-diagrams}

      4. ### **Software Architecture Component Diagrams** {#software-architecture-component-diagrams}

   7. ## **Software Object-Oriented Design** {#software-object-oriented-design}

      1. ### **Class Diagrams** {#class-diagrams}

   8. ## **Database Design** {#database-design}

      1. ### **Database Diagrams** {#database-diagrams}

5. # **Capítulo V: Product Implementation, Validation & Deployment** {#capítulo-v:-product-implementation,-validation-&-deployment}

   1. ## **Software Configuration Management** {#software-configuration-management}

      1. ### **Software Development Environment Configuration** {#software-development-environment-configuration}

      2. ### **Source Code Management** {#source-code-management}

      3. ### **Source Code Style Guide & Conventions** {#source-code-style-guide-&-conventions}

      4. ### **Software Deployment Configuration** {#software-deployment-configuration}

   2. ## **Landing Page, Services & Applications Implementation** {#landing-page,-services-&-applications-implementation}

   3. ## **Validation Interviews** {#validation-interviews}

      1. ### **Diseño de Entrevistas** {#diseño-de-entrevistas-1}

      2. ### **Registro de Entrevistas** {#registro-de-entrevistas-1}

      3. ### **Evaluaciones según heurísticas** {#evaluaciones-según-heurísticas}

   4. ## **Video About-the-Product** {#video-about-the-product}

# **Conclusiones** {#conclusiones}

# **Bibliografía** {#bibliografía}

# **Anexos** {#anexos}

[image1]: <data:image/png;base64,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>

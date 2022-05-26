# Documentación de Proyecto de Software

**Cátedra:** Trabajo Final ASC, Proyecto de software LSI.

**Profesores:**

- Titular : Dr. Mgter. Lic. Horacio Daniel Kuna
- JTP: Lic. Sergio Daniel Caballero - sergiodcaballero@gmail.com
- Ayudante 1º : Mgter. Martin Rey  - mrey00@gmail.com
- Ayudante 2º : Lic. Facundo Yatchesen - facundoyatchesen@gmail.com
- Adscripto Graduado : ASC. Baby John Charles - johnbabi.jb@gmail.com
- Adscripto Graduado: ASC. Lacheski Martin -martinlacheski@gmail.com

**Alumno:** Zakowicz Osvaldo Emanuel.

**Carreras:** Analista en Sistemas de Computación, Licenciatura en Sistemas de Información.

**Proyecto:** SiGAU - Sistema de gestión de albergues universitarios.

**Metodología:** UP, Unified Process.

**Año:** 2022.

---

## Indice de contenidos

1. Modelado del Negocio.

    1. [Descripción del Escenario](#descripción-del-escenario)

2. Requerimientos.

    1. [Entrevistas y Cuestionarios](#entrevistas-y-cuestionarios)

    2. [Requerimientos](#requerimientos)

3. Análisis del Dominio.

    1. [Diagrama de Casos de Uso](#diagrama-de-casos-de-uso)

    2. [Escenarios de Casos de Uso](#escenarios-de-casos-de-uso)

---

## Descripción del Escenario

volver al [Indice](#indice-de-contenidos)

Los albergues universitarios son un conjunto de casas destinadas a estudiantes de las carreras de la Universidad Nacional de Misiones, otorgadas como una beca. En la ciudad de Apóstoles está actualmente en funcionamiento un albergue para estudiantes de las carreras del Módulo de Informática de la FCEQyN. La “beca de albergue” es solicitada cada año a través de un formulario de google que registra las solicitudes en una planilla de cálculos, este formulario de solicitud está abierto un periodo de tiempo, al cerrar, el secretario de bienestar estudiantil revisa una a una cada petición, tomando en cuenta ciertas características primordiales de preseleccion de solicitudes, estas características son: distancia entre la localidad de origen del solicitante y las carreras informáticas, la situación socio-económica familiar (ganancias totales de la familia, el numero de integrantes de la familia y cuantos de ellos estudian), entre otros parámetros, (se da prioridad para la preseleccion a las peticiones en las que el interesado vive lejos de la ciudad de apóstoles y su familia tiene ganancias bajas); Además, el secretario de bienestar estudiantil debe separar las solicitudes nuevas de aquellas que son realizadas por alumnos anteriormente becados que desean renovar el beneficio, para estos últimos un requisito adicional es aprobar un mínimo de 2 materias del último año cursado. Finalmente el secretario de bienestar estudiantil comparte el acceso a la planilla de cálculos con las pre-selecciones al encargado de albergues, y además le envía un listado impreso de preseleccionados.

Los albergues universitarios tienen un encargado de albergue, su trabajo es analizar las solicitudes de beca preseleccionadas, las situaciones académicas de los solicitantes nuevos (si corresponde) o avanzados (solicitantes avanzados son los estudiantes con uno o mas años de uso de la beca.), y luego otorgar la beca teniendo en cuenta que solo se pueden emitir cierto numero de becas correspondiente a las plazas libres en cada casa. Otras responsabilidades del encargado de albergue son informar del reglamento de los albergues, de actuar según el incumplimiento de dichas normas y mediar en problemas de convivencia entre becados y en su solución. También se encarga de recopilar inconvenientes de mantenimiento en los albergues y planificar su reparación, planificar además las jornadas de limpieza y mantenimiento general de los albergues (la limpieza específica de cada casa es coordinada entre un delegado y los becados de la misa, se describirá mas adelante). El encargado de albergue también mantiene un registro de cada casa, y por cada casa el registro de las habitaciones, camas, colchones, muebles y electrodomésticos disponibles que son propiedad de los albergues.

Cada casa tiene un conjunto de habitaciones, 4 en total son destinadas para becados, cuenta con 1 baño instalado, y 1 cocina comedor, además de patio frontal y patio trasero. Cada habitación es estrictamente compartida por 2 becados, en las habitaciones mas pequeñas, y hasta 4 becados en la habitación mas grande, siendo hasta 10 el máximo de alumnos becados por casa. El total de 5 casas que forman parte del albergue universitario tienen exactamente el mismo diseño estructural, y están equipadas con muebles y electrodomésticos, y además con los servicios esenciales de luz y agua. De las 5 casas, 1 de ellas está destinada a becados femeninas, y las restantes 4 a becados masculinos.

Para acceder a la beca por primera vez, un Estudiante debe realizar una solicitud a la secretaria de bienestar estudiantil a través de un formulario de google, informando sus datos personales, datos de su padre, madre, cantidad de integrantes de la familia, ingresos familiares, cantidad de integrantes de la familia que están estudiando, domicilio actual (se considera la distancia desde su domicilio hasta la ciudad de apóstoles como un factor en el análisis de la solicitud, junto a la situación económica de la familia) entre otros datos y subir documentación que respalde los datos declarados. Posteriormente para renovar la beca, cada becado debe, además de mantener sus datos actualizados, aprobar por promoción o examen final un mínimo de 2 materias de una misma carrera cada año. En caso de que el becado no cumpla en su totalidad los requisitos académicos para renovar la beca (por ejemplo, tenga aprobadas 1 de 2 materias necesarias), puede tratar alternativas para aprobar materias faltantes (en mesas de examen) con el encargado de albergue, el cual también considerará el problema por el cual no se cumplió el requisito, y considerará el nivel de convivencia del becado en años anteriores como un factor a tener en cuenta para acordar una alternativa (un ejemplo de alternativa es establecer un plazo hasta próximas mesas de examen para que el becado apruebe y cumpla el requisito académico). En caso de que el becado no cumpla requisitos académicos, no tenga un historial de buena convivencia y no pueda aprobar materias faltantes incluso habiéndose considerado la alternativa de ejemplo anterior, se procederá al cese de la beca, aviso al becado y posterior solicitud de desalojo de su lugar en la casa que tenga designada, pudiendo el becado llevarse consigo solamente los bienes que trajo en un principio y aquellos que pueda demostrar que son suyos. Otro caso particular de cese de beca es ante una falta grave del reglamento de albergues.

Cada casa tiene un becado avanzado (mínimamente lleva un año como becado) que ejerce un papel de “delegado”, este papel es para la organización de cada casa y no es un puesto oficial, el delegado se encarga de coordinar las actividades de limpieza de la casa, guiando a los demás estudiantes nuevos las primeras semanas en la realización de cada tarea, estableciendo junto a ellos un cronograma de limpieza, la división del costo total de servicios de luz, agua e Internet (en caso de que la casa cuente con una conexión particular de Internet), recaudando el dinero del pago y realizando el pago de los servicios, poniendo a buen recaudo los comprobantes de pago.

Cada becado tiene que cumplir con las normas de convivencia y el reglamento de los albergues universitarios, y además, estar dispuesto a prestar ayuda en la limpieza y mantenimiento básico de los albergues (limpieza de la casa, asistir en jornadas de limpieza general, asistir a días previamente designados para pintar las casas, colaborar con el mantenimiento de los patios) aunque no es obligatorio, finalmente, aunque la beca de albergue es gratuita, el pago de servicios de luz y agua es dividido por el numero de integrantes de cada casa y esto también aplica a servicios terceros no incluidos, como por ejemplo el contrato particular de Internet por parte de algún miembro de la casa.

Cada casa cuenta con muebles y electrodomésticos propiedad de la universidad que pueden ser utilizados pero no sustraídos de las mismas bajo ningún concepto. Cada becado puede llevar efectos personales, equipaje, muebles tales como estantes, escritorios, electrodomésticos, etc. Sin embargo, bienes tales como heladeras, cocinas a gas, hornos eléctricos, cafeteras eléctricas u otros que se dispongan en la cocina comedor deben ser de uso compartido por todos los integrantes de la casa, teniendo conocimiento de esto el alumno becado dueño del bien y estando bajo toda la casa de becados la responsabilidad del uso y cuidado del mismo. Cuando un becado lleva muebles o electrodomésticos a la casa en la que vivirá, el encargado de albergue toma los datos de los bienes y los registra a nombre del becado, siendo estos bienes de propiedad del becado.

volver al [principio](#descripción-del-escenario)

## Entrevistas y Cuestionarios

volver al [Indice](#indice-de-contenidos)

Acontinuación se incluye un enlce a las respuestas de las entrevistas realizadas al secretario de bienestar estudiantil y al encargado del albergue.

- **Ver [entrevistas](entrevistas.md).**

## Requerimientos

volver al [Indice](#indice-de-contenidos)

### Definición de requerimientos del usuario

|  **Requerimientos del usuario** |
|:--------------------------------|
|1. SiGAU controlará las solicitudes de estudiantes para la beca de albergue, los datos y documentos que se deben adjuntar y la preselección de solicitudes.|
|2. SiGAU mantendrá registrada cada casa de la beca, cada becado y lugares libres en cada casa.|
|3. SiGAU se encargará de planificar la limpieza de cada casa de la beca para cada becado.|
|4. SiGAU se encargará de mantener seguimiento sobre el pago de servicios domesticos de cada casa de la beca, resguardando las boletas y comprobantes de pago.|
|5. SiGAU permitirá registrar solicitudes de mantenimiento, y planificar jornadas de mantenimiento en las casas de la beca.|
|6. SiGAU mantendra un sistema de puntajes para cada becado según estos cumplan sus tareas de limpieza y de pago de cuentas a tiempo y en forma, luego usará el puntaje de cada becado para darle un beneficio o asignarle una sancion.|
|7. SiGAU mantendrá perfiles de usuario, para un administrador general, un auditor, el secretario de bienestar estudiantil, el encargado de albergues, estudiantes y becados, cada perfil tendrá cierto nivel de permisos y acceso a ciertas partes del sistema.|
|8. SiGAU tiene que ser facil de usar, con ventanas, texto y botones simples, y legible, también debe tener algún manual o guia de uso.|
|9. SiGAU debe emitir reportes sobre los becados, solicitudes de beca, casas, el mantenimiento y el nivel de limpeza.|

### Especificación de los requerimientos del sistema

|  **Requerimientos del sistema, apartado 1.** |
|:---------------------------------------------|
|1.1 SiGAU Proporcionará un registro para usuarios estudiantes.|
|1.2 SiGAU Proporcionará un formulario de solicitud para los estudiantes registrados que tomará todos los datos de solicitud personales, académicos, socioeconómicos, familiares  y permitirá subir archivos en formato PDF, imagen o documento de texto.|
|1.3 SiGAU Encriptará los datos personales y documentacion de cada estudiante en la base de datos.|
|1.4 SiGAU Realizará una preselección de solicitudes de beca según parámetros de selección preestablecidos cuando el período de solicitud finalice.|
|1.5 SiGAU no debe permitir que se realice una solicitud hasta que se adjunten los documentos requeridos en cada apartado del formulario de solicitud en el formato adecuado.|
|1.6 SiGAU debe permitir a un becado finalizar su beca, dandose de baja por si mismo cuando no quiera usar mas el albergue.|

| **Requerimientos del sistema, apartado 2.** |
|:--------------------------------------------|
|2.1 SiGAU permitirá registrar cada casa de la beca de albergue, el numero de habitaciones y de camas por habitación.|
|2.2 SiGAU permitirá registrar cada usuario que resulte beneficiado por la beca como un becado en una casa, asignándole habitación y cama.|
|2.3 SiGAU mantendrá un registro con los lugares libres de cada casa por habitación.|
|2.4 A medida que se ocupen o liberen espacios en los albegrues, SiGAU mantendrá actualizada la cantidad de lugares libres.|
|2.5 Si ya no existen lugares libres en una casa, SiGAU no debe permitir que se asigue una beca de albergue a un estudiante para dicha casa.|

| **Requerimientos del sistema, apartado 3** |
|:-------------------------------------------|
|3.1 SiGAU mantendrá un listado de áreas que deben ser mantenidas limpias para cada casa, su nivel de prioridad, y el plazo de planificación en que debe cumplirse cada tarea.|
|3.2 SiGAU planificará en un calendario para cada becado de cada casa una o mas tareas de limpieza que se deben completar en un tiempo (5, 7, 10 dias).|
|3.3 SiGAU permitira que cada becado registre la finalización de una tarea asignada y envié una o mas imagenes (fotos) del área o áreas que limpió para que sea calificada por los demás integrantes de la casa  (calificación del 1 "mal" al 10 "perfecto").|
|3.4 SiGAU replanificará las tareas asignadas en un período de tiempo cuando se incluya un nuevo becado en una casa o cuando se quite un becado de una casa.|
|3.5 En caso de que no se estén cumpliendo las tareas en tiempo y forma, SiGAU propondrá resolver tareas por equipos o en otros horarios diferentes.|

| **Requerimientos del sistema, apartado 4** |
|:-------------------------------------------|
|4.1 SiGAU planificará en un calendario para cada casa el período en el que se espera paguen los servicios de luz y agua, este período de timpo va desde el inicio del mes hasta un tiempo aproximado en que llegan las boletas (1 al 15 de cada mes).|
|4.2 Por cada servicio, SiGAU esperará a que al final del período se suban los datos de identificación de la boleta de servicio pagada, para que la planificación del mes se considere cumplida. SiGAU no debe permitir que una planificación de pago se omita al no subir las boletas pagadas.|
|4.3 SiGAU no debe permitir que se suban boletas ya registradas, o en un formato inadecuado.|

| **Requerimientos del sistema, apartado 5** |
|:-------------------------------------------|
|5.1 SiGAU permitirá que cada becado pueda realizar una solicitud de mantenimiento sobre algún área en presunto desperfecto en la casa donde habita.|
|5.2 Por cada solicitud de mantenimiento, SiGAU establecerá un trabajo pendiente a resolver, marcándo esta solicitud como abierta.|
|5.3 SiGAU permitirá que cada solicitud de mantenimiento pueda luego establecerse como cerrada por el solicitante o el encargado de albergues cuando se encuentre cumplida.|
|5.4 SiGAU permitirá que el encargado de albergue planifique jornadas de mantenimiento e incluya en ellas solicitudes de mantenimiento a resolver, luego informará de esto a todos los becados.|
|5.5 En caso de que una o mas solicitudes de mantenimiento no se puedan cumplir en la jornada, se moverán a la siguiente jornada que se planifique.|

| **Requerimientos del sistema, apartado 6** |
|:-------------------------------------------|
|6.1 SiGAU mantendrá un sistema de puntajes y beneficios para cada becado con el objetivo de motivar a la realización de la limpieza y pago de servicios en tiempo y forma.|
|6.2 Por cada tarea que se cumpla en tiempo y se califique por los demás becados de una casa y por el pago a tiempo de los servicios se influirá de forma positiva o negativa en el puntaje del becado responsable de la tarea, de la siguiente forma:|
|6.2.1 Un becado con un periodo de tiempo de buen puntaje llegando a un determinado nivel será bonificado estando libre de tareas en la siguiente planificación de limpieza, esto es obtenible una sola vez, luego debe mantener buen puntaje hasta poder calificar nuevamente. Si ademas es delegado de la casa, al llegar a un buen nivel de puntaje 3 veces seguidas obtendrá un beneficio exclusivo para elegir una planificación en la que no quiere estar (puede elegir en que planificación estar libre).|
|6.2.2 Un becado con un nivel de mal puntaje será planificado con una tarea extra de limpieza (de entre varias tareas extra a las planificadas normalmente), al completar ambas tareas bien calificadas puede mejorar su puntaje general. Si además es delegado de la casa, al llegar a un mal nivel 3 veces, el sistema tomará el siguiente candidato con mayor puntaje para proponerle ser delegado. Puede rechazar ser delegado, el sistema tomará el siguiente becado con mejor puntaje y le hará la misma propuesta.|
|6.2.3 Si todos los becados tienen buen nivel en puntaje, se descontará una tarea poco critica. de la planificación de limpieza y cada uno de ellos tendrá una semana libre.|

| **Requerimientos del sistema, apartado 7** |
|:-------------------------------------------|
|7.1 Para el perfil de administrador, SiGAU tendrá todos sus modulos y apartados visibles y configurables. Excepto el apartado de Auditoría.|
|7.2 El perfil de Auditor solo podrá acceder al apartado de auditoria.|
|7.3 El perfil del secretario de bienestar estudiantil tendrá acceso a el módulo de beca, casa y becados.|
|7.4 El perfil del encargado de albergues tendrá acceso a los modulos de beca, casa, becados, mantenimiento y planificaciones|
|7.5 El perfil de estudiante tendrá acceso a la solictud de la beca, y el perfil de becado a su cuenta personal.|
|7.6 SiGAU no debe permitir el acceso de un perfil a un apartado que no le corresponde.|

| **Requerimientos del sistema, apartado 8** |
|:-------------------------------------------|
|8.1 El sistema se desarrollará con un buen tamaño de letra y equilibrado contraste en los colores de las ventanas, texto y botones.|
|8.2 Se proporcionará un manual de usuario del sistema|

| **Requerimientos del sistema, apartado 9** |
|:-------------------------------------------|
|9.1 El sistema proporcionará reportes de cada módulo con la posibilidad de elegir parámetros para el mismo, en formato PDF.|

volver al [principio](#requerimientos)

## Diagrama de Casos de Uso

## Escenarios de Casos de Uso

volver al [Indice](#indice-de-contenidos)

### Caso de Uso: Solicitar Beca

|**Nombre del Caso de Uso:** Solicitar Beca.|
|:---|
|**Actor(es):** Estudiante.|
|**Descripcion:** Permitir que un Estudiante complete el formulario de solicitud de beca y lo envíe.|
|**Evento desencadenador:** El estudiante accede al apartado de solicitud de beca.|
|**Flujo tipico de eventos (ruta principal):**|
|1.*Este caso de uso incia cuando el estudiante accede al apartado de solicitud de beca.*|
|2.*El sistema muestra el formulario de solicitud a completar, separado por secciones.*|
|3.*El estudiante completa los datos obligatorios por cada sección y adjunta la documentación necesaria en los apartados que así lo requieren, y confirma la solicitud de beca.*|
|4.*El sistema verifica los campos obligatorios de cada apartado y el formato de la documentación adjuntada y a continuación envia el formulario.*|
|5.*El sistema guarda una solicitud de beca, encriptando los datos de la misma, retorna un mensaje de solicitud de beca exitosa al estudiante, y finaliza el caso de uso.*|
|**Flujo alternativo de eventos:**|
|4.*El sistema indica al estudiante que faltan completarse datos obligatorios y/o el formato de la documentación no es válido, retornando al punto 3 del flujo tipico de eventos.*|
|**Precondición:** El estudiante ya se registró en el sistema, y accedió a su cuenta.|
|**Postcondición:** El estudiante solicitó con éxito la beca de albergue.|
|**Requerimientos cumplidos:** *Requerimientos del sistema, apartado 1, item 1.1 SiGAU proporcionará un formulario de solicitud de beca., item 1.3 SiGAU encriptará los datos de cada solicitud de estudiante, item 1.5 SiGAU no debe permitir que se registre una solicitud sin documentacion adjunta.* |

### Caso de Uso: Renovar Beca

|**Nombre del Caso de Uso:** Renovar Beca.|
|:---|
|**Actor(es):** Becado|
|**Descripcion:** Permitir que un becado renueve su beca de albergue realizando una solicitud.|
|**Evento desencadenador:** El becado accede al apartado de solicitud de beca, para su renovación.|
|**Flujo tipico de eventos (ruta principal):**|
|1.*Este caso de uso incia cuando el becado accede al apartado de solicitud de beca, para su renovación.*|
|2.*El sistema retorna todos los datos del becado para su revisión, solicita se completen datos académicos del ultimo año y adicionalmente solicita se adjunte una historia académica actualizada en formato PDF.*|
|3.*El becado revisa sus datos, completa sus datos académicos y adjunta una historia académica, a continuación confirma la solicitud de renovación de la beca.*|
|4.*El sistema verifica los campos obligatorios de cada apartado y el formato de la documentación adjuntada y a continuación envia el formulario.*|
|5.*El sistema una solicitud de renovacion de beca, encriptando los datos de la misma, retorna un mensaje de solicitud de beca exitosa al estudiante, y finaliza el caso de uso.*|
|**Flujo alternativo de eventos:**|
|4.*El sistema indica al estudiante que faltan completarse datos obligatorios y/o el formato de la documentación no es válido, retornando al punto 3 del flujo tipico de eventos.*|
|**Precondición:** El becado accedió a su cuenta correctamente.|
|**Postcondición:** El becado solicitó con éxito la renovación de la beca de albergue.|
|**Requerimientos cumplidos:** *Requerimientos del sistema, apartado 1, item 1.1 SiGAU proporcionará un formulario de solicitud de beca., item 1.3 SiGAU encriptará los datos de cada solicitud de estudiante, item 1.5 SiGAU no debe permitir que se registre una solicitud sin documentacion adjunta.*|

### Caso de Uso: Finalizar tarea de limpieza

|**Nombre del Caso de Uso:** Finalizar tarea de limpieza.|
|:---|
|**Actor(es):** Becado.|
|**Descripcion:** Permitir al becado indicar que ha finalizado la tarea de limpieza que le fue asignada registrando la finalización de la misma.|
|**Evento desencadenador:** El becado selecciona la tarea que le fue asignada para indicar su finalización.|
|**Flujo tipico de eventos (ruta principal):**|
|1.*Este caso de uso incia cuando el becado accede al apartado de tareas de su casa y selecciona una tarea que le fue asignada para finalizarla.*|
|2.*El sistema retorna un formulario de finalización de tarea con campos a completar y un campo para subir imágenes.*|
|3.*El becado completa el formulario y adjunta imágenes del área limpia correspondiente a la tarea de limpieza asignada, y lo envía.*|
|4.*El sistema valida los campos obligatorios del formulario.*|
|5.*El sistema establece la tarea asignada como realizada y lista para ser calificada, a continuación retorna un mensaje de tarea realizada al becado, y finaliza el caso de uso.*|
|**Flujo alternativo de eventos:**|
|4.*El sistema indica al becado que faltan completarse datos obligatorios, retornando al punto 3 del flujo tipico de eventos.*|
|**Precondición:** El becado accedió a su cuenta correctamente y tiene al menos una tarea de limpieza asignada que debe finalizar.|
|**Postcondición:** El becado registró la finalización de una tarea de limpieza con éxito.|
|**Requerimientos cumplidos:** *Requerimientos del sistema, apartado 3, item 3.3 SiGAU permitira que cada becado registre la finalización de una tarea asignada y envié una o mas imagenes (fotos) del área o áreas que limpió para que sea calificada por los demás integrantes de la casa*.|

### Caso de Uso: Calificar tarea de limpieza

|**Nombre del Caso de Uso:** Calificar tarea de limpieza.|
|:---|
|**Actor(es):** Becado.|
|**Descripcion:** Permitir a un becado, por cada tarea asignada a sus cmpañeros de casa, calificar una tarea de limpieza realizada con un puntaje del 1 al 10.|
|**Evento desencadenador:** El becado accede al apartado de tareas de la casa completadas y pendientes de calificación.|
|**Flujo tipico de eventos (ruta principal):**|
|1.*Este caso de uso incia cuando el becado accede al apartado de tareas de la casa que están pendientes de calificación.*|
|2.*El sistema retorna todas las tareas realizadas desde la vigencia de la planificación hasta la fecha actual.*|
|3.*El becado selecciona una tarea para su visualización*|
|4.*El sistema retorna la tarea con las imágenes que tiene asociada para su visualización, y un formulario con una escala de calificación*|
|5.*El becado carga la calificación que dará en la escala y a continuación califica la tarea.*|
|6.*El sistema verifica que se haya proporcionado una calificación a la tarea y a continuación envía el formulario.*|
|7.*El sistema guarda la calificación de un becado para una tarea de la casa finalizada, a continuación retorna un mensaje de tarea calificada, y finaliza el caso de uso.*|
|**Flujo alternativo de eventos:**|
|2.*El sistema retorna un mensaje indicando que aún no hay tareas finalizadas de la planificación actual para ser calificadas, y finaliza el caso de uso.*|
|6.*El sistema indica que es ncesario proporcionar una calificación para poder continuar, retornando al punto 4 del flujo tipico de eventos.*|
|**Precondición:** El sistema cuenta con al menos una tarea del período de planificación actual pendiente de calificación.|
|**Postcondición:** El becado calificó una tarea realizada con un puntaje de 1 a 10.|
|**Requerimientos cumplidos:** *Requerimientos del sistema, apartado 3, item 3.3 SiGAU permitira que cada becado registre la finalización de una tarea asignada y envié una o mas imagenes (fotos) del área o áreas que limpió para que sea calificada por los demás integrantes de la casa  (calificación del 1 "mal" al 10 "perfecto").* En este caso, se permitirá a cada becado calificar las tareas asignadas a sus compañeros de casa.|

### Caso de Uso: Finalizar beca

|**Nombre del Caso de Uso:** Finalizar Beca.|
|:---|
|**Actor(es):** Becado.|
|**Descripcion:** Permitir a un becado darse de baja de la beca de albergue.|
|**Evento desencadenador:** El becado accede a su cuenta y entra a la opción de finalización de beca.|
|**Flujo tipico de eventos (ruta principal):**|
|1.*Este caso de uso incia cuando el becado accede al apartado de finalización de beca.*|
|2.*El sistema despliega un formulario de finalización de beca que debe ser completado.*
|3.*El becado completa el formulario de baja de la beca y a continuación confirma su envío.*|
|4.*El sistema despliega un aviso informando sobre la acción a punto de realizarse y pidiendo confirmación solicitando que el becado ingrese su contraseña y confirme los terminos y condiciones de darse de baja de la beca*|
|5.*El becado proporciona su contraseña y confirma los terminos y condiciones.*|
|6.*El sistema verifica que se hayan completado los campos obligatorios y a continuación envía el formulario.*|
|7.*El sistema realiza la baja de la beca, indicando al becado y al encargado de albergue que debe realizarse un posterior desalojo de una casa, iniciando un desalojo, replanifica la limpieza de cada casa para los becados aún presentes. Finalmente, retorna un mensaje al becado de que se realizó su baja de la beca con éxito.*|
|**Flujo alternativo de eventos:**|
|5.*El becado cancela la operación de baja de la beca, y finaliza el caso de uso.*|
|6.*El sistema indica al becado que faltan completarse datos obligatorios, retornando al punto 2 del flujo tipico de eventos.*|
|**Precondición:** El becado accedió a su cuenta correctamente.|
|**Postcondición:** El becado realizó la baja de su beca de albergue con éxito.|
|**Requerimientos cumplidos:** Requerimientos del sistema, apartado 1, item 1.6 SiGAU debe permitir a un becado finalizar su beca, dandose de baja por si mismo cuando no quiera usar mas el albergue.|

### Caso de Uso: Retirar bienes

|**Nombre del Caso de Uso:** Retirar bienes|
|:---|
|**Actor(es):** Becado|
|**Descripcion:** Permitir a un becado retirar los bienes que ingreso al albergue, tales como muebles o electrodomésticos.|
|**Evento desencadenador:** El becado accede a su cuenta y al apartado de sus bienes para retirarlos.|
|**Flujo tipico de eventos (ruta principal):**|
|1.*Este caso de uso incia cuando el becado accede a su cuenta y al apartado de bienes para retirarlos.*|
|2.*El sistema retorna una lista de bienes que tiene el becado en la casa asignada.*|
|3.*El becado selecciona un bien para retirarlo.*|
|4.*El sistema sistema muestra el bien a retirar.*|
|5.*El becado confirma que retirará el bien de la casa*|
|6.*El sistema marca el bien como retirado de la casa, a continuación informa al becado del retiro exitoso del bien, y notifica al delegado sobre el bien retirado.*|
|**Flujo alternativo de eventos:**|
|2.*El sistema indica que el becado no tiene ningun bien en la casa a retirar, y finaliza el caso de uso.*|
|**Precondición:** El becado tiene al menos un bien en la casa asignada.|
|**Postcondición:** El becado retiró un bien de la casa asignada, informando de esto al encargado de albergues.|
|**Requerimientos cumplidos:** requerimientos|

### Caso de Uso: Registrar pedido de mantenimiento

|**Nombre del Caso de Uso:** Registrar pedido de mantenimiento.|
|:---|
|**Actor(es):** Becado, Encargado de albergue.|
|**Descripcion:** Permitir a cada actor registrar un pedido de mantenimiento sobre un área, electrodoméstico o mueble de una casa.|
|**Evento desencadenador:** El actor accede al apartado de mantenimiento para registrar un pedido de mantenimiento.|
|**Flujo tipico de eventos (ruta principal):**|
|1.*Este caso de uso incia cuando el actor accede al apartado de mantenimiento y a registrar un pedido de mantenimiento.*|
|2.*El sistema despliega un formulario de pedido de mantenimiento a completar para la casa en la que está el actor si es becado. O si es el encargado de albergue, para cualquier casa.*|
|3.*El actor completa el formulario de solicitud de mantenimiento para un área de una casa en concreto*|
|4.*El sistema verifica que se hayan completado los datos obligatorios y que no exista una solicitud previa sobre la misma área que esté pendiente de resolverse. A continuación envía el formulario.*|
|5.*El sistema establece un pedido de mantenimiento para un área de una casa.*|
|**Flujo alternativo de eventos:**|
|4.*El sistema indica al actor que faltan completarse datos obligatorios, retornando al punto 2 del flujo tipico de eventos.*|
|4.*El sistema indica que ya existe un pedido de mantenimiento pendiente para la misma área de la casa, retornando al punto 2 del flujo tipico de eventos.*|
|**Precondición:** El actor ingreso a su cuenta correctamente, el área de una casa para la cual se establecerá el pedido de mantenimiento no tiene otro pedido previo pendiente.|
|**Postcondición:** El actor registró con éxito un pedido de mantenimiento de un área de una casa en concreto.|
|**Requerimientos cumplidos:** requerimientos|

### Caso de Uso: Registrar pago de servicio

|**Nombre del Caso de Uso:** Registrar pago de servicio.|
|:---|
|**Actor(es):** Delegado|
|**Descripcion:** Permitir al delegado de la casa registrar que ha pagado un servicio doméstico (luz, agua) registrando la boleta de servicio pagada.|
|**Evento desencadenador:** El delegado ingresa al apartado de servicios de la casa para ingresar un nuevo registro de pago.|
|**Flujo tipico de eventos (ruta principal):**|
|1.*Este caso de uso incia cuando el delegado accede al apartado de servicios de la casa para ingresar un nuevo registro de pago.*|
|2.*El sistema retorna los servicios de cada mes que aún no han sido registrados*|
|3.*El delegado selecciona el servicio del mes que desea registrar como pagado.*|
|4.*El sistema retorna un formulario a completar con datos de la boleta de servicio pagada, y un espacio para subir una copia digitalizada de la boleta pagada y el comprobante de pago.*|
|5.*El delegado completa el formulario y adjunta la boleta y comprobante de pago.*|
|6.*El sistema verifica que se han completado los datos obligatorios y que los datos no sean de una boleta ya registrada con anterioridad, a continuación envía el formulario.*|
|7.*El sistema registra un pago de servicio para un mes específico, retorna un mensaje de registro exitoso al delegado, a continuación finaliza el caso de uso.*|
|**Flujo alternativo de eventos:**|
|6.*El sistema detecta que se han enviado datos de una boleta ya registrada como pagada con anterioriad en otro mes, o que faltan datos obligatorios por completarse, o el formato de la documentación adjunta no es el indicado, retornando al punto 4 del flujo tipico de eventos.*|
|**Precondición:** El delegado ingresó a su cuenta correctamente, existe al menos un servicio pendiente de pago.|
|**Postcondición:** El delegado registró con éxito el pago ya realizado de un servicio doméstico.|
|**Requerimientos cumplidos:** |

### Caso de Uso: Configurar período de solicitud

|**Nombre del Caso de Uso:** Abrir período de solicitud.|
|:---|
|**Actor(es):** Secretario de bienestar estudiantil.|
|**Descripcion:** Permitir al secretario de bienestar estudiantil configurar el inicio del período de solicitud de becas de albergue y establecer la duración del mismo hasta su cierre.|
|**Evento desencadenador:** El secretario de bienestar estudiantil accede al apartado de beca para configurar un nuevo periodo de solicitud.|
|**Flujo tipico de eventos (ruta principal):**|
|1.*Este caso de uso incia cuando el secretario de bienestar estudiantil accede al apartado de beca para configurar un nuevo periodo de solicitud.*|
|2.*El sistema retorna un formulario de configuración para el nuevo período de solicitud, con fechas de inicio y fin del período, y el comportamiento del sistema al cerrar el período.*|
|3.*El secretario de bienestar estudiantil establece las fechas de inicio y fin del período, si desea que el sistema preseleccione solicitudes o no al cerrarse.*|
|4.*El sistema muestra el total de dias que estará disponible el período de solicitud y adicionalmente mostrará una opcion para guardar la configuración como predeterminada si no hay configuraciones guardadas o si desea sobreescribir una configuración anterior*|
|5.*El secretario de bienestar estudiantil confirma la apertura del período segun las configuraciones enviando el formulario de configuración.*|
|6.*El sistema verifica que se han completado todos los campos obligatorios, a continuación configura la apertura y cierre de la solicitud de beca, retornando un mensaje de éxito al secretario de bienestar estudiantil, y finaliza el caso de uso.*|
|**Flujo alternativo de eventos:**|
|6.*El sistema indica al secretario de bienestar estudiantil que faltan completarse datos obligatorios, retornando al punto 2 del flujo tipico de eventos.*|
|**Precondición:** El secretario de bienestar estudiantil ingresó a su cuenta correctamente, no existe un período de solicitud de beca abierto con anterioridad que aún no ha cerrado.|
|**Postcondición:** El secretario de bienestar estudiantil configuró el período de solicitud para su apertura.|
|**Requerimientos cumplidos:** requerimientos|

### Caso de Uso: Configurar preseleccion de solicitudes

|**Nombre del Caso de Uso:** Configurar preseleccion de solicitudes.|
|:---|
|**Actor(es):** Secretario de bienestar estudiantil.|
|**Descripcion:** Permitir al secretario de bienestar estudiantil configurar parámetros de preselección de solicitudes que el sistema usará luego del cierre del período de solicitudes para preseleccionar las mismas.|
|**Evento desencadenador:** El secretario de bienestar estudiantil accede al apartado de configuración de preselección de solicitudes.|
|**Flujo tipico de eventos (ruta principal):**|
|1.*Este caso de uso incia cuando el secretario de bienestar estudiantil accede al apartado de configuración de preselección de solicitudes.*|
|2.*El sistema muestra en un formulario un listado de parámetros de preselección a configurar.*|
|3.*El secretario de bienestar estudiantil establece los parámetros de preselección, y a continuación envía el formulario.*|
|4.*El sistema verifica que se han proporcionado todos los datos obligatorios del formulario, a continuación guarda las nuevas configuraciones.*|
|5.*El sistema retorna un mensaje de éxito en la configuración y finaliza el caso de uso.*|
|**Flujo alternativo de eventos:**|
|4.*El sistema indica al secretario de bienestar estudiantil que faltan completarse datos obligatorios, retornando al punto 2 del flujo tipico de eventos*|
|**Precondición:** El scretario de bienestar estudiantil ingresó a su cuenta correctamente.|
|**Postcondición:** El secretario de bienestar estudiantil configuró los parámetros de preselección de solicitudes del sistema.|
|**Requerimientos cumplidos:** requerimientos|

### Caso de Uso: Verificar documentacion

|**Nombre del Caso de Uso:** Verificar documentacion.|
|:---|
|**Actor(es):** Secretario de bienestar estudiantil.|
|**Descripcion:** Permitir al secretario de bienestar estudiantil verificar la documentación de una solicitud de beca.|
|**Evento desencadenador:** El secretario de bienestar estudiantil selcciona una solicitud de beca para su análisis.|
|**Flujo tipico de eventos (ruta principal):**|
|1.*Este caso de uso incia cuando el secretario de bienestar estudiantil selecciona una solicitud para su análisis.*|
|2.*El sistema retorna los datos de la solicitud y la documentación asociada para su visualización*|
|3.*Por cada documento visualizado, el secretario de bienestar estudiantil puede marcarlo como aceptado o no y adicionalmente, en caso de que no se acepte el documento, comentando el motivo. Al finalizar, cierra la verificación.*|
|4.*El sistema analiza la solicitud, si toda la documentación fue aceptada, la misma se marca como "documentacion verificada", y finaliza el caso de uso.*|
|**Flujo alternativo de eventos:**|
|4.*El sistema analiza la solicitud, si existe documentación rechazada solicitar un reenvío de documentación, indicando el motivo de cada documento rechazado y dando una fecha límite de reenvío, y finaliza el caso de uso.*|
|**Precondición:** El secretario de bienestar estudiantil ingresó correctamente a su cuenta.|
|**Postcondición:** El secretario de bienestar estudiantil verificó con éxito la documentación asociada a una solicitud.|
|**Requerimientos cumplidos:** requerimientos|

### Caso de Uso: Finalizar análisis de solicitudes

|**Nombre del Caso de Uso:** Finalizar análisis de solicitudes|
|:---|
|**Actor(es):** Secretario de bienestar estudiantil.|
|**Descripcion:** Permitir al secretario de bienestar estudiantil finalizar el análisis de solicitudes realizando una preselccion de las mismas.|
|**Evento desencadenador:** El secretario de bienestar estdiantil accede al apartado de beca y finaliza el análisis de solicitudes|
|**Flujo tipico de eventos (ruta principal):**|
|1.*Este caso de uso inicia cuando el secretario de bienestar estdiantil accede al apartado de beca y finaliza el análisis de solicitudes*|
|2.*El sistema verifica que todas las solicitudes tengan su documentación verificada y todos los pedidos de reenvío hayan vencido, a continuación realiza una preselección de solicitudes y retorna los preseleccionados*|
|3.*El secretario de bienestar estudiantil confirma la preselección de solicitudes.*|
|4.*El sistema hace efectiva la preselección de solicitudes, ordenando las solicitudes preseleccionadas en orden de prioridad según sus parámetros, a continuación hace visibles los preseleccionados para el encargado de albergues, y finaliza el caso de uso.*|
|**Flujo alternativo de eventos:**|
|2.*El sistema indica al secretario de bienestar estudiantil que existen solicitudes cuya documentación no ha sido verificada, y finaliza el caso de uso.*|
|2.*El sistema indica al secretario de bienestar estudiantil que existen solicitudes cuyo período para reenviar documentación no ha finalizado, y finaliza el caso de uso.*|
|**Precondición:** El secretario de bienestar estudiantil ingresó correctamente a su cuenta, y todas las solicitudes tienen la documentación verificada y/o reenviada.|
|**Postcondición:** El secretario de binestar estudiantil fnalizó el análisis de solicitudes con una preselección de las mismas.|
|**Requerimientos cumplidos:** requerimientos|

### Caso de Uso: Otorgar beca

|**Nombre del Caso de Uso:** Otorgar beca.|
|:---|
|**Actor(es):** Encargado de albergue.|
|**Descripcion:** Permitir al encargado de albergue visualizar una solicitud de beca preseleccionada para otorgarle la beca.|
|**Evento desencadenador:** El encargado de albergue accede a la sección de beca, al apartado de preseleccionados, y selecciona una solicitud para visualizarla.|
|**Flujo tipico de eventos (ruta principal):**|
|1.*Este caso de uso incia cuando el encargado de albergue accede a la sección de beca, al apartado de preseleccionados, selecciona una solicitud para visualizarla.*|
|2.*El sistema retorna los datos de la solicitud, si es una solicitud nueva o una renovación de beca y la documentación adjunta.*|
|3. *El encargado de albergue comprueba el estado académico de la solicitud, si se trata de una renovación, para saber si cumple el requisito de renovación comprueba también la historia académica adjunta, de tratarse de una solicitud nueva, no existe requisito académico previo, si alguno de los casos es correcto, a continuación otorga la beca al estudiante.*|
|4. *El sistema despliega un formulario de beca, completa los datos del estudiante con los ya proporcionados en la solicitud y solicita se asigne una casa y una habitación al becado.*|
|5. *El encargado de albergue asigna una casa y habitación al becado.*|
|6. *El sistema verifica que se han proporcionado todos los datos obligatorios del formulario, a continuación, se otorga la beca a un estudiante asignándolo a una casa y habitación*|
|7. *El sistema retorna un mensaje indicando el éxito al becar al estudiante y el uso de un lugar disponible en los albergues universitarios, a continuación finaliza el caso de uso*|.
|**Flujo alternativo de eventos:**|
|3. *El encargado de albergue observa que la solicitud es de renovación y que no cumple el requisito mínimo académico, finaliza este caso de uso y continúa el caso de uso "Establecer plazo académico"*|
|4. *El sistema indica que ya no quedan lugares disponibles en la beca de albergue, y finaliza este caso de uso.*|
|6. *El sistema indica que faltan completarse datos obligatorios del formulario, retornando al punto 4 del flujo tipico de eventos.*|
|**Precondición:** El encargado de albergue accedió correctamente a su cuenta, ya está disponible el listado de preseleccionados, y existen aún lugares disponibles en la beca de albergue.|
|**Postcondición:** El encargado de albergué asignó una beca a un estudiante, incluyéndolo en una casa y una habitación, descontando de la beca un lugar.|
|**Requerimientos cumplidos:** requerimientos|

### Caso de Uso: Establecer plazo académico

|**Nombre del Caso de Uso:** Establecer plazo académico.|
|:---|
|**Actor(es):** Encargado de albergue.|
|**Descripcion:** Permitir al encargado de albergue establecer un plazo académico en el que un becado que esté renovando su beca debe previamente cumplir los requisitos académicos y presentar una história académica nueva.|
|**Evento desencadenador:** El encargado de albergue está visualizando una solicitud de renovación de beca y accede a establecer un plazo académico para la misma.|
|**Flujo tipico de eventos (ruta principal):**|
|1.*Este caso de uso incia cuando el encargado de albergue está visualizando una solicitud de renovación de beca y accede a establecer un plazo académico para la misma.*|
|2.*El sistema despliega un formulario para establecer un plazo académico solicitando la fecha del fin de plazo y la cantidad de materias que debe aprobar.*|
|3. *El encargado de albergues completa el formulario y a continuación confirma el plazo académico.*|
|4. *El sistema verifica que se han proporcionado todos los datos obligatorios del formulario. A continuación establece el plazo académico informando al becado que se le renueva la beca hasta que finalice el plazo, y para continuar becado debe aprobar las materias faltantes y presentar una nueva historia académica*|
|5. *El sistema retorna un mensaje de éxito al establecer un plazo académco, y a continuación finaliza el caso de uso.*|
|**Flujo alternativo de eventos:**|
|4.*El sistema indica que faltan completarse datos obligatorios del formulario, retornando al punto 2 del flujo tipico de eventos.*|
|**Precondición:** El encargado de albergues accedió correctamente a su cuenta.|
|**Postcondición:** El encargado de albergues estableció un plazo académico para un becado, renovando provisoriamente la beca hasta el fin del plazo.|
|**Requerimientos cumplidos:** requerimientos|

### Caso de Uso: Cambiar de casa

|**Nombre del Caso de Uso:** Cambiar de casa.|
|:---|
|**Actor(es):** Encargado de Albergue.|
|**Descripcion:** Permitir al encargado de albergue asignar otra casa y habitación a un becado, si hay lugares disponibles, o intercambiar dos becados de casa y habitación, o solo de habitación en la misma casa.|
|**Evento desencadenador:** El encargado de albergue accede al apartado de beca y al listado de becados, y selecciona uno para visualizarlo y cambiar de casa o habitación.|
|**Flujo tipico de eventos (ruta principal):**|
|1.*Este caso de uso incia cuando el encargado de albergue accede al apartado de beca y al listado de becados, y selecciona uno para visualizarlo y cambiar de casa o habitación*|
|2.*El sistema retorna un formulario de cambio de casa para el becado seleccionado, y a continuación solicita casa y lugar a asignar, o un becado con el que intercambiar lugar.*|
|3. *El encargado de albergue completa el formulario estableciendo el cambio de casa para el o los becados involucrados, o un cambio de habitacion en la misma casa*|
|4. *El sistema verifica que se han proporcionado todos los datos obligatorios del formulario. A continuación establece el intercambio de lugares, informando a cada becado e indicando que se confirme por parte de cada uno la conformidad del cambio. A continuación finaliza el caso de uso.*|
|**Flujo alternativo de eventos:**|
|4.*El sistema indica que faltan completarse datos obligatorios del formulario, retornando al punto 2 del flujo tipico de eventos.*|
|**Precondición:** El encargado de albergue accedió a su cuenta correctamente.|
|**Postcondición:** El encargado de albergue estableció un cambio de lugar para uno o dos becados.|
|**Requerimientos cumplidos:** requerimientos|

### Caso de Uso: Revocar beca

|**Nombre del Caso de Uso:** Revocar beca.|
|:---|
|**Actor(es):** Encargado de albergue.|
|**Descripcion:** Permitir al encargado de albergue revocar la beca a un becado y solicitar su desalojo en un plazo de tiempo.|
|**Evento desencadenador:** El encargado de albergue accede a los datos de un becado para revocar su beca.|
|**Flujo tipico de eventos (ruta principal):**|
|1.*Este caso de uso incia cuando el encargado de albergue accede a los datos de un becado para revocar su beca.*|
|2.*El sistema retorna un formulario de revocación de beca, solicitando seleccione el motivo por el cual se revoca la beca, detallando con una descripción y establezca un plazo de desalojo.*|
|3. *El encargado de albergue completa el formulario.*|
|4. *El sistema verifica que se han proporcionado todos los datos obligatorios del formulario. A continuación revoca el beneficio de beca e informa al becado el motivo y fecha limite de desalojo. A continuación muestra un mensaje de éxito y finaliza el caso de uso.*|
|**Flujo alternativo de eventos:**|
|4.*El sistema indica que faltan completarse datos obligatorios del formulario, retornando al punto 2 del flujo tipico de eventos.*|
|**Precondición:** El encargado de albergue accedió a su cuenta correctamente.|
|**Postcondición:** El encargado de albergues revocó la beca de un estudiante.|
|**Requerimientos cumplidos:** requerimientos|

### Caso de Uso: Planificar jornada de mantenimiento

|**Nombre del Caso de Uso:** Planificar jornada de mantenimiento.|
|:---|
|**Actor(es):** Encargado de albergue.|
|**Descripcion:** Permitir al encargado de albergue planificar una jornada de mantenimiento e incluir en ella pedidos de mantenimiento a atender.|
|**Evento desencadenador:** El encargado de albergue accede al apartado de mantenimiento para planificar una nueva jornada de mantenimiento.|
|**Flujo tipico de eventos (ruta principal):**|
|1.*Este caso de uso incia cuando el encargado de albergue accede al apartado de mantenimiento para planificar una nueva jornada de mantenimiento.*|
|2.*El sistema retorna un formulario de planificación de jornada, y una lista de pedidos de mantenimiento pendiente.*|
|3. *El encargado de albergue establece la fecha de la planificación, e incluye en ella las tareas de mantenimiento que se realizarán.*|
|4. *El sistema verifica que se han proporcionado todos los datos obligatorios del formulario. A continuación planifica una nueva jornada de mantenimiento, notifica a todos los becados de la misma, y finaliza el caso de Uso.*|
|**Flujo alternativo de eventos:**|
|2.*El sistema retorna un formulario de planificación e indica que no hay pedidos de mantenimiento pendientes, indicando que se pueden "registrar pedidos de mantenimiento" nuevas para la planificación, o en caso contrario, finalizar el caso de uso.*|
|4. *El sistema indica que faltan completarse datos obligatorios del formulario, retornando al punto 2 del flujo tipico de eventos.*|
|**Precondición:** El encargado de albergue accedió correctamente a su cuenta.|
|**Postcondición:** El encargado de albergues planificó una jornada de mantenimiento e incluyó en ella pedidos de mantenimiento a tratar, notificando a los becados.|
|**Requerimientos cumplidos:** requerimientos|

### Caso de Uso: Registrar casa

|**Nombre del Caso de Uso:** Registrar casa.|
|:---|
|**Actor(es):** Encargado de albergue.|
|**Descripcion:** Permitir al encargado de albergue registrar una casa de albergue universitario.|
|**Evento desencadenador:** El encargado de albergue accede al apartado de casas para registrar una nueva casa de albergue.|
|**Flujo tipico de eventos (ruta principal):**|
|1.*Este caso de uso incia cuando el ncargado de albergue accede al apartado de casas para registrar una nueva casa de albergue*|
|2.*El sistema retorna un formulario de registro de casas.*|
|3. *El encargado de albergue completa el formulario con los datos de una casa.*|
|4. *El sistema verifica que se han proporcionado todos los datos obligatorios del formulario. A continuación rgistra una nueva casa de albergue, y en base al numero de habitaciones y lugares por habitación, amplia el numero de becas otorgables.*|
|**Flujo alternativo de eventos:**|
|4. *El sistema indica que faltan completarse datos obligatorios del formulario, retornando al punto 2 del flujo tipico de eventos.*|
|**Precondición:** El encargado de albergues accedió correctamente a su cuenta.|
|**Postcondición:** El encargado de albergues registró con éxito una nueva casa para la beca de albergues.|
|**Requerimientos cumplidos:** requerimientos|

### Caso de Uso: Registrar bienes

|**Nombre del Caso de Uso:** Registrar bienes.|
|:---|
|**Actor(es):** Encargado de albergues.|
|**Descripcion:** Permitir al encargado de albergues registrar un bien ingresado a una de las casas erteneciente a un becado o perteneciente a una de las casas, siendo un bien un electrodoméstico, mueble, o alguna otra utilidad.|
|**Evento desencadenador:** El encargado de albergue selecciona una casa para la cual registrará un bien.|
|**Flujo tipico de eventos (ruta principal):**|
|1.*Este caso de uso incia cuando el encargado de albergue selecciona una casa para la cual registrará un bien.*|
|2.*El sistema retorna un formulario de registro para un bien.*|
|3. *El encargado de albergues completa el formulario con los datos de un bien, indicando si se trata de el bien de un becado, seleccionando al mismo, o propio de una casa.*|
|4. *El sistema verifica que se han proporcionado todos los datos obligatorios del formulario. A continuación registra el nuevo bien, si se trata del bien de un becado este es notificado, se notifica del éxito de la operación y finaliza el caso de uso.*|
|**Flujo alternativo de eventos:**|
|4. *El sistema indica que faltan completarse datos obligatorios del formulario, retornando al punto 2 del flujo tipico de eventos.*|
|**Precondición:** El encargado de albergues accedió correctamente a su cuenta.|
|**Postcondición:** El encargado de albergues registró un nuevo bien para una casa.|
|**Requerimientos cumplidos:** requerimientos|

### Titulo 3

|**Nombre del Caso de Uso:** Nombre|
|:---|
|**Actor(es):** Actores|
|**Descripcion:** descripcion|
|**Evento desencadenador:** evento|
|**Flujo tipico de eventos (ruta principal):**|
|1.*Este caso de uso incia cuando*|
|2.**|
|**Flujo alternativo de eventos:**|
|1.**|
|2.**|
|**Precondición:** precondicion|
|**Postcondición:** postcondicion|
|**Requerimientos cumplidos:** requerimientos|

volver al [principio](#escenarios-de-casos-de-uso)

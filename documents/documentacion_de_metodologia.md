# Documentación de Proyecto de Software. 

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

#### Indice de contenidos.

1. [Descripción del Escenario](#descripción-del-escenario)
    1. [Entrevistas y Cuestionarios](#entrevistas-y-cuestionarios)
    2. [Requerimientos](#requerimientos)
2. 


---

## Descripción del Escenario. 

volver al [Indice](#indice-de-contenidos)

Los albergues universitarios son un conjunto de casas destinadas a estudiantes de las carreras de la Universidad Nacional de Misiones, otorgadas como una beca. En la ciudad de Apóstoles está actualmente en funcionamiento un albergue para estudiantes de las carreras del Módulo de Informática de la FCEQyN. La “beca de albergue” es solicitada cada año a través de un formulario de google que registra las solicitudes en una planilla de cálculos, este formulario de solicitud está abierto un periodo de tiempo, al cerrar, el secretario de bienestar estudiantil revisa una a una cada petición, tomando en cuenta ciertas características primordiales de preseleccion de solicitudes, estas características son: distancia entre la localidad de origen del solicitante y las carreras informáticas, la situación socio-económica familiar (ganancias totales de la familia, el numero de integrantes de la familia y cuantos de ellos estudian), entre otros parámetros, (se da prioridad para la preseleccion a las peticiones en las que el interesado vive lejos de la ciudad de apóstoles y su familia tiene ganancias bajas); Además, el secretario de bienestar estudiantil debe separar las solicitudes nuevas de aquellas que son realizadas por alumnos anteriormente becados que desean renovar el beneficio, para estos últimos un requisito adicional es aprobar un mínimo de 2 materias del último año cursado. Finalmente el secretario de bienestar estudiantil comparte el acceso a la planilla de cálculos con las pre-selecciones al encargado de albergues, y además le envía un listado impreso de preseleccionados.

Los albergues universitarios tienen un encargado de albergue, su trabajo es analizar las solicitudes de beca preseleccionadas, las situaciones académicas de los solicitantes nuevos (si corresponde) o avanzados (solicitantes avanzados son los estudiantes con uno o mas años de uso de la beca.), y luego otorgar la beca teniendo en cuenta que solo se pueden emitir cierto numero de becas correspondiente a las plazas libres en cada casa. Otras responsabilidades del encargado de albergue son informar del reglamento de los albergues, de actuar según el incumplimiento de dichas normas y mediar en problemas de convivencia entre becados y en su solución. También se encarga de recopilar inconvenientes de mantenimiento en los albergues y planificar su reparación, planificar además las jornadas de limpieza y mantenimiento general de los albergues (la limpieza específica de cada casa es coordinada entre un delegado y los becados de la misa, se describirá mas adelante). El encargado de albergue también mantiene un registro de cada casa, y por cada casa el registro de las habitaciones, camas, colchones, muebles y electrodomésticos disponibles que son propiedad de los albergues.
 
Cada casa tiene un conjunto de habitaciones, 4 en total son destinadas para becados, cuenta con 1 baño instalado, y 1 cocina comedor, además de patio frontal y patio trasero. Cada habitación es estrictamente compartida por 2 becados, en las habitaciones mas pequeñas, y hasta 4 becados en la habitación mas grande, siendo hasta 10 el máximo de alumnos becados por casa. El total de 5 casas que forman parte del albergue universitario tienen exactamente el mismo diseño estructural, y están equipadas con muebles y electrodomésticos, y además con los servicios esenciales de luz y agua. De las 5 casas, 1 de ellas está destinada a becados femeninas, y las restantes 4 a becados masculinos. 
 
Para acceder a la beca por primera vez, un Estudiante debe realizar una solicitud a la secretaria de bienestar estudiantil a través de un formulario de google, informando sus datos personales, datos de su padre, madre, cantidad de integrantes de la familia, ingresos familiares, cantidad de integrantes de la familia que están estudiando, domicilio actual (se considera la distancia desde su domicilio hasta la ciudad de apóstoles como un factor en el análisis de la solicitud, junto a la situación económica de la familia) entre otros datos y subir documentación que respalde los datos declarados. Posteriormente para renovar la beca, cada becado debe, además de mantener sus datos actualizados, aprobar por promoción o examen final un mínimo de 2 materias de una misma carrera cada año. En caso de que el becado no cumpla en su totalidad los requisitos académicos para renovar la beca (por ejemplo, tenga aprobadas 1 de 2 materias necesarias), puede tratar alternativas para aprobar materias faltantes (en mesas de examen) con el encargado de albergue, el cual también considerará el problema por el cual no se cumplió el requisito, y considerará el nivel de convivencia del becado en años anteriores como un factor a tener en cuenta para acordar una alternativa (un ejemplo de alternativa es establecer un plazo hasta próximas mesas de examen para que el becado apruebe y cumpla el requisito académico). En caso de que el becado no cumpla requisitos académicos, no tenga un historial de buena convivencia y no pueda aprobar materias faltantes incluso habiéndose considerado la alternativa de ejemplo anterior, se procederá al cese de la beca, aviso al becado y posterior solicitud de desalojo de su lugar en la casa que tenga designada, pudiendo el becado llevarse consigo solamente los bienes que trajo en un principio y aquellos que pueda demostrar que son suyos. Otro caso particular de cese de beca es ante una falta grave del reglamento de albergues.  
 
Cada casa tiene un becado avanzado (mínimamente lleva un año como becado) que ejerce un papel de “delegado”, este papel es para la organización de cada casa y no es un puesto oficial, el delegado se encarga de coordinar las actividades de limpieza de la casa, guiando a los demás estudiantes nuevos las primeras semanas en la realización de cada tarea, estableciendo junto a ellos un cronograma de limpieza, la división del costo total de servicios de luz, agua e Internet (en caso de que la casa cuente con una conexión particular de Internet), recaudando el dinero del pago y realizando el pago de los servicios, poniendo a buen recaudo los comprobantes de pago. 
 
Cada becado tiene que cumplir con las normas de convivencia y el reglamento de los albergues universitarios, y además, estar dispuesto a prestar ayuda en la limpieza y mantenimiento básico de los albergues (limpieza de la casa, asistir en jornadas de limpieza general, asistir a días previamente designados para pintar las casas, colaborar con el mantenimiento de los patios) aunque no es obligatorio, finalmente, aunque la beca de albergue es gratuita, el pago de servicios de luz y agua es dividido por el numero de integrantes de cada casa y esto también aplica a servicios terceros no incluidos, como por ejemplo el contrato particular de Internet por parte de algún miembro de la casa. 
 
Cada casa cuenta con muebles y electrodomésticos propiedad de la universidad que pueden ser utilizados pero no sustraídos de las mismas bajo ningún concepto. Cada becado puede llevar efectos personales, equipaje, muebles tales como estantes, escritorios, electrodomésticos, etc. Sin embargo, bienes tales como heladeras, cocinas a gas, hornos eléctricos, cafeteras eléctricas u otros que se dispongan en la cocina comedor deben ser de uso compartido por todos los integrantes de la casa, teniendo conocimiento de esto el alumno becado dueño del bien y estando bajo toda la casa de becados la responsabilidad del uso y cuidado del mismo. Cuando un becado lleva muebles o electrodomésticos a la casa en la que vivirá, el encargado de albergue toma los datos de los bienes y los registra a nombre del becado, siendo estos bienes de propiedad del becado.

volver al [principio](#descripción-del-escenario)

## Entrevistas y Cuestionarios.

volver al [Indice](#indice-de-contenidos)

Acontinuación se incluye un enlce a las respuestas de las entrevistas realizadas al secretario de bienestar estudiantil y al encargado del albergue.

- **Ver [entrevistas](entrevistas.md).**

## Requerimientos.

volver al [Indice](#indice-de-contenidos)

### Definición de requerimientos del usuario.

|  **Requerimientos del usuario** |
|:--------------------------------|
|1. SiGAU controlará las solicitudes de estudiantes para la beca de albergue, los datos y documentos que se deben adjuntar y la pre-selección de solicitudes.|
|2. SiGAU mantendrá registrada cada casa de la beca, cada becado y lugares libres en cada casa.|
|3. SiGAU se encargará de planificar la limpieza de cada casa de la beca para cada becado.|
|4. SiGAU se encargará de mantener seguimiento sobre el pago de servicios domesticos de cada casa de la beca, resguardando las boletas y comprobantes de pago.|
|5. SiGAU permitirá registrar solicitudes de mantenimiento, y planificar jornadas de mantenimiento en las casas de la beca.|
|6. SiGAU mantendra un sistema de puntajes para cada becado según estos cumplan sus tareas de limpieza y de pago de cuentas a tiempo y en forma, luego usará el puntaje de cada becado para darle un beneficio o asignarle una sancion.|
|7. SiGAU mantendrá perfiles de usuario, para un administrador general, un auditor, el secretario de bienestar estudiantil, el encargado de albergues, estudiantes y becados, cada perfil tendrá cierto nivel de permisos y acceso a ciertas partes del sistema.|
|8. SiGAU tiene que ser facil de usar, con ventanas, texto y botones simples, y legible, también debe tener algún manual o guia de uso.|
|9. SiGAU debe emitir reportes sobre los becados, solicitudes de beca, casas, el mantenimiento y el nivel de limpeza.|

### Especificación de los requerimientos del sistema.

|  **Requerimientos del sistema, apartado 1.** |
|:---------------------------------------------|
|1.1 SiGAU Proporcionará un registro para usuarios estudiantes.|
|1.2 SiGAU Proporcionará un formulario de solicitud para los estudiantes registrados que tomará todos los datos de solicitud personales, académicos, socio-económicos, familiares  y permitirá subir archivos en formato PDF, imagen o documento de texto.|
|1.3 SiGAU Encriptará los datos personales y documentacion de cada estudiante en la base de datos.|
|1.4 SiGAU Realizará una pre-selección de solicitudes de beca según parámetros de selección pre-establecidos cuando el período de solicitud finalice.|
|1.5 SiGAU no debe permitir que se realice una solicitud hasta que se adjunten los documentos requeridos en cada apartado del formulario de solicitud en el formato adecuado.|

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
|3.3 SiGAU permitira que cada becado envié una o mas imagenes (fotos) del área o áreas que limpió para que sea calificada por los demás integrantes de la casa  (calificación del 1 "mal" al 10 "perfecto").|
|3.4 SiGAU re-planificará las tareas asignadas en un período de tiempo cuando se incluya un nuevo becado en una casa o cuando se quite un becado de una casa.|
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
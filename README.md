# choice_in_database_delvalle
primera pre-entrega

1. Descripción Temática de la Base de Datos

La base de datos choice_in está diseñada para gestionar un sistema de reservas de paquetes turísticos, que incluye clientes, proveedores, pagos, vuelos, alojamientos y actividades. Permite la gestión de reservas de paquetes turísticos, pagos asociados, así como la conexión con diferentes servicios como vuelos, alojamientos y actividades ofrecidos por proveedores. Se enfoca en ofrecer un registro detallado de cada cliente y sus interacciones con los diferentes servicios contratados.
2. Diagrama de Entidad-Relación (DER)

El Diagrama de Entidad-Relación muestra las entidades de la base de datos, sus atributos y las relaciones entre ellas. Puedes utilizar herramientas como MySQL Workbench, draw.io, Lucidchart, o cualquier otra que prefieras para crear el diagrama.

Principales Entidades y Relaciones:

    CLIENTE está relacionado con CLIENTE_CATEGORIA.
    RESERVA está relacionada con CLIENTE y PAQUETE_TURISTICO.
    PAQUETE_TURISTICO está relacionado con VUELO, ALOJAMIENTO, y ACTIVIDAD a través de tablas intermedias.
    PROVEEDOR proporciona VUELO, ALOJAMIENTO, y ACTIVIDAD.
    PAGO está relacionado con RESERVA.
    OPINION_CALIFICACION permite calificar vuelos, alojamientos y actividades.

3. Listado de Tablas con Descripción

A continuación, se presenta el listado de las tablas de la base de datos, junto con una breve descripción de cada una:

    CLIENTE_CATEGORIA: Define las categorías de clientes, incluyendo descripción y beneficios asociados.
    CLIENTE: Contiene información básica de los clientes, incluyendo su categoría.
    PAQUETE_TURISTICO: Describe los paquetes turísticos, incluyendo el precio y la disponibilidad.
    RESERVA: Registra las reservas realizadas por los clientes para los paquetes turísticos.
    PAGO: Registra los pagos realizados por los clientes asociados a una reserva.
    PROVEEDOR: Almacena la información de los proveedores que ofrecen vuelos, alojamientos y actividades.
    VUELO: Detalla la información sobre los vuelos ofrecidos en los paquetes turísticos.
    ALOJAMIENTO: Contiene la información sobre los alojamientos ofrecidos en los paquetes turísticos.
    ACTIVIDAD: Describe las actividades turísticas disponibles en los paquetes.
    OPINION_CALIFICACION: Permite registrar las opiniones y calificaciones de los clientes sobre vuelos, alojamientos y actividades.
    PAQUETE_VUELO, PAQUETE_ALOJAMIENTO, PAQUETE_ACTIVIDAD: Tablas intermedias que relacionan los paquetes turísticos con vuelos, alojamientos y actividades.

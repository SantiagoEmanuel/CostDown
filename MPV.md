# MVP

1. ## Objetivo del MVP

   El objetivo del MVP es ofrecer las funcionalidades esenciales para que los usuarios gestionen sus finanzas de forma simple, permitiéndote lanzar el producto rápidamente, obtener retroalimentación y ajustarlo antes de agregar más características avanzadas.

2. ## Funcionalidades Clave del MVP

   El MVP debe enfocarse en las funcionalidades básicas que permitirán a los usuarios gestionar sus finanzas, visualizar sus gastos y establecer presupuestos. A continuación, detallo las características esenciales:

   1. ### Registro e Inicio de Sesión

      Función: Permitir que los usuarios creen una cuenta y accedan a la plataforma.
      Características:
      Registro por email y contraseña.
      Autenticación usando JWT o Auth0.
      Protección de contraseñas mediante hashing seguro (por ejemplo, bcrypt).

   2. ### Gestión de Ingresos y Gastos

      - Función:

        Los usuarios podrán agregar manualmente sus ingresos y gastos.

      - Características:

        Formulario para ingresar detalles de un gasto o ingreso (categoría, monto, fecha).

        Clasificación de transacciones por categorías predeterminadas (alimentación, transporte, ocio, etc.).

        Posibilidad de editar o eliminar una transacción.

        Validaciones básicas (campos obligatorios, formatos numéricos, fechas).

   3. ### Gráficas de Seguimiento

      - Función:

        Visualizar las finanzas de forma gráfica, mostrando la evolución de ingresos y gastos.

      - Características:

        Gráfico mensual que muestre el total de ingresos vs. gastos.

        Gráfica de categorías (porcentaje del gasto total en cada categoría).

        Puedes usar ECharts o TradingView para gráficos interactivos.

   4. ### Presupuesto Mensual

      - Función:

        Los usuarios podrán definir un presupuesto mensual y recibir notificaciones si están cerca de alcanzarlo.

      - Características:

        Establecer un límite de gasto mensual global.

        Visualización del porcentaje consumido del presupuesto.

        Alertas automáticas cuando los gastos se acercan o superan el presupuesto.

   5. ### Resumen Mensual

      - Función:

        Ofrecer un resumen financiero básico del mes (gastos vs. ingresos).

      - Características:

        Total de ingresos, total de gastos y balance mensual (diferencia entre ingresos y gastos).

        Desglose por categoría (alimentación, transporte, ocio).

        Posibilidad de exportar el resumen en PDF o CSV.

3. ## Flujo de Usuario en el MVP

   **El flujo de usuario es importante para garantizar que la experiencia sea sencilla y fluida**

   - **Registro**: El usuario crea una cuenta con su correo electrónico y contraseña

   - **Inicio de sesión**: Una vez registrado, el usuario inicia sesión y accede a su panel financiero

   - **Agregar ingresos/gastos**: El usuario ingresa su información financiera diaria (manual en esta etapa)

   - **Visualizar gráficos**: Los usuarios pueden ver cómo sus ingresos y gastos evolucionan en tiempo real a través de gráficos

   - **Configurar presupuesto**: El usuario establece un presupuesto mensual para controlar sus gastos

   - **Resumen mensual**: Al final de cada mes, el usuario ve un resumen detallado de sus finanzas

4. ## Tecnología para el MVP

   ### Frontend

   - Next.js con React: Ideal para aplicaciones SPA (Single Page Applications) con la posibilidad de realizar SSR (Server-Side Rendering).
   - Tailwind CSS o Chakra UI: Para diseñar rápidamente una interfaz simple y eficiente.
   - ECharts: Para las gráficas interactivas de gastos e ingresos.

   ### Backend

   - Node.js (o Bun, si prefieres): Ideal para manejar la lógica del servidor.
   - Express.js: Simple y ligero para la API.
   - Base de datos SQL (PostgreSQL/MySQL): Te permitirá almacenar los ingresos y gastos de forma estructurada.

   ### Autenticación

   - JWT o Auth0: Para manejar la autenticación segura de los usuarios.

   ### Almacenamiento de datos

   - PostgreSQL/MySQL: Almacenar los datos financieros (gastos, ingresos, presupuestos) en una base de datos relacional.
   - Firebase (opcional): Si planeas manejar datos en tiempo real, Firebase puede ser útil para sincronización rápida entre dispositivos. 5. Cronograma de Desarrollo

## CRONOGRAMA

### Semana 1: Planificación y Configuración

- Configuración del entorno de desarrollo (Next.js, Node.js, Turso (SQLite) ).
- Creación del esquema de la base de datos (usuarios, ingresos, gastos, presupuestos).
- Diseño de las pantallas iniciales (registro, inicio de sesión, panel de usuario).

### Semana 2: Funcionalidades Básicas

- Implementar el registro y autenticación.
- Creación de las API para agregar, editar y eliminar ingresos/gastos.
- Implementación del panel principal con formularios para ingresar transacciones.

### Semana 3: Gráficas y Resumen

- Implementación de gráficas interactivas (ECharts) para visualizar ingresos y gastos.
- Desarrollo del módulo de presupuesto.
- Creación del resumen mensual con balance.

### Semana 4: Pruebas y Ajustes

- Pruebas funcionales y ajustes basados en la retroalimentación.
- Implementación de notificaciones básicas (para presupuestos).
- Ajustes finales en la interfaz de usuario

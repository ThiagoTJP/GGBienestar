# 🌸 GGBienestar - Sistema de Gestión Integral

**Aviso:** Este repositorio funciona como una **Vitrina (Showcase)** de un proyecto de software desarrollado para un cliente real (Centro de Estética). Por motivos de privacidad y seguridad, el código fuente completo y la base de datos se mantienen en un repositorio privado.

## 🚀 Sobre el Proyecto
GGBienestar (GabyGodoyBienestar) es una aplicación web administrativa diseñada a medida para digitalizar las operaciones diarias de un centro de estética. El sistema permite gestionar de manera centralizada al personal, los clientes y los servicios ofrecidos, optimizando los tiempos de recepción y administración.

## 🛠️ Stack Tecnológico
* **Frontend:** Next.js, Tailwind CSS
* **Backend & Base de Datos:** Supabase (PostgreSQL)
* **Arquitectura:** Single Page Application (SPA) orientada a componentes.

---

## 📸 Módulos y Funcionalidades Principales

A continuación se detallan los módulos principales del sistema, demostrando la capacidad de realizar operaciones CRUD (Crear, Leer, Actualizar, Borrar) sobre distintas entidades relacionadas.

### 1. Autenticación y Control de Acceso
Sistema de login seguro diseñado para el personal de recepción y administración, protegiendo los datos sensibles de los clientes y la facturación.

*[ARRASTRÁ LA IMAGEN login.png ACÁ Y BORRÁ ESTE TEXTO]*

### 2. Gestión del Equipo Médico (Doctores)
Módulo para la administración de los profesionales del centro. Permite dar de alta nuevos especialistas, editar sus datos de contacto y gestionar su estado (Activo/Inactivo) dentro de la plataforma. Cuenta con un buscador dinámico integrado.

**Vista General del Personal:**
*[ARRASTRÁ LA IMAGEN doctores.png ACÁ Y BORRÁ ESTE TEXTO]*

**Alta de un Nuevo Profesional:**
*[ARRASTRÁ LA IMAGEN seccion_nuevodoctor.png ACÁ Y BORRÁ ESTE TEXTO]*

### 3. Base de Datos de Pacientes
Registro centralizado de clientes. Permite tener a mano el contacto rápido de cada paciente y gestionar su historial de estado para futuras campañas de retención o turnos.

**Directorio de Pacientes:**
*[ARRASTRÁ LA IMAGEN pacientes.png ACÁ Y BORRÁ ESTE TEXTO]*

**Formulario de Ingreso (Nuevo Paciente):**
*[ARRASTRÁ LA IMAGEN seccion_nuevopaciente.png ACÁ Y BORRÁ ESTE TEXTO]*

### 4. Catálogo de Tratamientos
Administración de los servicios ofrecidos por la estética (ej. Botox, Masajes, Drenaje Linfático). Este módulo es vital, ya que parametriza la duración en minutos de cada servicio y sugiere un precio, datos que luego el sistema utiliza para calcular automáticamente los espacios en el calendario de turnos.

**Listado de Servicios Parametrizados:**
*[ARRASTRÁ LA IMAGEN tratamientos.png ACÁ Y BORRÁ ESTE TEXTO]*

**Configuración de un Nuevo Tratamiento:**
*[ARRASTRÁ LA IMAGEN seccion_nuevotratamiento.png ACÁ Y BORRÁ ESTE TEXTO]*

---

### 5. Agenda Interactiva y Gestión de Turnos
El corazón operativo de la clínica. Un calendario dinámico que previene superposiciones y facilita la lectura rápida de la jornada laboral.

* **Vista de Calendario Multiprofesional:** La agenda permite navegar por día, semana o mes, mostrando en columnas paralelas la disponibilidad y los turnos asignados a cada doctor.
* **Asignación Inteligente:** El modal de nuevo turno vincula automáticamente al paciente con el catálogo de tratamientos (o permite tratamientos personalizados), registrando el estado del turno y los montos.
* **Exportación Rápida a WhatsApp:** Funcionalidad diseñada a medida para las necesidades del cliente, que formatea y copia la agenda diaria/semanal de un doctor específico con un solo clic, lista para ser enviada por mensajería.

**Vista del Calendario:**
*[ARRASTRÁ LA IMAGEN turnos.png ACÁ Y BORRÁ ESTE TEXTO]*

**Creación de Turno:**
*[ARRASTRÁ LA IMAGEN seccion_nuevoturno.png ACÁ Y BORRÁ ESTE TEXTO]*

**Exportación para Recepción:**
*[ARRASTRÁ LA IMAGEN seccion_turnoscopiaragenda.png ACÁ Y BORRÁ ESTE TEXTO]*

---

### 6. Módulo de Facturación y Control de Pagos
Sistema de seguimiento financiero que permite auditar los ingresos del negocio y gestionar morosidades.

* **Panel de Control Financiero:** Una tabla centralizada que calcula en tiempo real el total recaudado según los filtros aplicados (por fechas predefinidas o rangos personalizados, métodos de pago y estados).
* **Gestión de Saldos y Pagos Parciales:** Lógica avanzada para manejar el estado de cuenta de cada turno. Permite registrar múltiples entregas de dinero (historial de pagos) sobre un mismo tratamiento, calculando automáticamente el saldo deudor restante y actualizando el estado a "Pagado" o "Parcial".

**Dashboard de Ingresos y Filtros:**
*[ARRASTRÁ LA IMAGEN pagos.png ACÁ Y BORRÁ ESTE TEXTO]*

**Control de Saldos y Pagos Parciales:**
*[ARRASTRÁ LA IMAGEN seccion_editarpagos.png ACÁ Y BORRÁ ESTE TEXTO]*

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

<img width="1917" height="911" alt="login" src="https://github.com/user-attachments/assets/84e526ea-d715-45ec-ac33-6525de379fb8" />

### 2. Gestión del Equipo Médico (Doctores)
Módulo para la administración de los profesionales del centro. Permite dar de alta nuevos especialistas, editar sus datos de contacto y gestionar su estado (Activo/Inactivo) dentro de la plataforma. Cuenta con un buscador dinámico integrado.

**Vista General del Personal:**
<img width="1911" height="905" alt="doctores" src="https://github.com/user-attachments/assets/e71261c4-570e-4cf4-97c8-6e24737ed64e" />

**Alta de un Nuevo Profesional:**
<img width="1910" height="912" alt="seccion_nuevodoctor" src="https://github.com/user-attachments/assets/1c827322-3ac8-4c78-9784-0a04b1f51e7a" />

### 3. Base de Datos de Pacientes
Registro centralizado de clientes. Permite tener a mano el contacto rápido de cada paciente y gestionar su historial de estado para futuras campañas de retención o turnos.

**Directorio de Pacientes:**
<img width="1916" height="908" alt="pacientes" src="https://github.com/user-attachments/assets/38a44680-e179-433a-b9f1-dddf138a9c98" />

**Formulario de Ingreso (Nuevo Paciente):**
<img width="1914" height="913" alt="seccion_nuevopaciente" src="https://github.com/user-attachments/assets/29eaab93-7bc1-4924-8ecb-9d81bff990df" />

### 4. Catálogo de Tratamientos
Administración de los servicios ofrecidos por la estética (ej. Botox, Masajes, Drenaje Linfático). Este módulo es vital, ya que parametriza la duración en minutos de cada servicio y sugiere un precio, datos que luego el sistema utiliza para calcular automáticamente los espacios en el calendario de turnos.

**Listado de Servicios Parametrizados:**
<img width="1914" height="908" alt="tratamientos" src="https://github.com/user-attachments/assets/15aa1e95-5141-4c41-a59f-95d98ef8190d" />

**Configuración de un Nuevo Tratamiento:**
<img width="1918" height="911" alt="seccion_nuevotratamiento" src="https://github.com/user-attachments/assets/efbe8e63-7b9f-4d4c-be7f-9351fb67683a" />

### 5. Agenda Interactiva y Gestión de Turnos
El corazón operativo de la clínica. Un calendario dinámico que previene superposiciones y facilita la lectura rápida de la jornada laboral.

* **Vista de Calendario Multiprofesional:** La agenda permite navegar por día, semana o mes, mostrando en columnas paralelas la disponibilidad y los turnos asignados a cada doctor.
* **Asignación Inteligente:** El modal de nuevo turno vincula automáticamente al paciente con el catálogo de tratamientos (o permite tratamientos personalizados), registrando el estado del turno y los montos.
* **Exportación Rápida a WhatsApp:** Funcionalidad diseñada a medida para las necesidades del cliente, que formatea y copia la agenda diaria/semanal de un doctor específico con un solo clic, lista para ser enviada por mensajería.

**Vista del Calendario:**
<img width="1913" height="909" alt="turnos" src="https://github.com/user-attachments/assets/0b1b0472-f707-420a-8d76-f7f4ce1ca5b8" />

**Creación de Turno:**
<img width="1911" height="905" alt="seccion_nuevoturno" src="https://github.com/user-attachments/assets/26e63ebb-6951-4c05-90c2-0ac9472f0e1e" />

**Exportación para Recepción:**
<img width="1921" height="909" alt="seccion_turnoscopiaragenda" src="https://github.com/user-attachments/assets/98a0bf2f-0b27-4f71-90b3-66a095fc4202" />

El mensaje que se copia es similar a este: 
"📋 Agenda Thiago Poletti
24/08 - 30/08
Miércoles 26/08
10:00 - Laura Jimenes - Drenaje Linfático"

**Recordatorio para el cliente:**
<img width="1921" height="911" alt="recordatorioturno" src="https://github.com/user-attachments/assets/bd2a5dc4-21b9-4ddc-93b4-14f092c87539" />

El mensaje que se manda es similar a este:
"Hola Laura 🩷 Tenemos agendado turno para Drenaje Linfático el MIÉRCOLES 26-08 a las 10:00hs 
¿Confirmamos el turno? 🫶🏻

📍 Av. Cabildo 321, CABA. Te dejo adjunto el link de Google maps con la ubicación: (Link de la ubicación de la estetica)

Si necesitás reprogramar, avisame con al menos 48 horas de anticipación (dentro del horario de atención: 9 a 18 hs) para poder ofrecerle el espacio a otra persona 🫶🏻

Gracias, Dr. 🪬"

---

### 6. Módulo de Facturación y Control de Pagos
Sistema de seguimiento financiero que permite auditar los ingresos del negocio y gestionar morosidades.

* **Panel de Control Financiero:** Una tabla centralizada que calcula en tiempo real el total recaudado según los filtros aplicados (por fechas predefinidas o rangos personalizados, métodos de pago y estados).
* **Gestión de Saldos y Pagos Parciales:** Lógica avanzada para manejar el estado de cuenta de cada turno. Permite registrar múltiples entregas de dinero (historial de pagos) sobre un mismo tratamiento, calculando automáticamente el saldo deudor restante y actualizando el estado a "Pagado" o "Parcial".

**Dashboard de Ingresos y Filtros:**
<img width="1912" height="904" alt="pagos" src="https://github.com/user-attachments/assets/5ab45957-2546-4c52-97ca-0396e00d0afd" />

**Control de Saldos y Pagos Parciales:**
<img width="1911" height="906" alt="seccion_editarpagos" src="https://github.com/user-attachments/assets/b8ebeeea-b457-47ac-8b5f-0db8644cfde2" />

---

*Desarrollado por [Thiago Poletti](https://github.com/ThiagoTJP | https://www.linkedin.com/in/thiago-poletti/).*

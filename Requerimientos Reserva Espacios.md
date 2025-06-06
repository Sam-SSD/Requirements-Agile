# 📚 Plataforma de Reserva de Espacios de Estudio  
**Documento de Requerimientos del Cliente**

---

## 🧭 Propósito del Sistema

El objetivo del sistema es permitir a estudiantes reservar espacios de estudio colaborativos (salones, cubículos, etc.) por franjas horarias, gestionar sus reservas, cancelar si es necesario y acceder físicamente mediante códigos QR. El sistema debe ser accesible, eficiente y seguro.

---

## 👥 Usuarios del Sistema

Los principales perfiles de usuario serán:

- **Estudiante (usuario final)**
- **Administrador (gestión de espacios y control general)**
- **Personal de soporte (monitoreo y validación en sitio)**

---

## ✅ Requerimientos Funcionales

### 👤 Gestión de Usuarios

**Acciones disponibles:**
- Registro e inicio de sesión
- Gestión de perfil
- Cambio de contraseña
- Consulta de historial de reservas

**Campos requeridos en el registro:**
- Nombre completo
- Correo institucional
- Número de identificación
- Programa académico
- Rol (estudiante / administrador)
- Contraseña

**Niveles de acceso:**
- **Estudiante:** Crear y cancelar reservas, generar QR de acceso  
- **Administrador:** Gestión de espacios, horarios, reportes y usuarios  
- **Soporte:** Validación en sitio y control de asistencia mediante escaneo de QR  

---

### 📅 Gestión de Reservas

**Tipos de espacios disponibles:**
- Cubículos individuales
- Salones grupales
- Salas de trabajo colaborativo

**Flujo de reserva:**
1. Selección de tipo de espacio
2. Selección de día y franja horaria
3. Confirmación de disponibilidad
4. Confirmación de reserva y generación de QR
5. Visualización en el historial

**Otras funcionalidades:**
- Cancelación de reservas con anticipación
- Reglas de uso (ej. máximo de reservas diarias)
- Visualización de disponibilidad en calendario

---

### 🔐 Acceso con Código QR

**Acciones automáticas del sistema:**
- Generación de código QR único al confirmar una reserva
- Escaneo en sitio para validar acceso
- Registro de asistencia
- Bloqueo automático por inasistencia recurrente (opcional)

---

### 🛠 Funciones Administrativas

**Acciones del administrador:**
- Registro y edición de espacios disponibles
- Gestión de franjas horarias y horarios de apertura
- Monitoreo de ocupación y uso
- Generación de reportes de uso por estudiante, espacio y horario
- Gestión de usuarios y control de acceso

---

## 🔔 Comunicación y Notificaciones

**Notificaciones enviadas por el sistema:**
- Confirmación o cancelación de reservas
- Recordatorios antes de la franja reservada
- Avisos de penalización por inasistencia
- Enlace para regenerar QR en caso de pérdida

**Canales sugeridos:**
- Correo electrónico institucional
- Notificaciones push (si hay app móvil)
- WhatsApp (opcional)

---

## 🛠 Requerimientos No Funcionales

**Dispositivos compatibles:**
- Computadoras
- Teléfonos celulares
- Tablets

**Disponibilidad del sistema:**  
24/7, con administración horaria según políticas de la institución.

**Velocidad y rendimiento:**  
- Interfaz rápida y responsiva  
- Visualización de disponibilidad en tiempo real  
- QR generado instantáneamente

**Seguridad:**  
- Autenticación segura (correo y contraseña o SSO institucional)  
- Información encriptada  
- Control de acceso físico mediante códigos QR únicos y temporales

**Integraciones sugeridas:**
- Google Calendar / iCal (opcional)
- Plataforma institucional (para validación de identidad)
- Sistema de escaneo QR en entrada física

---

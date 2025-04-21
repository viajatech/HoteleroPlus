# Hotelero Plus by Viaja Tech 🏨⚡

> **La navaja suiza open‑source para la operación hotelera moderna.**  
> Gestión de huéspedes, habitaciones, reservas, proveedores **y** horarios laborales en una sola app de escritorio **Python + PyQt5**. Sin licencias ocultas, sin dependencia de la nube, con licencia **Apache 2.0** para que la hackees a tu gusto.

<p align="center">
  <img src="docs/banner_hotelero_plus.svg" alt="Hotelero Plus banner">
</p>

---

## 🚀 Por qué te va a encantar

| Módulo | Superpoder |
| ------ | ---------- |
| **Login seguro** | BCrypt + SQLite: usuarios, roles y auditoría de sesiones |
| **Mapa de habitaciones** | Plano visual drag‑&‑drop con estados de color (disponible, ocupado, VIP, mantenimiento…) |
| **Wizard de reservas** | Checkout ágil con cálculo automático de noches, tarifas y cargos extra |
| **CRM de huéspedes** | Historial, cargos adicionales y generación de QR para check‑in express |
| **Proveedores & deudas** | Control de cuentas por pagar con filtros y alertas |
| **Reporting** | Gráficas de ingresos / pasivos y exportación a **PDF** o **Word** |
| **Hotel Analytics** | Resúmenes de horas trabajadas, días laborados y cumplimiento LFT 🇲🇽 |
| **Scheduler IA‑Ready** | Generación y asignación automática de turnos 24/7 (mañana‑tarde‑noche) + export a **Excel** |
| **Made in MX** | Integra los artículos clave de la Ley Federal del Trabajo para evitar multas |

---

## ✨ Capturas de pantalla

> *(Añade tus screenshots en `docs/` — aquí va solo el layout placeholder)*

<p align="center">
  <img src="docs/screenshot_dashboard.png" width="800">
  <br><em>Panel principal con pestañas dinámicas</em>
</p>

---

## 🛠️ Instalación rápida

```bash
git clone https://github.com/viajatech/HoteleroPlus.git
cd HoteleroPlus
python -m venv venv && source venv/bin/activate  # opcional
pip install -r requirements.txt                  # PyQt5, pandas, bcrypt, reportlab, etc.
python hotelero_plus.py                          # ¡Listo!


┌─────────── GUI (PyQt5) ────────────┐
│  Tabs: Login · Rooms · Guests · … │
└──────────────┬────────────────────┘
               │ signals / slots
        SQLite 3 (hotelero.db)
               │ ORM‑lite via cursor
┌───── Business Logic Layers ──────┐
│ • Habitaciones                   │
│ • Reservas & Guests              │
│ • Proveedores & Deuda            │
│ • Schedules (horario laboral)    │
└───────────────────────────────────┘

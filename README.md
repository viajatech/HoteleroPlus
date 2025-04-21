# Hotelero Plus by Viaja Tech 🏨⚡

> **La navaja suiza open‑source para la operación hotelera moderna.**  
> Gestión de huéspedes, habitaciones, reservas, proveedores **y** horarios laborales en una sola app de escritorio **Python + PyQt5**. Sin licencias ocultas, sin dependencia de la nube, con licencia **Apache 2.0** para que la hackees a tu gusto.


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

```markdown
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
```

> **Tip:** El primer usuario lo registras desde la misma pantalla de login—elige rol **Administrador**.

---

## 🏗️ Arquitectura en 30 segundos

```
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
```

---

## 📍 Roadmap

- [ ] Multi‑propiedad (cadena hotelera)  
- [ ] Sincronización en la nube (PostgreSQL / REST)  
- [ ] Módulo de housekeeping móvil (Flutter)  
- [ ] Integración con puertas IoT & POS

> Abre un issue o un pull request y construyamos esto juntos.

---

## 🤝 Contribuir

1. Haz fork, crea una rama con tu feature (`git checkout -b feature/mi‑feature`)
2. Sigue la guía de estilo **PEP‑8**
3. Incluye pruebas o una demo GIF
4. Envía PR 🍻

---

## 🧾 Licencia

Este proyecto se publica bajo la **Apache License 2.0**.  
Libertad para usarlo, forkearlo y mejorarlo, siempre citando a Viaja Tech.

---

## ⭐ Agradecimientos

- **PyQt5** por la magia visual  
- **ReportLab** & **matplotlib** por los PDFs y gráficas  
- Comunidad open‑source por la inspiración constante

---

## ⚡ TL;DR

*Hotelero Plus* es una aplicación de escritorio 100 % Python que reúne **gestión hotelera completa**, reportes financieros y un **generador inteligente de horarios** en un solo lugar. Corre localmente, guarda todo en SQLite y exporta a PDF, Word o Excel con un clic — ¡ideal para hoteles boutique que quieren músculo digital sin pagar SaaS caros!

---

<p align="center">
Hecho con ❤️ y café por <strong>Viaja Tech</strong>
</p>
```
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

# 🌍 Ruber — Guía Turística Inteligente

Plataforma web basada en Django para la planificación personalizada de viajes, cálculo de rutas óptimas y emisión digital de tickets.

---

## Características

- **Gestión de usuarios:** Registro, perfiles personalizados y preferencias de viaje.
- **Catálogo de destinos:** Organización por categorías, actividades y costos.
- **Rutas inteligentes:** Cálculo de rutas óptimas mediante algoritmos de grafos (Dijkstra).
- **Generador de itinerarios:** Planificación automática ajustada a presupuesto y disponibilidad horaria.
- **Ticketing digital:** Emisión de boletos con códigos QR dinámicos.
- **Búsqueda inteligente:** Soporte planificado para consultas en lenguaje natural.

---

## Stack Tecnológico

| Componente | Tecnología |
| :--- | :--- |
| **Backend** | Python 3.10+, Django 4.2 LTS |
| **Base de datos** | SQLite (desarrollo) / PostgreSQL (producción) |
| **Frontend** | HTML5, CSS3, JavaScript, Bootstrap 5 (Crispy Forms) |
| **Librerías clave** | `Pillow`, `qrcode`, `python-decouple` |
| **Algoritmia** | Grafos, Dijkstra, Combinatoria |

---

## Estructura del Proyecto

```text
ruber_project/
├── core/           # Vistas principales, landing page y configuración base
├── usuarios/       # Modelo de usuario personalizado (Turista) y autenticación
├── lugares/        # Gestión de destinos, atracciones y categorías
├── rutas/          # Lógica y algoritmos de optimización de rutas (Dijkstra)
├── itinerarios/    # Generación y persistencia de planes de viaje
└── tickets/        # Generación de pases y códigos QR

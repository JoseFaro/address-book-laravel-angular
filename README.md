# Address Book — Laravel 11 + Angular 18

Aplicación web de directorio de contactos desarrollada como prueba
técnica en una ventana de 24 horas. El resultado fue satisfactorio
y derivó en una oferta de trabajo.

## Funcionalidades

- Registro y gestión de contactos con datos personales
- Soporte para múltiples teléfonos y correos por contacto
  — almacenados en tablas independientes con relación a la entidad principal
- Selección de teléfono y correo predeterminado visible en tabla principal
- Tabla con buscador en tiempo real sobre campos clave
- Arquitectura Full Stack completa — Laravel en backend, Angular en frontend

## Arquitectura

    app/
    ├── Http/Controllers/    # ContactController
    ├── Models/              # Address, Contact, Email, Phone, User
    ├── Providers/           # Service Providers
    ├── Repositories/        # ContactRepository — capa de acceso a datos
    └── Services/            # ContactService — lógica de negocio

    resources/angular/src/   # Frontend Angular 18

    database/
    ├── migrations/          # Esquema normalizado con tablas relacionadas
    ├── factories/
    └── seeders/

## Stack técnico

- **Backend:** PHP, Laravel 11
- **Frontend:** Angular 18, TypeScript, SCSS
- **Base de datos:** MySQL — esquema normalizado con relaciones
- **Arquitectura:** Repositories + Services para separación de
  lógica de negocio y acceso a datos

## Contexto

Prueba técnica con límite de 24 horas. Enfoque en arquitectura
limpia, separación de responsabilidades y entrega funcional
dentro del tiempo establecido.

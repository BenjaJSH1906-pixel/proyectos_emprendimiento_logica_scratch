# 🧠 Lógica del Negocio: Vinloop

## 📖 Descripción

**Vinloop** es un emprendimiento que ofrece mini reproductores de música personalizables. El sistema permite al cliente elegir entre un modelo estándar o uno personalizado, verificando primero si existe stock disponible.

---

## 🔄 Flujo principal

```mermaid
flowchart TD
    A[Inicio] --> B[Bienvenido a Vinloop]
    B --> C{¿Desea personalizar su mini reproductor?}

    C -- Sí --> D{¿Hay stock disponible?}
    C -- No --> E[Seleccionar modelo estándar]
    E --> Z[Fin]

    D -- Sí --> F[Ingresar nombre personalizado]
    F --> G[Seleccionar playlist]
    G --> H[Confirmar personalización]
    H --> Z

    D -- No --> I[Producto agotado]
    I --> Z[Fin]
```

---

## 💻 Pseudocódigo

```text
INICIO

Mostrar "Bienvenido a Vinloop"

Leer personalizar

Si personalizar = "Sí" Entonces

    Si hay_stock Entonces

        Leer nombre
        Leer playlist

        Mostrar "Mini reproductor personalizado correctamente."

    SiNo

        Mostrar "Producto agotado."

    FinSi

SiNo

    Mostrar "Se ha seleccionado un modelo estándar."

FinSi

FIN
```

---

## 🎮 Simulación en Scratch

- **Nombre del proyecto:** Vinloop-logica
- **Hecho por:** Domenica
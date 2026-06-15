# 🧠 Lógica del Negocio: Inspira+

## 📖 Descripción

**Inspira+** es un sistema que orienta a estudiantes interesados en postular a becas. Evalúa si el usuario cumple con tres requisitos importantes: contar con un certificado de inglés, demostrar liderazgo y haber realizado voluntariados. Si no cumple alguno de estos requisitos, el sistema le brinda una recomendación para mejorar su perfil antes de aplicar.

---

## 🔄 Flujo principal

```mermaid
flowchart TD
    A[Inicio] --> B[¿Tiene certificado de inglés?]

    B -- Sí --> C[¿Tiene liderazgo?]
    B -- No --> D[Debe mejorar su inglés antes de aplicar a becas]
    D --> Z[Fin]

    C -- Sí --> E[¿Ha realizado voluntariado?]
    C -- No --> F[Le recomendamos desarrollar liderazgo]
    F --> Z

    E -- Sí --> G[¡Tu perfil está listo para aplicar a becas!]
    E -- No --> H[Te recomendamos realizar más voluntariados para mejorar tu perfil]
    H --> Z

    G --> Z
```

---

## 💻 Pseudocódigo

```text
INICIO

Leer certificado_ingles

Si certificado_ingles = "Sí" Entonces

    Leer liderazgo

    Si liderazgo = "Sí" Entonces

        Leer voluntariado

        Si voluntariado = "Sí" Entonces
            Mostrar "¡Tu perfil está listo para aplicar a becas!"
        SiNo
            Mostrar "Te recomendamos realizar más voluntariados para mejorar tu perfil."
        FinSi

    SiNo
        Mostrar "Le recomendamos desarrollar liderazgo."
    FinSi

SiNo
    Mostrar "Debe mejorar su inglés antes de aplicar a becas."
FinSi

FIN
```

---

## 🎮 Simulación en Scratch

- **Nombre del proyecto:** Inspira+-logica
- **Hecho por:** Domenica
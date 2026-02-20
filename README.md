# Proyecto 13: Estrategias de Retención Model Fitness
> **Análisis de Pronósticos y Predicciones de Churn**

---

## 📋 Descripción del Proyecto
La cadena de gimnasios **Model Fitness** está desarrollando una estrategia de interacción con clientes basada en datos analíticos. El desafío principal es combatir la **tasa de cancelación (churn)**.

En el contexto de un gimnasio, la pérdida se define cuando un cliente deja de asistir durante **un mes**. El objetivo es identificar estos patrones antes de que el cliente abandone definitivamente la membresía.

### 🎯 Objetivo
Analizar los perfiles digitalizados de los clientes para elaborar una estrategia de retención efectiva basada en su comportamiento y características demográficas.

---

## 📊 Descripción de los Datos
Los datos contienen información del mes actual y el historial previo.

### Información del Usuario
| Campo | Descripción |
| :--- | :--- |
| `gender` | Género del usuario. |
| `Near_Location` | Proximidad al gimnasio (vive o trabaja cerca). |
| `Partner` | Empleado de una compañía asociada (descuento corporativo). |
| `Promo_friends` | Registro mediante oferta "Trae a un amigo". |
| `Phone` | Disponibilidad de número telefónico. |
| `Age` | Edad del usuario. |
| `Lifetime` | Meses desde su primera visita. |

### Historial y Membresía
* **`Contract_period`**: Duración del contrato (1, 3, 6 o 12 meses).
* **`Month_to_end_contract`**: Meses restantes para el vencimiento.
* **`Group_visits`**: Participación en clases grupales.
* **`Avg_class_frequency_total`**: Promedio de visitas semanales histórico.
* **`Avg_additional_charges_total`**: Gasto total en servicios extras (cafetería, masajes, etc.).
* **`Churn`**: Cancelación del mes en cuestión (Variable objetivo).

---

## 💡 Conclusiones y Estrategias Sugeridas

Tras el análisis de segmentación, se han priorizado dos grupos clave para aplicar medidas de mitigación inmediatas:

### 🟢 Cluster 0: Clientes de Alta Lealtad
**Perfil:** Usuarios de mayor poder adquisitivo y compromiso.
* **Servicio Premium:** Membresías con acceso a clases personalizadas.
* **Exclusividad:** Acceso a zonas VIP o espacios exclusivos de ejercicio.
* **Fidelización:** Kit de productos del gym (merchandising) incluido en su anualidad.

### 🔴 Cluster 4: Clientes en Riesgo
**Perfil:** Usuarios jóvenes con menor presupuesto o propensos al abandono.
* **Flexibilidad Económica:** Promociones por volumen o créditos para pago a plazos.
* **Bono de Distancia:** Descuentos especiales para quienes no viven cerca del centro.
* **Gamificación:** Cupones de tienda canjeables por asistencia constante (recompensa por hábito).

---

## 🔗 Enlaces del Proyecto
* [📂 Ver Notebook en GitHub](https://github.com/LuisPeza/Proyecto_13/blob/main/Proyecto_13_pronosticos.ipynb)

<h1> Proyecto_13 </h1>
Pronósticos y predicciones

<h2>Descripción del proyecto</h2>
La cadena de gimnasios Model Fitness está desarrollando una estrategia de interacción con clientes basada en datos analíticos.

Uno de los problemas más comunes que enfrentan los gimnasios y otros servicios es la pérdida de clientes. ¿Cómo descubres si un/a cliente ya no está contigo? Puedes calcular la pérdida en función de las personas que se deshacen de sus cuentas o no renuevan sus contratos. Sin embargo, a veces no es obvio que un/a cliente se haya ido: puede que se vaya de puntillas.

Los indicadores de pérdida varían de un campo a otro. Si un usuario o una usuaria compra en una tienda en línea con poca frecuencia, pero con regularidad, no se puede decir que ha huido. Pero si durante dos semanas no ha abierto un canal que se actualiza a diario, es motivo de preocupación: es posible que tu seguidor o seguidor/a se haya aburrido y te haya abandonado.

En el caso de un gimnasio, tiene sentido decir que un/a cliente se ha ido si no viene durante un mes. Por supuesto, es posible que estén en Cancún y retomen sus visitas cuando regresen, pero ese no es un caso típico. Por lo general, si un/a cliente se une, viene varias veces y luego desaparece, es poco probable que regrese.

<h3>Objetivo</h3>
Con el fin de combatir la cancelación, Model Fitness ha digitalizado varios de sus perfiles de clientes. Tu tarea consiste en analizarlos y elaborar una estrategia de retención de clientes.

<h3>Descripcion de los datos</h3>

Model Fitness te aportó archivos CSV que contienen los datos sobre la cancelación de un mes en concreto e información del mes que lo precedía.

- 'Churn' — la cancelación para el mes en cuestión
Campos de dataset actuales:
Datos del usuario del mes anterior
- 'gender'.
- 'Near_Location' — si el/la usuario/a vive o trabaja en el vecindario donde se encuentra el gimnasio.
- 'Partner' — si el/la usuario/a trabaja en una compañía asociada (el gimnasio tiene empresas asociadas cuyos empleados obtienen descuentos; en esos casos el gimnasio almacena información sobre los empleadores de los clientes).
- Promo_friends — si el/la usuario/a originalmente se inscribió mediante una oferta “trae a un/a amigo/a” (se utilizó el código promocional de un/a amigo/a cuando pagaron el primer abono).
- 'Phone' — si el/la usuario/a aportó el número de teléfono.
- 'Age'.
- 'Lifetime' — el tiempo (en meses) desde que el/la usuario/a llegó por primera vez al gimnasio.

Datos del registro de visitas y compras y datos sobre el estado actual de la membresía:
- 'Contract_period' — 1 mes, 3 meses, 6 meses o 1 año.
- 'Month_to_end_contract' — los meses que faltan hasta que expire el contrato.
- 'Group_visits' — si el/la usuario/a participa en sesiones grupales.
- 'Avg_class_frequency_total' — frecuencia media de visitas por semana a lo largo de la vida del cliente.
- 'Avg_class_frequency_current_month' — frecuencia media de visitas por semana durante el mes en curso.
'Avg_additional_charges_total' — cantidad total de dinero gastado en otros servicios del gimnasio: cafetería, productos deportivos, cosméticos, masajes, etc.

<!DOCTYPE html>
<html lang="es">
<head>
<style>
    body { font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif; line-height: 1.6; color: #333; }
    .container { max-width: 800px; margin: 20px auto; padding: 20px; }
    
    .intro { background: #f8f9fa; border-left: 5px solid #2c3e50; padding: 15px; margin-bottom: 30px; border-radius: 4px; }
    
    .cluster-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 20px; }
    
    .card { border: 1px solid #e1e4e8; border-radius: 8px; padding: 20px; transition: transform 0.2s; }
    .card:hover { transform: translateY(-5px); box-shadow: 0 4px 15px rgba(0,0,0,0.1); }
    
    .high-loyalty { border-top: 5px solid #27ae60; }
    .high-risk { border-top: 5px solid #e74c3c; }
    
    h2 { font-size: 1.2rem; margin-top: 0; color: #2c3e50; }
    h3 { font-size: 1rem; color: #7f8c8d; margin-bottom: 15px; }
    
    ul { padding-left: 20px; }
    li { margin-bottom: 10px; }
    
    .badge { display: inline-block; padding: 3px 10px; border-radius: 20px; font-size: 0.8rem; font-weight: bold; margin-bottom: 10px; }
    .badge-green { background: #d4edda; color: #155724; }
    .badge-red { background: #f8d7da; color: #721c24; }
</style>
</head>
<body>

<div class="container">
    <div class="intro">
        <strong>Conclusiones del Análisis:</strong> Se observa que el <strong>Cluster 4</strong> representa a los usuarios con mayor riesgo de fuga, mientras que el <strong>Cluster 0</strong> muestra la mayor lealtad. A continuación, se proponen estrategias de mitigación:
    </div>

    <div class="cluster-grid">
        <div class="card high-loyalty">
            <span class="badge badge-green">Mayor Lealtad</span>
            <h2>Cluster 0: Premium</h2>
            <h3>Perfil: Alto poder adquisitivo</h3>
            <ul>
                <li><strong>Servicio Premium:</strong> Membresía con acceso a clases personalizadas.</li>
                <li><strong>Exclusividad:</strong> Espacios preferenciales para entrenamiento.</li>
                <li><strong>Beneficios Físicos:</strong> Inclusión de productos oficiales con el pago de membresía.</li>
            </ul>
        </div>

        <div class="card high-risk">
            <span class="badge badge-red">Propenso a Cancelar</span>
            <h2>Cluster 4: Jóvenes</h2>
            <h3>Perfil: Menor edad y presupuesto</h3>
            <ul>
                <li><strong>Flexibilidad Financiera:</strong> Descuentos, promociones y créditos a meses sin intereses.</li>
                <li><strong>Incentivo Geográfico:</strong> Descuento especial por lejanía del gimnasio.</li>
                <li><strong>Gamificación:</strong> Cupones canjeables en la tienda del gym por asistencia regular.</li>
            </ul>
        </div>
    </div>
</div>

</body>
</html>


<a href="https://github.com/LuisPeza/Proyecto_13/blob/main/Proyecto_13_pronosticos.ipynb">Abrir proyecto</a>.


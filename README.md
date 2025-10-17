# 🧾 Invoice Payment Status Report – n8n Automation

Este flujo automatiza la generación y envío semanal de un reporte de facturas pendientes de pago.  
Utiliza **QuickBooks Online**, **Google Sheets** y **Gmail**, integrados mediante **n8n**, para consolidar información contable y enviarla automáticamente al equipo de finanzas.

## ⚙️ Flujo de Trabajo

1. **Schedule Trigger:** ejecuta el flujo todos los lunes a las 8:00 a.m.  
2. **QuickBooks Online:** obtiene todas las facturas desde la API.  
3. **IF Node:** filtra aquellas con saldo pendiente.  
4. **Set Node:** limpia y formatea los campos principales (Cliente, Fecha, Monto, Balance, Estado).  
5. **Google Sheets:** registra los datos en un reporte dinámico.  
6. **Gmail:** envía automáticamente un correo con la tabla de resultados a `accounting@miningstore.com`, con copia a `jp@miningstore.com`.

## 🧩 Tecnologías y Herramientas

- **n8n** (Low-code Automation Platform)  
- **QuickBooks Online API**  
- **Google Sheets API**  
- **Gmail API**

## 📈 Resultado

Cada semana, el equipo contable recibe un correo automatizado con el estado actualizado de todas las facturas, reduciendo el tiempo manual de preparación de reportes y mejorando la precisión de la información financiera.

---

**Autor:** Andrés Felipe Arteaga Cruz  
**Proyecto:** Automatización contable – MiningStore Systems  

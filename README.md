# Armado de Legajo para el Pago de Publicidad y Propaganda (RG66)

## Descripción del Proceso

1. **Descarga de Información desde SAP HANA S4**
   - **Transacción FBL3N (Mayor Contable)**: Se descarga la información correspondiente al mes a pagar.
   - **Transacción FS10N (Saldo Contable)**: Se descarga la información correspondiente al mes a pagar.
   - **Tabla LFA1**: Se descarga la razón social de cada proveedor.

2. **Armado del Cuadro de Retenciones**
   - Con los datos obtenidos de las transacciones y la tabla, se arma un cuadro que incluirá los datos relativos a cada retención practicada.
   - El monto detallado en este cuadro debe ser abonado a la AGIP.

## Detalles del Cuadro de Retenciones

- **Proveedor**: Razón social obtenida de la tabla LFA1.
- **Monto de la Retención**: Información obtenida de las transacciones FBL3N.
- **Fecha de la Retención**: Información obtenida de las transacciones FBL3N.
- **Concepto de la Retención**: Detalle del motivo de la retención.
- **Total a Abonar**: Suma de todas las retenciones a abonar a la AGIP.

## Notas Adicionales

- La automatizacion del proceso evita errores involuntarios al momento de manipular la informacion.
- Se reduce considerablemente el tiempo requerido para el armado del legajo

![](https://github.com/cgzanfa/Legajo_pago_AGIP_RG66/blob/main/Capturarg66.PNG)

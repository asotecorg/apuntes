# Pasos para instalación
  - Subir app.war al Tomcat
  - Ejecutar los script que se encuentra en las misma carpeta. scripts
  - En la sgf_prod_comision  poner valor de la comision a debitar en el campo  val_atm_ret_otrared 
  - En la sgf_tran insertar "NDCTR";"N/D Comision Transferencia Web";0;"A";"VT";"S";"ND COMI";"N";"A";"2101350500";"ND";"S";"";"S";"";"5490101100";"D";1;"S";"N";1;"";"";"N";"CC";"N";0;""
  -En la sgf_prod_comision debe quedar asi 1;0.00;0.31;0.31;0.00;0.00;0.04;0.04;0.00;0.31;0.76;0.66;0.00;0.04;0.11;0.09;0.00;0.00;0.45;0.35;0.00;0.00;0.06;0.05;0.00;0.00;0.00;0.00;0.00
  - Se debe insertar un empleado 99 y  en sgf_caja una caja 99 asignada con ese empleado.
  - Probar funciones con select coop_sp_nd(1, 10000061, '2020-4-3', 9);
  
  # Configurar los archivos properties.
   - Para conexiones y envio de mail en persistence.properties
   - Pra configuración de envio de sms config.properties
  

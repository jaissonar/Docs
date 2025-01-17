---

layout: default
title: Facturas
permalink: /Operacion/scm/pos/jcajero/jfac
editable: si

---



# Facturas - JFAC



**Menú**  



[Manual de Parametrización Exención de IVA en OasisCom](http://docs.oasiscom.com/Operacion/scm/pos/jcajero/Manual-de-Parametrización-Exención-de-IVA-en-OasisCom.pdf)![](http://docs.oasiscom.com/Mercadeo/fichas/Gift_new100gif.gif)  
Descargar PDF.  





* [JFAC - Facturas](http://docs.oasiscom.com/Operacion/scm/pos/jcajero/jfac#jfac---facturas)  
* [Liquidación por Vencimiento](http://docs.oasiscom.com/Operacion/scm/pos/jcajero/jfac#liquidación-por-vencimiento)  
* [Fidelización de clientes](http://docs.oasiscom.com/Operacion/scm/pos/jcajero/jfac#fidelización-de-clientes)    
* [Redimir puntos acumulados](http://docs.oasiscom.com/Operacion/scm/pos/jcajero/jfac#redimir-puntos-acumulados)  
* [Proceso de Packing](http://docs.oasiscom.com/Operacion/scm/pos/jcajero/jfac#proceso-de-packing)  
* [Cambios Mano a Mano](http://docs.oasiscom.com/Operacion/scm/pos/jcajero/jfac#cambios-mano-a-mano)  
* [Consulta Rápida de Terceros](http://docs.oasiscom.com/Operacion/scm/pos/jcajero/jfac#consulta-rápida-de-terceros)  
* [Facturación de combos](http://docs.oasiscom.com/Operacion/scm/pos/jcajero/jfac#facturación-de-combos)    
* [Redención de Puntos](http://docs.oasiscom.com/Operacion/scm/pos/jcajero/jfac#redención-de-puntos)     
* [Configuración Datafono](http://docs.oasiscom.com/Operacion/scm/pos/jcajero/jfac#configuración-datafono)   




## [**JFAC - Facturas**](http://docs.oasiscom.com/Operacion/scm/pos/jcajero/jfac#jfac---facturas)



Aplicación que permite elaborar facturas o devoluciones que se realicen en el punto de venta, estas son discriminadas por turnos para tener control sobre la cantidad de cajeros existentes.  



![](jfac2.png)



**Documento:** Documento parametrizado con anterioridad en el sistema. Este documento puede ser FA (Factura) o DE (Devolución).  

**Número:** Consecutivo de documento automático.  

**Ubicación:** Ubicación de punto de venta.  

**Fecha:** Fecha de registro de la factura.  

**Concepto:** Iniciales del concepto por el cual se desea realizar el documento Éste se debe parametrizar previamente en el sistema, en este caso el concepto puede ser FA (Factura) o DE (Devolución).  

**Motivo:**  Este se encuentra definido como 0.  

**Vendedor:** Número de identificación de la persona que se encuentra facturando.  

**Condición de Pago:** Representa un acuerdo establecido con clientes y proveedores en forma de tipos de descuento y plazos de pago, las diferentes opciones de condición de pago se encentran parametrizadas en la opción BCND.  

**Tipo de precio:** Precio debidamente parametrizado en la aplicación **FBTP**. Se presenta el siguiente escenario: guardo el maestro e inserto un producto en el detalle. Me devuelvo y cambio en el maestro el **Tipo Precio** el sistema lanza un mensaje de control indicando que debe de corregir el detalle así:  

![](jfac52.png)   

**Frecuente:** Cliente habitual, aplica para todos los puntos de venta de la compañía.  

![](jfac59.png)  

**Periodo:** Este campo se llena automaticamente, al insertar el registro.  

**Año:** Campo que se llena automaticamente, al insertar el registro.   

**Tercero:** Número de identificación del tercero al cual se carga el movimiento.   



En este se encuentran parametrizados tres tipos de Zooms que se visualizan al dar clic derecho. El primero es buscar cliente y el segundo crear tercero y por ultimo ir al tercero (BTER).  





![](jfac3.png)  

Damos ahora clic derecho en el campo de *Tercero,* en donde se desplegara un menu con tres opciones, para el caso del *Zoom de creación de Terceros,* damos clicen el *Segundo Elemento.*

**Despliega el siguiente formulario**.  



![](jfac4.png)  

Una vez damos clic en la segunda opción del menú de Zoom, vemos que se muestra una ventana tipo formulario en donde permite realizar acciones básicas, como son: Creación, Edición y Búsqueda de Terceros. 

1. *Nuevo Cliente:* Cuando damos clic en este botón se habilitara el formulario, para poder crear nuestro cliente, el botón cambiara de texto, para poder mostrar, luego damos clic en *Guardar cliente*  
2. *Editar Cliente:* Dando clic en este botón se habilitara un formulario, para poder editar nuestro cliente previamente consultado, el botón cambiara de texto para poder mostrar damos clic en el botón *Guardar Cliente*  
3. *Limpiar Formulario o Cancelar:* Permite realizar operaciones de limpieza del formulario y cancelaciones de alguna acción, como la creación, edición de algún tercero. 




**Filtros de busqueda**.  



![](jfac5.png)

Sobre el zoom de creación rápida de tercero, se agrega el campo de **teléfono** para que se pueda filtrar, así como evitar estar seleccionando el tipo de filtro, también se activa el evento de búsqueda al dar **enter.**  

![](jfac46.png)

**“Crear Cliente”**  



![](jfac6.png)



**Editar cada uno de los campos**.  



![](jfac7.png)



Al generarse el nuevo registro debemos diligenciar los siguientes campos cómo mínimo:  



En el caso que el registro nuevo sea de cliente, los campos requeridos son:  



* Tercero  

* Campos nombres y apellidos  

* Nombre Tercero  

* Tipo Cliente   

* Tipo de precio  



En caso que el cliente sea una empresa debemos tener en cuenta lo siguiente:  



* Tercero  

* Nombre Tercero  

* Tipo Cliente  

* Tipo de precio  

* Check digit  



![](jfac8.png)  



* Validamos el tercero creado en la opcion del BTER y vemos que quedo creado correctamente.  

* En esta creación rápida de terceros, campos obligatorios como teléfono, dirección, ubicación geográfica y demás, datos indispensables para el reporte de la información exógena a la DIAN.  

Para ingresar sobre la factura el cliente creado, se selecciona sobre el registro nuevo y automáticamente queda ingresado en el campo tercero del formulario JFAC - Facturas.  



Si se desea que el total de la factura tenga un porcentaje de descuento se debe ingresar en el campo **“% porcentaje”** y este hará el descuento en el valor total de la factura.  



Al realizar una factura en JFAC, es posible relacionar una solicitud de crédito realizada previamente en la aplicación **CSOL - Solicitudes de Crédito**, para ello, en el zoom _Número1_ seleccionaremos la solicitud que corresponda a la factura que se registra, este zoom permite ver el saldo de la solicitud del crédito para conocer el valor por el cual se puede realizar la factura.  



![](jfac23.png)



Posteriormente damos click sobre el botón _Guardar_.  



![](jfac11.png)  



* Cuando realizamos el guardado del maestro de la factura; el sistema lleva el cursor al primer renglón del producto, para seguir editando la factura insertando los productos y características de esta.  



![](bfor51.png)  

## [Vista Previa _Secundaria_](http://docs.oasiscom.com/Operacion/scm/pos/jcajero/jfac#vista-previa-detalle)  

En la botonera del maestro podemos encontrar el botón de vista previa para cuando se requiere visualizar documentos antes de imprimirlos o configurar las diferentes vistas que se requieran.
![](jfac83.png)  

Cuando damos clic nos muestra las vistas que se hayan configurado en la opción **[SPRO]**
![](jfac84.png)  

Como podemos visualizar en las dos siguientes imágenes de vistas previas el formato es diferente, esto depende del formato que se requiera utilizar para utilizar esta funcionalidad.
![](jfac85.png)  
![](jfac86.png)  

Por último, la parametrización se debe realizar en la opción **[SPRO]**, en la parte del Detalle tendremos que diligenciar los siguientes campos:

**Argumento:** Se debe colocar el procedimiento de donde se cargara la información del formato.
**Nombre:** Sera el nombre como se visualizara al momento de dar clic al botón de vista secundaria
**Defecto:** En este campo tendremos que colocar el comando ***js_SecondPreview***  para habilitar dicha funcionalidad.  
![](jfac87.png)  
**Esta configuración se puede utilizar para cualquier opción dentro de la aplicación.*

## [Pestaña _Detalle_](http://docs.oasiscom.com/Operacion/scm/pos/jcajero/jfac#pestaña-detalle)  


En la pestaña “Detalle” en la parte inferior de la aplicación, existe la opción de inserción de producto mediante el lector de código de barras, este funciona ubicándose en el campo producto y utilizando el lector se realiza la lectura del código de barras del producto, si dado el escenario: el producto ya fue registrado en otro renglon; el sistema realiza la suma del producto en el mismo renglon; de esta manera se registra la venta del producto y se completará la información en los campos Nombre Producto, Cantidad, Precio y %Descuento (Si aplica). Igualmente, en caso de no contar con el lector del código de barras en el campo producto se puede registrar manualmente el código del producto y al dar TAB se diligencian los campos de nombre de producto, cantidad precio y %Descuento (Si aplica), si el producto no trae asociado un % descuento, podemos ingresarlo manualmente y este se aplicará solo al producto al que se ingresó.  



![](jfac12.png)  



![](jfac13.png)  

### Integración con Balanzas.  

Se realiza la integración con 4 balanzas (marca: torrey, modelo pcs-35), con el objetivo: al pesar el sistema haga la lectura en el campo cantidad y registre el resultado de la unidad de medida peso, ejemplo en gramos y lo aplique en el campo **cantidad**, esto aplica tanto para el **IMOV** como para **JFAC**.  
Previa parametrizacion en WVAR (variables)y BUBI (ubicaciones).  

![](jfac13_01.png)  

* Existe una tercera pestaña denominada **PAGO.**  



En ella se almacena la forma de pago, la cual se parametriza en la aplicación **[BFOR]** , al tercero tipo cliente en el **[BTER]**.  

Para el escenario donde la forma de pago es mayor al precio de la factura existe el campo llamado **cambio**.  

El sistema calculará automáticamente el valor; lanzando un mensaje resaltado en azul, como se ilustra.  



![](jfac51.png)  





*****************************



* Existe una funcionalidad en el detalle del **JFAC** con el boton: 'saldos de inventarios en linea'.  

Se inserta el renglon nuevo en el detalle, con el producto y sus caracteristicas propias, se guarda y al dar click al boton:   

* Escenario uno: este emitira su saldo al final del renglon, siempre y cuando el saldo en linea sea inferior al que intenta facturar.   





![](jfac81.png)   



* Escenario dos: su saldo en linea permite realizar la transaccion, se mostrara en el campo QuantityInventory -1  indicando que existen saldos en linea para este producto.  

Detalle del **JFAC**.  



![](jfac82.png)







**********************



Existe una funcionabilidad al digitar Enter sobre uno de estos campos: Price (Precio), Quantity (Cantidad), Discount (Descuento), ProductId (Producto), Expiration (Vencimiento), DiscountPercentage (Porcentaje de Descuento) el sistema automáticamente habilitará el siguiente renglón del detalle, para proseguir insertando productos en el detalle de la factura.  



![](jfacc13.png)



## [Cambio de campos con credenciales](http://docs.oasiscom.com/Operacion/scm/pos/jcajero/jfac#cambio-de-campos-con-credenciales)



Esta funcionalidad permite al usuario la modificación de los campos _Precio_, _% Descuento_ y _Descuento_ cuando dichos campos estén bloqueados, donde pedirá credenciales de usuario y permita la modificación de los mismos.  



![](jfac24.png)



+ Parametrización



Para poder modificar dichos campos primero se debe realizar una parametrizacion en la opcion [**BRAN - Rangos**](http://docs.oasiscom.com/Operacion/common/btercer/bran), en donde por documento y por rol definimos que rangos de valores tiene permitido el usuario ingresar.   





![](bran.png)



El campo _Tipo_ tiene tres letras importantes con relación de los rangos permitidos en los campos, en donde consta de las siguientes caracteristicas:  



**P:** Precio

**D:** % Descuento

**V:** Descuento (valor)



Los campos de _Mínimo_ y _Máximo_ son los encargados de indicar los rangos permitidos que puede ingresar el rol asociado.  



Seguidamente, en la aplicación [**SROL - Roles**](http://docs.oasiscom.com/Operacion/system/sacceso/srol), en el detalle en la pestaña _Campos_, definimos que campos no serán editables, con el fin de que cuando se abra la aplicación y se inserte o actualice algún valor de los campos parametrizados, podamos realizar el funcionamiento de cambio de valor.  



![](jfac25.png)



En campo renglón, indicar a que tab queremos afectar, es decir, el **Renglón 0** afectará al maestro y el **Renglon 1** al primer tab del detalle, y así con los que se deseen.  



+ Proceso



Una vez realizadas las parametrizaciones en las anteriores aplicaciones, vamos a verificar el funcionamiento en la opcion **JFAC - Facturas**.  



En el siguiente ejemplo tomamos como referencia la factura: Documento: FA, Numero: 0, Almacen: 11.  



![](jfac26.png)



En el detalle que se ve editable, utilizaremos el campo de _Precio_, en donde el valor que actualmente tiene es de 123, ahora solo damos doble click sobre el campo y veremos que se muestra una modal solicitando credenciales de usuario.  



La autenticación del usuario solicitará el usuario y su contraseña, el sistema lo que hará una vez demos click en el botón _Aceptar_ es validar que el usuario exista, este usuario puede ser cualquiera al que inició sesion en la aplicación.  



![](jfac27.png)



Haremos un ejemplo del funcionamiento, en donde ingresaremos datos erroneos.  



![](jfac28.png)



El mensaje de error sólo valida que el usuario exista, más no que la contraseña esté correcta, pues no es necesario realizar una serie de validaciones a fondo ya que no es un inicio de sesion normal a la aplicación.  



![](jfac29.png)



Si utilizamos un usuario existente y damos click en _Aceptar_, se mostrará el mensaje de **Usuario Válido**. Una vez el sistema autentica el usuario, se visualizará otra pestaña en donde podremos realizar el cambio del valor de nuestro campo.  



![](jfac30.png)



El valor que ingresaremos será 3.5, donde al ser el campo de _Precio_ este restará el valor digitado.  



![](jfac31.png)



El valor que estaba en el campo _Precio_ era de 123 y con el valor de 3.5 quedará a 119.5.  



![](jfac32.png)



En el campo **% Descuento**, ingresaremos un valor de 123 en donde saldrá un error indicando que el valor no se encuentra en el rango permitido y mostrará los rangos Minimos y Maximos en los que se puede modificar.  



![](jfac33.png)



Si ingresamos un valor entre los rangos permitidos, el sistema dejará ingresar el valor al detalle.  



![](jfac34.png)



![](jfac35.png)



_**Nota:** En la opcion del BRAN - Rangos, se pueden parametrizar diferentes Rangos a diferentes Roles, pero si un usuario tiene más de un Rol, el sistema tomará el de menor jerarquía, es decir, si un usuario tiene el Rol 18, y el Rol 100, tomará la parametrización del Rol 18._  



## [Pestaña _Pago_](http://docs.oasiscom.com/Operacion/scm/pos/jcajero/jfac#pestaña-pago)



Permite realizar la modificación de la forma de pago de la factura, en el campo forma de pago se debe modificar la misma, puede ser efectivo, débito, crédito entre otros, esto se parametriza previamente en el sistema en la aplicación BFOR. Igualmente, en esta pestaña se puede consultar el valor de la factura y el impuesto del mismo.  



![](jfac14.png)



![](jfac15.png)



Si el cliente nos entrega un monto mayor al total de la factura y la forma de pago es “efectivo”, podemos visualizar el cambio, o como comúnmente es llamado “vueltas” en el campo del registro maestro “Cambio”, ingresando el monto inicial dado por el cliente en el campo total. Ejemplo:  



Tenemos nuestra factura por un valor de $50.170 y en estado activo.  



![](jfac16.png)



En el campo valor ingresaremos el monto que nos entrega el cliente y guardamos, en este caso el cliente nos dio la suma de $60.000.  



![](jfac17.png)



Por último, procesamos la factura y verificamos el campo cambio, que nos indicara el valor a devolver al cliente (Note que el campo _“valor”_, vuelve a su estado original: el valor total de la factura.)  



![](jfac18.png)



Si no se desea realizar el proceso de cambio, al terminar de realizar la factura, también se debe procesar el registro en el botón **_Procesar_**, este cambiará el estado de activo a procesado, indicando que la factura quedo terminada e impidiendo que sus datos sean modificados.  



![](jfac19.png)



Al procesar, el registro sobre el maestro se puede evidenciar los campos Valor Bruto, descuento, Subtotal, impuesto, Total, Neto y de la misma manera se encuentra un campo tipo Check con nombre impreso que nos indica si la factura ya fue procesada o no.  



![](jfac20.png)



**Nota:** Para realizar la impresión del Boucher de la factura se debe dar clic sobre el botón imprimir, teniendo en cuenta que el registro de factura debe estar procesado.  



![](jfac21.png)



![](jfac22.png)



En caso de tener parametrizada la forma de pago Nómina, se puede tener la opción de imprimir un voucher que nos indica el nombre del tercero y el valor a descontar por nómina, cómo se muestra a continuación.  Dando click sobre el botón “Imprimir Colilla”.  





## [Pestaña _Garantías_](http://docs.oasiscom.com/Operacion/scm/pos/jcajero/jfac#pestaña-garantías)



A través de esta pestaña el usuario podrá asignar garantías a los productos facturados en el maestro.  



Creamos un nuevo registro y diligenciamos los datos, seguidamente



![](jfac1.png)





## [Liquidación por Vencimiento](http://docs.oasiscom.com/Operacion/scm/pos/jcajero/jfac#liquidación-por-vencimiento)



Esta funcionalidad realiza la liquidación de diferentes precios de un mismo producto con base a los vencimientos que este tenga. Esto, con previa parametrización en las opciones [**WVAR - Variables**](http://docs.oasiscom.com/Operacion/dss/bsc/wbasica/wvar#parametrización-liquidación-por-vencimiento) y [**FDES - Descuentos**](http://docs.oasiscom.com/Operacion/scm/facturacion/fprecio/fdes#parametrización-liquidación-por-vencimiento). (_Ver aplicaciones_)  



Al crear una factura en JFAC e ingresar al zoom para seleccionar el producto, podremos ver que según las fechas de vencimiento el sitema tomó el descuento.  



![](jfac36.png)





![](jfac37.png)





## [Fidelización de clientes](http://docs.oasiscom.com/Operacion/scm/pos/jcajero/jfac#fidelización-de-clientes)



El proceso de _Fidelización de Clientes_ permite que por cada compra que realice un cliente, este acumule puntos que podrá redimir en una próxima compra.  



+ Parametrización



Inicialmente se requiere hacer la siguiente parametrización.  



[**BTER - Terceros**](http://docs.oasiscom.com/Operacion/common/btercer/bter#parametrizaci%C3%B3n-fidelizaci%C3%B3n-de-clientes)  



En la aplicación **BTER** se deben registrar los clientes que podrán acumular puntos. En el momento del registro, se deberá marcar el flag _**Frecuente**_ ubicado en la pestaña del detalle llamada _Ventas_, esto permitirá al sistema identificar que por cada compra que realice dicho cliente, este acumulará puntos.  



![](jfac38.png)



[**FDES - Descuentos**](http://docs.oasiscom.com/Operacion/scm/facturacion/fprecio/fdes#parametrizaci%C3%B3n-fidelizaci%C3%B3n-de-clientes)



![](jfac39.png)



En la aplicación **FDES** se deberá crear un registro correspondiente a _Tarifa Puntos_, en el cual indicaremos el rango de **fecha inicial** y **fecha final** en el cual aplicará la adquisición de puntos por compras. Por ejemplo, el cliente podrá adquirir puntos por sus compras desde el 4 de julio del 2018 hasta el 31 de julio del 2018.  



![](jfac40.png)



También se deberá registrar en el campo **Tarifa** el valor que definirá cada cuanto acumularán puntos los clientes y en el campo **Tariff Substraction** se indica la cantidad de puntos que adquirirá de acuerdo con la tarifa. Por ejemplo, por cada 100 pesos del valor de la compra, el cliente acumulará un punto, es decir, que si un cliente hace una compra de 1.000 pesos tendrá 10 puntos.  



![](jfac41.png)





[**BFOR - Descuentos**](http://docs.oasiscom.com/Operacion/common/bcomer/bfor#parametrización-fidelización-de-clientes)



En la aplicación **BFOR** se debe parametrizar la forma de pago _Redención Puntos_, la cual se asignará como forma de pago en la compra del cliente que quiera usar sus puntos acumulados.  



![](jfac42.png)



**Forma Pago:** ingresar el consecutivo que corresponda teniendo en cuenta las formas de pago ya registradas.  

**Nombre forma pago:** asignar el nombre _Redención Puntos_.  

**Tipo:** seleccionar el tipo _Puntos_.  

**Código:** ingresar el código _PUR_.  



* Las formas de pago **tipo puntos** para su redención, valida la cuenta contable correspondiente y **saldos en puntos de fidelización de clientes** por diferentes cuentas contables.  





+ Proceso Fidelización de Clientes  



De acuerdo con la parametrización anterior, en la aplicación **JFAC** se realizará la factura de venta al cliente registrado en la aplicación [**BTER - Terceros**](http://docs.oasiscom.com/Operacion/common/btercer/bter#parametrizaci%C3%B3n-fidelizaci%C3%B3n-de-clientes).  



El valor de la venta fue de 1.786 pesos, es decir, que el cliente acumuló 17 puntos.  



![](jfac43.png)



Seguidamente, ingresamos a la aplicación [**ASSP - Saldos de Clientes**](http://docs.oasiscom.com/Operacion/crm/mercadeo/wfidelizacion/assp#fidelizaci%C3%B3n-de-clientes) a verificar los puntos acumulados.  





## [Redimir puntos acumulados](http://docs.oasiscom.com/Operacion/scm/pos/jcajero/jfac#redimir-puntos-acumulados)



Si un cliente desea redimir sus puntos acumulados o una parte de ellos en alguna compra, se debe crear normalmente la factura de venta en la aplicación **JFAC** y en la pestaña del detalle _Pago_ ingresar un renglón en donde la forma de pago sea _PUNTOS_.  



A continuación, veremos un ejemplo en donde la compra realizada por el cliente tiene un valor subtotal de $700.  



![](jfac44.png)



Ahora en la pestaña _Pago_ ingresaremos la forma de pago _PUNTOS_ en la cual se indicará la cantidad de puntos que desea redimir el cliente para esa compra. En caso de que la cantidad de puntos no cubra el total del valor de la factura, se debe ingresar la(s) otra(s) formas de pago con las cuales se completará el pago.  



En el siguiente ejemplo el cliente redimirá 100 puntos, estos son ingresados en el campo **Valor**. Como la venta era por un total de $833, el sistema creó la forma de pago _EFECTIVO_ con el saldo restante teniendo en cuenta la condición de pago ingresada en el maestro la cual era _CONTADO_.  





![](jfac45.png)



Finalmente, se procesa la factura y se verifican los saldos de puntos acumulados en la aplicación [**ASSP - Saldos de Clientes**](http://docs.oasiscom.com/Operacion/crm/mercadeo/wfidelizacion/assp#saldo-al-redimir-puntos-acumulados) para el cliente correspondiente. Vale aclarar que como el cliente redimió solo 100 puntos en el ejemplo anterior y tuvo que pagar el restante que eran $733, obtuvo 7 puntos más.  



Verificamos el nuevo saldo de puntos acumulados en [**ASSP - Saldos de Clientes**](http://docs.oasiscom.com/Operacion/crm/mercadeo/wfidelizacion/assp#saldo-al-redimir-puntos-acumulados).  



* Se incluye la funcionalidad de contabilizacion de puntos en la fidelizacion de clientes, para esto se debe tener presente la siguiente configuracion:   

1. Es necesario crear el código de cuenta VPU e incluirlo en el **BPLA** para la contabilización en otorgación de puntos.  

2. Marcar las cuentas contables en el **BCUE** en el campo QuantityType la opción valor contabilidad.  

Estas ya se encuentran marcadas por BD, se encontrara disponible el ListBox.  



Aquí finaliza el proceso de _fidelización de clientes_.   

## [Proceso de Packing](http://docs.oasiscom.com/Operacion/scm/pos/jcajero/jfac#proceso-de-packing)  

Para realizar la respectiva parametrización y proceso que se realizaba en la aplicación EITRA –desde la aplicación JFAC – Facturas, a continuación, se describe procedimiento de cómo realizar la parametrización y como es su funcionalidad. 

### Parametrización 
-	Aplicación SCAM, se debe configurar el botón que aparecerá en el detalle de la aplicación JFAC – Factura que contiene las siguientes características. 

 ![](produv.png)
 
-	Aplicación WVAR – Variables, en esta aplicación se deben configurar las respectivas variables.   

![](produv2.png)

 Luego de la anterior configuración, el sistema nos mostrara en la aplicación JFAC en la parte superior del detalle un botón, la principal funcionalidad de este botón es para que en esta aplicación se puedan generar pedidos o diferentes tipos de documentos el cual ya contienen productos a despachar o a vender, el objetivo es que los productos que se vayan a utilizar a nivel del detalle, la mayoría va a ser de un pedido previamente realizado, es decir relacionado un documento en el maestro de la factura.   
 
 ![](produv1.png)
 
 A nivel del detalle de los pedidos, el cual ya contiene algunos productos a despachar o a vender, los productos que se vayan a utilizar a nivel de detalle, la mayoría van a ser de algún pedido previamente realizado, la aplicación VPED ya cuenta con unos productos precargados.   
 
![](produv3.png)

El objetivo principal es el embalaje o empaque de estos productos en cajas, para realizar el proceso se debe dar clic en el icono de *Picking – Facturas* que se encuentra en la parte superior del detalle, como se evidencia es el mismo proceso de la aplicación EITRA. Aquí se pueden visualizar y posteriormente dividirlos en las respectivas cajas, es decir si se requiere que en el renglón 1 el producto cuenta con 2 unidades, pero se necesita que sean despachados en cajas diferentes, en el botón de color verde haciendo clic en el sistema nos traerá una ventana emergente donde se indicara cuantas unidades irán en cada caja.      

![](produv4.png)

![](produv5.png)

Cuando la aplicación no muestre las opciones descritas anteriormente, el objetivo de ellas es verificar con código de barras que se encuentra la opción en la parte superior. El sistema lo que realiza es buscar el producto que encuentra con el código de barras y lo va a insertar en la parte derecha. Luego de culminar el proceso anterior se debe dar clic en terminar empaque.    

![](produv6.png)


## [Cambios Mano a Mano](http://docs.oasiscom.com/Operacion/scm/pos/jcajero/jfac#cambios-mano-a-mano)


Para realizar la respectiva parametrización y proceso desde la aplicación **JFAC** (Facturas), a continuación, se describe procedimiento de cómo realizar la parametrización y como es su funcionalidad. 

### Parametrización 
-	Para realizar la configuración de la funcionalidad de cambios mano a mano, se debe parametrizar el botón de cambio mano a mano, desde la opción **SCAM**, donde se especifica que es tipo botón y que ejecutara el método de javascript. 

 ![](jfac54.png)


**Programa:** jfac  
**FieldID:** btnInfo1  
**Nombre:** Cambio Mano a Mano  
**Descripcion:** js_HandToHandExchange  
**Defecto:** Cambio Mano a Mano  
**Condicion:**  ui-icon-transfer-e-w  
**Tipo:** Boton  

Luego de la parametrización de **SCAM**, el botón estará disponible en la opción deseada. sobre la cual se hace clic y se desplegara la ventana de cambios.

![](jfac56.png)

En la ventana de cambios se buscan los productos a intercambiar, se seleccionan desde los listados y se especifica la cantidad a intercambiar. luego se hace clic en el botón aceptar y se ejecuta el proceso de cambio.

![](jfac55.png)

Por último, el cambio se podrá ver reflejado en la opción **ICNV**
![](jfac57.png)


## [Consulta Rápida de Terceros](http://docs.oasiscom.com/Operacion/scm/pos/jcajero/jfac#consulta-rápida-de-terceros)

Lo primero que hacemos es abrir la opción **JFAC** y dar clic al botón *Consulta Tercero*
![](jfac47.png)

Luego de esto nos abre la ventana de *Consulta Rápida - terceros* en el cual podemos realizar 2 tipo de filtro ya sea por numero de documento.
![](jfac48.png)
![](jfac49.png)

Ó por el nombre del tercero.
![](jfac50.png)
![](jfac60.png)

Por otra parte, al realizar el filtro nos trae todos los terceros que coincidan con documento o nombre correspondiente y podremos movernos con las flechas de anterior y siguiente.
![](jfac61.png)

## [Facturación de combos](http://docs.oasiscom.com/Operacion/scm/pos/jcajero/jfac#facturación-de-combos)    

Para realizar la facturación de los combos primero se debe parametrizar el producto y sus componentes en la aplicación BPRO.  

![](combo.png)

![](combo1.png)

Posteriormente deben crear una factura en la aplicación JFAC, al momento de la adición de producto posteriormente guardarlo, el sistema traerá en el detalle cada uno de los productos que tiene un combo.   

![](combo2.png)

En la aplicación FPRE, cada uno de esos productos debe estar previamente creado y con su valor correspondiente.   

![](combo3.png)

## [Redención de Puntos](http://docs.oasiscom.com/Operacion/scm/pos/jcajero/jfac#redención-de-puntos)   

Cálculo de grados de fidelidad por asociado y ajuste al proceso de acumulación y/o registro de puntos para efectos de redención como forma de pago en las facturas de venta.   

### Parametrización 

La categorización o membresía por asociado se tomara del campo ABC que la calificación del tercero.   

![](punto.png)

El tercero debe estar marcado en la aplicación BTER como frecuente.  

![](punto1.png)

Con ello la calificación correspondiente.  

![](punto2.png)

El comportamiento de los puntos a obtener y redimir se configura en FDES con la jerarquía de la calificación que corresponda.  Adicional para los casos en que la obtención de puntos depende de los kilos facturados en OCAF se configura por medio de la columna Descripción.  también se deben configurar tantos FDES sean necesarios por las diferentes combinaciones para otorgar puntos.  

![](punto3.png)

Configurados los FDES por cada compra de café o venta en JFAC y FFAC que cumplan con la configuración del FDES otorgara los puntos pertinentes.   

![](punto4.png)

Adicional para la redención de puntos se debe configurar la forma de pago puntos y asociarla en la forma de pago pertinente.   

![](punto5.png)

Para redimir u obtener puntos tanto en OCAF como JFAC o FFAC se deben configurar los códigos de cuenta pertinentes en BPLA para la validación del sistema.   

![](punto7.png)

Para el proceso automático del cálculo del BABC se realiza por medio del WCAL, se configura la estrategia 101 para actualizar masivamente por medio de variables configurables.  Este punto se está trabajando directamente con el cliente para aclarar cálculo de algunos porcentajes.  

![](punto8.png)

Ejemplo de como redmimir los puntos.  

![](punto6.png)


## [Configuración Datafono](http://docs.oasiscom.com/Operacion/scm/pos/jcajero/jfac#configuración-datafono)   

### Parametrización 

En la aplicación BFOR se debe especificar qué tipo es y diligenciar el campo datafono para que el sistema lo reconozca.   

![](datafono.png)

En la aplicación SCAM, se debe realizar la respectiva parametrización de este campo.  

![](datafono1.png)

Posteriormente, en la aplicación JFAC luego de crear la factura y diligenciar los respectivos productos, en la pestaña pago elegir la forma de pago Tarjeta, luego clic en procesar.   

![](datafono4.png)

Luego de que el datafono ya reconozca el pago y sea debitado de la cuenta, el sistema construye los valores que son el número de autorización, los números de la tarjeta y lo deja en estado procesado.   

![](datafono5.png)

Luego se debe verificar si el pago efectivamente quedo en la aplicación EPAY. 

![](datafono3.png)

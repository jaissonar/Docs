---
layout: default
title: Facturacion
permalink: /Operacion/is/hospital/gfacturacion/gfac
editable: si
---

# Facturas - GFAC


* [Verificación parametrización Tipo de Precio](http://docs.oasiscom.com/Operacion/is/hospital/gfacturacion/gfac#verificación-parametrización-tipo-de-precio)
* [Consultas dinámicas](http://docs.oasiscom.com/Operacion/is/hospital/gfacturacion/gfac#consultas-dinámicas)
* [Detalle](http://docs.oasiscom.com/Operacion/is/hospital/gfacturacion/gfac#detalle)



## [Verificación parametrización Tipo de Precio](http://docs.oasiscom.com/Operacion/is/hospital/gfacturacion/gfac#verificación-parametrización-tipo-de-precio)

Realizada la parametrización de tipo de precio en la aplicación [**BUBI - Ubicaciones Organización**](http://docs.oasiscom.com/Operacion/common/borgan/bubi), podemos validar en la aplicación **GFAC**, que al agregar un nuevo registro e ingresar en el campo _Ubicación_, la ubicación  en la cual se realizó la parametrización, este trae automáticamente en el campo _Tipo de Precio_ el definido en la aplicación [**BUBI - Ubicaciones Organización**](http://docs.oasiscom.com/Operacion/common/borgan/bubi).  

* Con clic derecho, permite crear nuevos afiliados desde el **GMOV, GFAC** como se tiene actualmente la creación desde el **JFAC.**  

![](gfac5.png)


En cuanto a la aplicación **GMOV**  lo único que cambia es el formulario para creación de doctores es más simple que el de crear cliente, por lo demás cuenta con las mismas funcionalidades.

![](gmov.png)


* Al crear un registro, por defecto muestra la ubicación _0_ con el tipo de precio designado para esta como se muestra en la imagen.  

![](gfac.png)

Si se cambia la ubicación por la parametrizada en la opción [**BUBI - Ubicaciones Organización**](http://docs.oasiscom.com/Operacion/common/borgan/bubi), es decir, la ubicación _1_, debe enseñar el tipo de precio parametrizado en esta opción.  

![](gfac1.png)

## [Consultas dinámicas](http://docs.oasiscom.com/Operacion/is/hospital/gfacturacion/gfac#consultas-dinámicas)

Realización de una consulta dinámica en la aplicación _GFAC - Facturas_.  

![](gfac2.png)

## [Detalle](http://docs.oasiscom.com/Operacion/is/hospital/gfacturacion/gfac#detalle) 

* Existe una funcionabilidad en el detalle del **GFAC** con el boton: 'saldos de inventarios en linea'. 
Se inserta el renglon nuevo en el detalle, con el producto y sus caracteristicas propias, se guarda y al dar clic al boton:  
* Escenario uno: este emitira su saldo al final del renglon, siempre y cuando el saldo en linea sea inferior al que intenta facturar.  


![](gfac3.png)

* Escenario dos: su saldo en linea permite realizar la transaccion, se mostrara en el campo QuantityInventory -1  indicando que existen saldos en linea para este producto.  
Detalle del **GFAC**.  

![](gfac4.png)


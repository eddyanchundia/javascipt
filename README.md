
<html>
<center><h3> FACTURACION DE AUTOS</h3></center>

<script>
    function soloLetras(e){
       key = e.keyCode || e.which;
       tecla = String.fromCharCode(key).toLowerCase();
       letras = " Ã¡Ã©Ã­Ã³ÃºabcdefghijklmnÃ±opqrstuvwxyz";
       especiales = [8,37,39,46];

       tecla_especial = false
       for(var i in especiales){
            if(key == especiales[i]){
                tecla_especial = true;          
			break;
            }
        }
		        if(letras.indexOf(tecla)==-1 && !tecla_especial){
            			return false;
			        }
    }
</script>

Nombres del cliente <input type="text" onkeypress="return soloLetras(event)"><br><br>

<script type="text/javascript">
function Solo_Numerico(variable){
Numer=parseInt(variable);
if (isNaN(Numer)){
return "";
}
return Numer;
}
function ValNumero(Control){
Control.value= Solo_Numerico(Control.value);
}

</script>
Numero de Cedula<input type="text" onkeyup="return ValNumero(this);"><br><br>

Fecha <input type="text"  maxlength="15" name="fecha"> &nbsp &nbsp &nbsp &nbsp &nbsp


<!-- menu desplegable de descuento -->
 
 &nbsp &nbsp  &nbsp &nbsp  
 
<form name="saldos">
 &nbsp &nbsp Item &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp&nbsp &nbsp &nbsp &nbsp &nbsp &nbsp&nbsp &nbsp &nbsp &nbsp &nbsp Cantidad &nbsp &nbsp &nbsp Valor  &nbsp &nbsp  Subtotal<br>

<input type="text" size="25" maxlength="15" name="detalle1"> <input type="text" size="5" maxlength="4" name="cantidad1" onfocus="sum()"> <input type="text" size="5" maxlength="4" name= "valor1" onfocus="sum()"> <input type="text" size="5" maxlength="4" name="subtotal1"><br>
<input type="text" size="25" maxlength="15" name="detalle2"> <input type="text" size="5" maxlength="4" name="cantidad2" onfocus="sum()"> <input type="text" size="5" maxlength="4" name="valor2" onfocus="sum()"> <input type="text" size="5" maxlength="4" name="subtotal2"><br>
<input type="text" size="25" maxlength="15" name="detalle3"> <input type="text" size="5" maxlength="4" name="cantidad3" onfocus="sum()"> <input type="text" size="5" maxlength="4" name="valor3" onfocus="sum()"> <input type="text" size="5" maxlength="4" name="subtotal3"><br>
<input type="text" size="25" maxlength="15" name="detalle4"> <input type="text" size="5" maxlength="4" name="cantidad4" onfocus="sum()"> <input type="text" size="5" maxlength="4" name="valor4" onfocus="sum()"> <input type="text" size="5" maxlength="4" name="subtotal4"><br>
<input type="text" size="25" maxlength="15" name="detalle5"> <input type="text" size="5" maxlength="4" name="cantidad5" onfocus="sum()"> <input type="text" size="5" maxlength="4" name="valor5" onfocus="sum()"> <input type="text" size="5" maxlength="4" name="subtotal5"><br>
<br>

<script>
function sum()
{
var v1;
var v2;
var res1;

var v3;
var v4;
var res2;

var v5;
var v6;
var res3;

var v7;
var v8;
var res4;

var v9;
var v10;
var res5;

v1=document.forms["saldos"]["cantidad1"].value;
v2=document.forms["saldos"]["valor1"].value;
res1=v1*v2;
document.forms["saldos"]["subtotal1"].value=res1;

v3=document.forms["saldos"]["cantidad2"].value;
v4=document.forms["saldos"]["valor2"].value;
res2=v3*v4; 
document.forms["saldos"]["subtotal2"].value=res2;


v5=document.forms["saldos"]["cantidad3"].value;
v6=document.forms["saldos"]["valor3"].value;
res3=v5*v6; 
document.forms["saldos"]["subtotal3"].value=res3;

var parc;
parc= res1+ res2 + res3;

}

</script>

</BODY> 

</HTML> 


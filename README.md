javascript
<html>
<center><h3> Sistematizacion de factura</h3></center>


<!-- menu desplegable de descuento -->

&nbsp 

<br>

<fieldset style="width:500px;background: #115461;">
<form name="saldos">
 &nbsp &nbsp Item &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp&nbsp &nbsp &nbsp &nbsp &nbsp &nbsp&nbsp &nbsp &nbsp &nbsp &nbsp Cantidad &nbsp &nbsp &nbsp Valor  &nbsp &nbsp  Subtotal<br>

<input type="text" size="25" maxlength="15" name="detalle1"> <input type="text" size="5" maxlength="4" name="cantidad1" onfocus="sum()"> <input type="text" size="5" maxlength="4" name= "valor1" onfocus="sum()"> <input type="text" size="5" maxlength="4" name="subtotal1"><br>
<input type="text" size="25" maxlength="15" name="detalle2"> <input type="text" size="5" maxlength="4" name="cantidad2" onfocus="sum()"> <input type="text" size="5" maxlength="4" name="valor2" onfocus="sum()"> <input type="text" size="5" maxlength="4" name="subtotal2"><br>
<input type="text" size="25" maxlength="15" name="detalle3"> <input type="text" size="5" maxlength="4" name="cantidad3" onfocus="sum()"> <input type="text" size="5" maxlength="4" name="valor3" onfocus="sum()"> <input type="text" size="5" maxlength="4" name="subtotal3"><br>
<br>

&nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp  &nbsp &nbsp &nbsp subtotal :  <input type="text" name="parcial"> <br> 
&nbsp &nbsp &nbsp &nbsp &nbsp &nbsp  &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp&nbsp&nbsp&nbspIva: <input type="text" name="iva"> <br> 
&nbsp  &nbsp &nbsp  &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbspDescuento: <input type="text" name="descuento"> <br>
&nbsp  &nbsp &nbsp  &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp Total:&nbsp<input type="text" name="total"> <br>


</html>


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
parc= res1+ res2 + res3 + res4 + res5 + res6 + res7 + res8 + res9 + res10; 

document.forms["saldos"]["parcial"].value=parc;

var iva;
iva=parc*0.12;
document.forms["saldos"]["iva"].value=iva;


var tot;
tot= parc + iva - des;
document.forms["saldos"]["total"].value=tot; 

}
</script>


<script>
function sum1()
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

var v11;
var v12;
var res6;

var v13;
var v14;
var res7;

var v15;
var v16;
var res8;

var v17;
var v18;
var res9;

var v19;
var v20;
var res10;

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

v7=document.forms["saldos"]["cantidad4"].value;
v8=document.forms["saldos"]["valor4"].value;
res4=v7*v8; 
document.forms["saldos"]["subtotal4"].value=res4;

v9=document.forms["saldos"]["cantidad5"].value;
v10=document.forms["saldos"]["valor5"].value;
res5=v9*v10; 
document.forms["saldos"]["subtotal5"].value=res5;

v11=document.forms["saldos"]["cantidad6"].value;
v12=document.forms["saldos"]["valor6"].value;
res6=v11*v12; 
document.forms["saldos"]["subtotal6"].value=res6;

v13=document.forms["saldos"]["cantidad7"].value;
v14=document.forms["saldos"]["valor7"].value;
res7=v13*v14; 
document.forms["saldos"]["subtotal7"].value=res7;

v15=document.forms["saldos"]["cantidad8"].value;
v16=document.forms["saldos"]["valor8"].value;
res8=v15*v16; 
document.forms["saldos"]["subtotal8"].value=res8;


v17=document.forms["saldos"]["cantidad9"].value;
v18=document.forms["saldos"]["valor9"].value;
res9=v17*v18; 
document.forms["saldos"]["subtotal9"].value=res9;


v19=document.forms["saldos"]["cantidad10"].value;
v20=document.forms["saldos"]["valor10"].value;
res10=v19*v20; 
document.forms["saldos"]["subtotal10"].value=res10;

var parc;
parc= res1+ res2 + res3 + res4 + res5 + res6 + res7 + res8 + res9 + res10; 

document.forms["saldos"]["parcial"].value=parc;

var iva;
iva=parc*0.12;
document.forms["saldos"]["iva"].value=iva;

var des;
des=parc*0.15;
document.forms["saldos"]["descuento"].value=des;


var tot;
tot= parc + iva - des;
document.forms["saldos"]["total"].value=tot; 

}
</script>

<script>
function sum2()
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

var v11;
var v12;
var res6;

var v13;
var v14;
var res7;

var v15;
var v16;
var res8;

var v17;
var v18;
var res9;

var v19;
var v20;
var res10;

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

v7=document.forms["saldos"]["cantidad4"].value;
v8=document.forms["saldos"]["valor4"].value;
res4=v7*v8; 
document.forms["saldos"]["subtotal4"].value=res4;

v9=document.forms["saldos"]["cantidad5"].value;
v10=document.forms["saldos"]["valor5"].value;
res5=v9*v10; 
document.forms["saldos"]["subtotal5"].value=res5;

v11=document.forms["saldos"]["cantidad6"].value;
v12=document.forms["saldos"]["valor6"].value;
res6=v11*v12; 
document.forms["saldos"]["subtotal6"].value=res6;

v13=document.forms["saldos"]["cantidad7"].value;
v14=document.forms["saldos"]["valor7"].value;
res7=v13*v14; 
document.forms["saldos"]["subtotal7"].value=res7;

v15=document.forms["saldos"]["cantidad8"].value;
v16=document.forms["saldos"]["valor8"].value;
res8=v15*v16; 
document.forms["saldos"]["subtotal8"].value=res8;


v17=document.forms["saldos"]["cantidad9"].value;
v18=document.forms["saldos"]["valor9"].value;
res9=v17*v18; 
document.forms["saldos"]["subtotal9"].value=res9;


v19=document.forms["saldos"]["cantidad10"].value;
v20=document.forms["saldos"]["valor10"].value;
res10=v19*v20; 
document.forms["saldos"]["subtotal10"].value=res10;

var parc;
parc= res1+ res2 + res3 + res4 + res5 + res6 + res7 + res8 + res9 + res10; 

document.forms["saldos"]["parcial"].value=parc;

var iva;
iva=parc*0.12;
document.forms["saldos"]["iva"].value=iva;

var des;
des=parc*0.25;
document.forms["saldos"]["descuento"].value=des;


var tot;
tot= parc + iva - des;
document.forms["saldos"]["total"].value=tot; 

}
</script>


<script>
function sum3()
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

var v11;
var v12;
var res6;

var v13;
var v14;
var res7;

var v15;
var v16;
var res8;

var v17;
var v18;
var res9;

var v19;
var v20;
var res10;

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

v7=document.forms["saldos"]["cantidad4"].value;
v8=document.forms["saldos"]["valor4"].value;
res4=v7*v8; 
document.forms["saldos"]["subtotal4"].value=res4;

v9=document.forms["saldos"]["cantidad5"].value;
v10=document.forms["saldos"]["valor5"].value;
res5=v9*v10; 
document.forms["saldos"]["subtotal5"].value=res5;

v11=document.forms["saldos"]["cantidad6"].value;
v12=document.forms["saldos"]["valor6"].value;
res6=v11*v12; 
document.forms["saldos"]["subtotal6"].value=res6;

v13=document.forms["saldos"]["cantidad7"].value;
v14=document.forms["saldos"]["valor7"].value;
res7=v13*v14; 
document.forms["saldos"]["subtotal7"].value=res7;

v15=document.forms["saldos"]["cantidad8"].value;
v16=document.forms["saldos"]["valor8"].value;
res8=v15*v16; 
document.forms["saldos"]["subtotal8"].value=res8;


v17=document.forms["saldos"]["cantidad9"].value;
v18=document.forms["saldos"]["valor9"].value;
res9=v17*v18; 
document.forms["saldos"]["subtotal9"].value=res9;


v19=document.forms["saldos"]["cantidad10"].value;
v20=document.forms["saldos"]["valor10"].value;
res10=v19*v20; 
document.forms["saldos"]["subtotal10"].value=res10;

var parc;
parc= res1+ res2 + res3 + res4 + res5 + res6 + res7 + res8 + res9 + res10; 

document.forms["saldos"]["parcial"].value=parc;

var iva;
iva=parc*0.12;
document.forms["saldos"]["iva"].value=iva;

var des;
des=parc*0.50;
document.forms["saldos"]["descuento"].value=des;




var tot;
tot= parc + iva - des;
document.forms["saldos"]["total"].value=tot; 


}
</script>


</fieldset>

javascript

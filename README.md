validar
=======
 <!DOCTYPE HTML>
<img src=".\faccii.jpg" /><br>
TOBAR BRIONES MARVIN ANDRES<BR>
3 NIVEL "A"<BR>
PROGRAMACION APLICADA A LA WEB
 <html>
<head>
<title>Averigua si un números es primo</title>
<script LANGUAGE="JavaScript">


function calculate(form) {
var num=parseInt(form.number.value);
if (isNaN(num) || num < 0) {
form.result.value=(form.number.value + " is not a valid number!  Try again!");
}
if (num == 1 || num == 2) {
form.result.value=(num + " is prime!");
}
for (var i=2;i<num;i++) {
if (num % i == 0) {
var prime="yes";
form.result.value=(num + " no es primo, es divisible por " + i + ".");
break;
}
if (num % i != 0) var prime="no";
}
if (prime == "no") form.result.value=(num + " es primo.");
} 
// End -->
</script>
</head>

<body>

<center>
<form name="form">
  <h2><font size="3">Averigua si un número es primo</font></h2>
  <p>Por favor entra un número:<br>
  <input type="text" name="number" size="7">
  <input type="button" value="Calcular" onClick="calculate(this.form)"> </p>
  <p><input type="text" name="result" size="45" value> </p>
</form>
</center>
<p></p>
<center>
<p>&nbsp;</p>
</center>
<p></p>


</body>

</html>



<html>
<head>
<title>Datos hexadecimal</title>
<script lenguaje="JavaScript">
function cadec(tabla) {
hex=tabla.valorhex.value;
hex=hex.toUpperCase()
lon=hex.length;
simbolos="0123456789ABCDEF";
dec=0;
for (i=0; i<lon; i++)
	{
	caracter=hex.substring(i,i+1);
	for (j=0; j<16; j++) {
		if (caracter==simbolos.charAt(j)) {valcar=j;}
		}
	dec=dec+valcar*Math.pow(16,lon-i-1);
	}
tabla.valorhex.value=hex;
tabla.valordec.value=dec;
}
function cahex(tabla) {
dec=eval(tabla.valordec.value);
coc=1;
res=0;
hex=" ";
simbolos="0123456789ABCDEF";
while(coc>0)
	{
	coc=Math.floor(dec/16);
	res=dec-coc*16;
	hex=simbolos.charAt(res)+hex;
	dec=coc;
	}


tabla.valorhex.value=hex;
}

function cabin(tabla){

}

// Fin -->

</script>
</head>
<body>
<p align="center"><b><font size="6"> decimal-hexadecimal</font></b></p>
<p align="center">&nbsp;</p>
<div align="center">
  <center>
  <form name="tabla">
  <table border="0" cellspacing="10" cellpadding="5">
    <tr>
      <td rowspan="2">
        <p align="center"><font size="4">Hexadecimal<br>
        </font><input type="text" name="valorhex" size="20"></p>
      </td>
      <td valign="baseline" align="center">
      </td>
      <td rowspan="2">
        <p align="center"><font size="4">Decimal<br>
        </font><input type="text" name="valordec" size="20"></p>
      </td>
    </tr>
    <tr>
      <td valign="baseline" align="center">
      
      </td>
    </tr>
    <tr>
      <td valign="middle" align="center">
        <p align="center">
      <input type="button" value="Convertir  a  decimal" onClick="cadec(this.form)">
      </td>
      <td valign="middle" align="center">
        <input type="Reset" value="Borrar">
      </td>
      <td valign="middle" align="center">
        <input type="button" value="Convertir a hexadecimal" onClick="cahex(this.form)">
      </td>
    </tr>
    
  </table>
  </form>
  </center>
</div>
</body>
</html>





<html>
<head>
<title>
</title>
   <script language="javascript" type="text/javascript">
       
        function Solo_Numerico(variable){
            Numer=parseInt(variable);
            if (isNaN(Numer)){
                return "";
            }
            return Numer;
        }
        function ValNumero(Control){
            Control.value=Solo_Numerico(Control.value);
        }
    </script>
     
</head>
<body>
<h3>ingresar numero de cedula</h3>
<center>Cedula: <input type=text name=Cedula onkeyUp="return ValNumero(this);" maxlength="10" size="24"  /></center>
</body>
</html>




<html>
<head>
<title>sumar dos numeros</title>
<script type="text/javascript" language="javascript">
		function sumarDosNumeros()
		{
		   var n1=0
   		var n2=0
   		var rsultado=0
		n1=parseInt(prompt("digite su numero"))
		n2=parseInt(prompt("digite su numero"))
		resultado= n1+n2
		alert("la suma de "+n1+"+"+n2+" ="+resultado)
		}


</script>
<script type="text/javascript">
function validar(e) {
tecla = (document.all) ? e.keyCode : e.which;
if (tecla==8 || tecla==46 || tecla==48 || tecla==49) return true;
return false;
}
</script> 

</script>
</head>
<body bgcolor="silver"/>


<h3>ingreso solo numeros binarios</h3>
<center>valor1<input type="text" id="sumarDosNumeros()" onkeypress="return validar(event)"  ></center>



</body>

</html>




<html>
<head>
<title>Invertir cadena</title>
<p align="center"><b>Invertir cadena

<SCRIPT LANGUAGE="JavaScript">

function reverse(form) {
text = "";
str = form.revtext.value;
for (i = 0; i <= str.length; i++)
text = str.substring(i, i+1) + text;
form.revtext.value = text;
}

</script>

</head>

</b>

<BODY style="font-family: Verdana">
</p>
<form>
<p align="center">
<input type=text name=revtext value="" size="20">
<input type=button value="Invertir" onClick="reverse(this.form)"> </p>
</form>
</body>

</html>



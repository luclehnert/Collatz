# Collatz

<html>
	<head>
		<title>Tabelle bauen</title>
			
		<meta charset="utf-8">
    </head>
		<script>
			"use strict";
			function programm() {
		
                var vAusgabe;
                var vN;
                var vNummern=1;



               
                vAusgabe= ""

                vN= document.getElementById("idvN").value;
                
                
            while (vN!=1) {
				
                vAusgabe=vAusgabe+vN+"->";
				
				
				if(vN%2>0){

                    vN=vN*3+1
				}
				
				else {
                    vN=vN/2
                    
                }
                vNummern++;
            }

            vAusgabe=vAusgabe+vN+"<br>";
            vAusgabe=vAusgabe+"<br>Anzahl an Berechnungen  : "+vNummern;

            document.getElementById("idAusgabe").innerHTML= vAusgabe;
        }
              


		</script>
	<body>

        <h1>Collatz-Folge und das 3n+1 Problem... </h1>
	
		  Collatz Zahlen <br><input id="idvN" type="text" value="27"></br>
		<button onClick="programm();">Collatz</button><br/><br/>
        <div id="idAusgabe"></div>
		
	</body>
</html>

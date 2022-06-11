
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>bmi calculator</title>
    <style>
        body {
            background-color: antiquewhite;

            overflow-x: hidden;
            border: 40px dotted violet;
            overflow-y: hidden;
            height: 660px;
        }

        @media screen and (max-width:350px){
           body{
               background-color: rgb(215, 250, 250);
               border: 2px dotted rgb(215, 250, 250);
           }
           #oo{
               font-size: 12px;
           }

        }
    </style>
</head>

<body id="i34">
   
        <h1 id="oo"
            style="text-align: center; font-size:55px; font-family: algerian; font-weight: lighter;color: rgb(63, 22, 100);">
           📈 BMI CALCULATOR</h1><br>
        <p id="n1" style="text-align: center;"></p>

    <div class="c1" style="height: 90vh; width: 100vw; text-align: center;">
            <label for="i1" style="font-family: algerian; font-weight: lighter;">ENTER YOUR HEIGHT(in mtrs)</label>
            <input type="text" name="height" id="i1">
            <br><br>
            <label for="i2" style="font-family: algerian; font-weight: lighter;">ENTER YOUR WEIGHT(in Kgs)</label>
            <input type="text" name="weight" id="i2">
            <br><br>
            <button onclick="am()">submit</button>
           
            <p style="height: 40px;" id="i3"></p>
            <p style="height: 40px;" id="i4"></p>
    </div>
    <script>
        document.getElementById("n1").innerHTML = Date();
        function am() {
            var float, a = document.getElementById("i1").value;
            var float, b = document.getElementById("i2").value;
            c = b / (a * a);
            document.getElementById("i3").innerHTML = "CALCULATED BMI IS:    " + c;
            if (c < 18) {
                document.getElementById("i4").innerHTML = "❌YOU ARE UNDER-WEIGHTED";
            }
            if (c >= 18 && c <= 25) {
                document.getElementById("i4").innerHTML = "✅YOU ARE FIT";
            }
            if (c > 25) {
                document.getElementById("i4").innerHTML = "❌OVER-WEIGHTED";
            }


        }

    </script>
</body>

</html>

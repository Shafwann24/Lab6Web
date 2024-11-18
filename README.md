<h2>1. jQuery Effects – Sliding</h2>

    <!DOCTYPE html>
    <html 
    <head>
        <script src=""http:ajax.googleapis.com/ajax/libs/jquery/1.10.2/jquery.min.js">
        </script>
        <script>
        $(document).ready(function(){
            $("#flip").click(function(){
                $("#panel").slideToggle("slow");
            });
        });
        </script>
    
        <style type="text/css">
            #panel, #flip {
                padding: 5px;
                text-align: center;
                background-color: #e5eecc;
                border: solid 1px #c3c3c3;
            }
            #panel {
                padding: 50px;
                display: none;
            }
    
        </style>
    </head>
    <body>
        <div id = "flip">Click to slide the panel down or up</div>
        <div id = "panel">Hello world!</div>
    </body>
    </html>

![image](https://github.com/user-attachments/assets/80086878-2c49-424d-aa3b-322b5d48c977)

Kode ini menggunakan jQuery untuk membuat animasi slide. Ketika elemen "flip" diklik, elemen "panel" akan tampil atau tersembunyi dengan efek geser.
<br> <hr>

<h2>2. jQuery Animation </h2>

    <!DOCTYPE html>
    <html>
    <head>
        <script src="http://ajax.googleapis.com/ajax/libs/jquery/1.10.2/jquery.min.js">
        </script>
        <script>
        $(document).ready(function(){
            $("button").click(function(){
                var div=$("div");
                div.animate({height:'300px',opacity:'0.4'}, "slow");
                div.animate({height:'300px',opacity:'0.8'}, "slow");
                div.animate({height:'100px',opacity:'0.4'}, "slow");
                div.animate({height:'100px',opacity:'0.8'}, "slow");
            });
        });
        </script>
    </head>
    <body>
        <button>Start Animation</button>
        <div style="background:#98bf21;height:100px;width:100px;position:absolute;"></div>
    </body>
    </html>

![image](https://github.com/user-attachments/assets/9b48ca5e-ecce-4da7-b628-ae2c98563bd5)

![image](https://github.com/user-attachments/assets/ad266feb-a373-4113-80c6-32b404dd6f4c)
Kode ini memanfaatkan jQuery untuk menambahkan animasi pada elemen `<div>` ketika tombol diklik. Animasi secara perlahan mengubah tinggi elemen antara 300px dan 100px, serta opasitasnya antara 0.4 dan 0.8.
<br> <hr>

<h2>3. jquery UI draggable </h2>

    <!DOCTYPE html>
    <html>
    <head>
        <title>Elemen yang Dapat Ditarik</title>
        <link rel="stylesheet" href="http://code.jquery.com/ui/1.10.3/themes/base/jquery-ui.css" />
        <script src="http://code.jquery.com/jquery-1.9.1.js"></script>
        <script src="http://code.jquery.com/ui/1.10.3/jquery-ui.js"></script>
        <style>
            #draggable {
                width: 125px;
                height: 125px;
                background-color: #FFF;
                text-align: center;
                padding: 1px 5px;
                border: 1px solid #AAA;
                margin: auto;
                float: left;
            }
    
            #containment-wrapper {
                width: 95%;
                height: 200px;
                border: 1px solid #4E4E4E;
                padding: 10px;
            }
        </style>
        <script>
            $(function() {
                $("#draggable").draggable({
                    containment: "#containment-wrapper",
                    scroll: false
                });
            });
        </script>
    </head>
    <body>
        <div id="containment-wrapper">
            <div id="draggable">
                <p>I'm contained within the box</p>
            </div>
        </div>
    </body>
    </html>

![image](https://github.com/user-attachments/assets/0fb063cc-47a4-40c5-abc4-d03c360e03d7)
Kode ini memungkinkan elemen draggable dapat dipindahkan (drag) hanya di dalam area containment-wrapper menggunakan jQuery UI.


    

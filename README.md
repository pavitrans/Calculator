 <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Calculator</title>
    <link rel="stylesheet" href="pjk1.css">
    <style>
        *{
    margin: 0;
    padding: 0;
    font-family: 'Poppins,sans serif';
    box-sizing: border-box;
}
.cont{
    width: 100%;
    height: 100vh;
    background-color: rgb(192, 228, 216);
    justify-content: center;
    align-items: center;
    display: flex;
}
.calcu{
    background-color: #304452;
    padding: 20px;
    border-radius: 10px;
}
.calcu form input{
    border: 0;
    outline: 0;
    width: 60px;
    height: 60px;
    border-radius: 10px;
    background-color: transparent;
    font-size: 30px;
    color: #fff;
    cursor: pointer;
    box-shadow: 5px 5px 10px rgb(64, 183, 183);
    margin: 10px;
    
}
form .display{
    display: flex;
    justify-content: flex-end;
    margin: 20px 0;
}
 form input.vv{
    width: 145px;
 }
 form .display input{
    text-align: right;
    flex: 1;
    font-size: 45px;
    box-shadow: none;
 }
 form input.col{
    color: orange;
 }
 form input.vv{
    color: orange;
 }

    </style>
</head>
<body>
    
    <div class="cont">
        <div class="calcu">
            <form action="">
                <div class="display">
                    <input type="text" name="display">
                </div>
                <div>
                    <input type="button" value="AC" onclick="display.value ='' " class="col">
                    <input type="button" value="DE" onclick="display.value=display.value.toString().slice(0,-1)" class="col">
                    <input type="button" value="." onclick="display.value +='.' " class="col">
                    <input type="button" value="/" onclick="display.value +='/' " class="col">
                </div>
                <div>
                    <input type="button" value="7" onclick="display.value +='7' ">
                    <input type="button" value="8" onclick="display.value +='8'">
                    <input type="button" value="9" onclick="display.value +='9'">
                    <input type="button" value="*" onclick="display.value +='*'" class="col">
                </div>
                <div>
                    <input type="button" value="4" onclick="display.value +='4'">
                    <input type="button" value="5" onclick="display.value +='5'">
                    <input type="button" value="6" onclick="display.value +='6'">
                    <input type="button" value="-" onclick="display.value +='-'" class="col">
                </div>
                <div>
                    <input type="button" value="1" onclick="display.value +='1'">
                    <input type="button" value="2"onclick="display.value +='2'">
                    <input type="button" value="3" onclick="display.value +='3'">
                    <input type="button" value="+"onclick="display.value +='+'" class="col">
                </div>
                <div>
                    <input type="button" value="00" onclick="display.value +='00'">
                    <input type="button" value="0" onclick="display.value +='0'">
                    <input type="button" value="=" class="vv" onclick="display.value=eval(display.value)" class="col">
                 
                </div>
            </form>
        </div>
    </div>
</body>
</html>

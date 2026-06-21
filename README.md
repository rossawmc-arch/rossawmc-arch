<!DOCTYPE html>
<html lang="tr">
<head>
<meta charset="UTF-8">
<title>Border Radius Değiştirme</title>

<style>
body{
    background-color: gray;
    color: white;
    font-weight: bold;
    font-family: Arial;
}

#cerceve{
    background-color: orange;
    width: 100px;
    height: 100px;
    margin-top: 10px;
}
</style>
</head>

<body>

<div id="cerceve"></div>

<form>
    <input type="radio" id="r0" name="secm" onclick="kenaryuvarla('0px')">
    <label for="r0">0 pixel</label><br>

    <input type="radio" id="r10" name="secm" onclick="kenaryuvarla('10px')">
    <label for="r10">10 pixel</label><br>

    <input type="radio" id="r25" name="secm" onclick="kenaryuvarla('25px')">
    <label for="r25">25 pixel</label><br>

    <input type="radio" id="r50" name="secm" onclick="kenaryuvarla('50px')">
    <label for="r50">50 pixel</label><br>
</form>

<script>
function kenaryuvarla(degere){
    document.getElementById("cerceve").style.borderRadius = degere;
}
</script>

</body>
</html>

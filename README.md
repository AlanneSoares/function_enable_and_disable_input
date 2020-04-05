# Habilitar e Desabilitar Campos Input

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Title</title>
	
	<script type="text/javascript">

	function toogle_disable (bool) {
		var input = document.getElementsByTagName ('input');
		var textarea = document.getElementsByName ('textarea');

		for (var i = 0; i <= (input.length - 1); i++) {
			if (input [i].type != 'button') {
				input [i].disabled = bool;
			}
		}

		for (var i = 0; i <= (textarea.length - 1; i++) {
			textarea [i].disabled = bool;
		}
}

</script>
				
</head>

<body>

	<form>
		<input type = "button" onclick = "toogle_disabled (false)" value = "Habilitar" />
		<input type = "button" onclick = "toogle_disabled (true)" value = "Desabilitar" />

		<br>
		
		Nome: <input type = "text" name = "nome" />
		Local <input type = "text" name = "local" />
		
		<br>

		Nome: <input type = "text" name = "nome2" />
		Local <input type = "text" name = "local2" />
	</form>
</body>
</html>

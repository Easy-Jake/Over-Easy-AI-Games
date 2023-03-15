# Over-Easy-AI-Games
<!DOCTYPE html>
<html>
<head>
	<title>Escape the Diner</title>
</head>
<body>

	<h1>Escape The Diner</h1>

	<img src="dungeon1.png" alt="Dungeon1" style="width:100%; max-width:500px;">

	<p>You wake up to the smell of coffee and bacon, you're in a diner. You have no memory of how you got here. The only thing you know is that you are hungry and need to escape.</p>

	<p>There is a chest in the middle of the room. It is locked with a combination lock. The lock has three dials, each with the numbers 0-9. You see a note on the chest that reads:</p>

	<blockquote>
		<p>I am taken from a mine, and shut up in a wooden case, from which I am never released, and yet I am used by almost every human being. What am I?</p>
	</blockquote>

	<p>What combination do you enter?</p>

	<form onsubmit="return checkAnswer()">
		<input type="text" id="answer" maxlength="3">
		<input type="submit" value="Enter">
	</form>

	<script>
		function checkAnswer() {
			var answer = document.getElementById("answer").value;
			if (answer == "8 4 0") {
				alert("You enter the correct combination and the chest opens. Inside you find the key to the door. Congratulations, you have escaped!");
				location.reload();
				return false;
			} else {
				alert("You enter the wrong combination. Nothing happens.");
				return false;
			}
		}
	</script>

</body>
</html>
![Dungeon1](https://user-images.githubusercontent.com/127925463/225382017-995dc50a-832f-48fb-ae2e-2df782ff4529.jpg)

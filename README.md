# Macros-Calculateur

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Calculateur de Macros</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="container">
        <h1>Calculateur de Macros</h1>
        <form id="macroForm">
            <label for="age">Âge :</label>
            <input type="number" id="age" name="age" required><br>

            <label for="sex">Sexe :</label>
            <select id="sex" name="sex">
                <option value="male">Homme</option>
                <option value="female">Femme</option>
            </select><br>

            <label for="weight">Poids (kg) :</label>
            <input type="number" id="weight" name="weight" required><br>

            <label for="height">Taille (cm) :</label>
            <input type="number" id="height" name="height" required><br>

            <label for="activity">Niveau d'activité :</label>
            <select id="activity" name="activity">
                <option value="sedentary">Sédentaire</option>
                <option value="light">Léger</option>
                <option value="moderate">Modéré</option>
                <option value="active">Actif</option>
                <option value="very_active">Très actif</option>
            </select><br>

            <label for="goal">Objectif :</label>
            <select id="goal" name="goal">
                <option value="lose_weight">Perte de poids</option>
                <option value="maintain_weight">Maintien du poids</option>
                <option value="gain_muscle">Prise de masse</option>
            </select><br>

            <button type="button" onclick="calculateMacros()">Calculer</button>
        </form>

        <div id="results" style="display: none;">
            <h2>Résultats</h2>
            <p id="calories"></p>
            <p id="protein"></p>
            <p id="carbs"></p>
            <p id="fat"></p>
        </div>
    </div>
    <script src="script.js"></script>
</body>
</html>

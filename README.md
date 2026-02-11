<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Foot Locker - Instant Gagnant</title>
    <link href="https://fonts.googleapis.com/css2?family=Oswald:wght@700&family=Roboto:wght@400;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary-orange: #EF422B;
            --dark-grey: #222222;
            --light-grey: #F5F5F5;
            --white: #FFFFFF;
            --font-display: 'Oswald', sans-serif;
            --font-body: 'Roboto', sans-serif;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            background-color: var(--dark-grey);
            color: var(--white);
            font-family: var(--font-body);
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            padding: 20px;
        }

        .container {
            width: 100%;
            max-width: 450px;
            background: linear-gradient(180deg, #333 0%, #111 100%);
            border-radius: 20px;
            overflow: hidden;
            box-shadow: 0 20px 50px rgba(0,0,0,0.5);
            text-align: center;
            border: 1px solid #444;
        }
        .header {
            padding: 30px 20px;
        }

        .sneaker-display {
            display: flex;
            justify-content: center;
            gap: 10px;
            margin-bottom: 20px;
        }

        .sneaker-display img {
            width: 80px;
            filter: drop-shadow(0 10px 15px rgba(0,0,0,0.5));
            transition: transform 0.3s ease;
        }

        .sneaker-display img:hover {
            transform: translateY(-10px) scale(1.1);
        }

        h1 {
            font-family: var(--font-display);
            font-size: 2.5rem;
            text-transform: uppercase;
            letter-spacing: 1px;
            margin-bottom: 10px;
        }

        p.subtitle {
            font-size: 0.9rem;
            color: #bbb;
            margin-bottom: 30px;
        }
        .form-section {
            padding: 0 30px 40px;
        }

        .input-group {
            margin-bottom: 15px;
            text-align: left;
        }

        input {
            width: 100%;
            padding: 12px 15px;
            border-radius: 5px;
            border: 1px solid #555;
            background: rgba(255, 255, 255, 0.05);
            color: white;
            font-size: 1rem;
            outline: none;
            transition: border-color 0.3s;
        }

        input:focus {
            border-color: var(--primary-orange);
        }
        .btn {
            display: inline-block;
            width: 100%;
            padding: 15px;
            margin-top: 10px;
            border: none;
            border-radius: 5px;
            font-family: var(--font-display);
            font-size: 1.1rem;
            text-transform: uppercase;
            cursor: pointer;
            transition: all 0.2s ease;
            text-decoration: none;
        }

        .btn-primary {
            background-color: var(--primary-orange);
            color: white;
        }

        .btn-primary:hover {
            background-color: #d63824;
            transform: scale(1.02);
        }

        .btn-secondary {
            background: transparent;
            color: #999;
            font-size: 0.8rem;
            margin-top: 5px;
        }

        .btn-secondary:hover {
            color: white;
        }
        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.05); }
            100% { transform: scale(1); }
        }

        .winner-tag {
            color: var(--primary-orange);
            font-weight: bold;
            animation: pulse 2s infinite;
        }
    </style>
</head>
<body>

    <div class="container">
        <div class="header">
            <div class="sneaker-display">
                <img src="z1.jpeg" alt="Sneaker 1">
                <img src="Z2.jpeg" alt="Sneaker 2" style="width: 100px;">
                <img src="Z3.jpeg" alt="Sneaker 3">
            </div>
            <h1>Tente ta chance</h1>
            <p class="subtitle">Complète le formulaire pour <span class="winner-tag">récolter ton gain</span></p>
        </div>

        <div class="form-section">
            <div class="input-group">
                <input type="text" placeholder="Prénom" required>
            </div>
            <div class="input-group">
                <input type="text" placeholder="Nom" required>
            </div>
            <div class="input-group">
                <input type="email" placeholder="E-mail" required>
            </div>
            <div class="input-group">
                <input type="text" placeholder="Code Postal" required>
            </div>
            <div class="input-group">
                <input type="tel" placeholder="Téléphone" required>
            </div>

            <button class="btn btn-primary">Valider</button>
            <a href="#" class="btn btn-secondary">Précédent</a>
        </div>
    </div>

</body>
</html>

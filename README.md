<!DOCTYPE html>
<html lang="ro">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Formular Comandă Serviciu</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #f9f9f9;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      margin: 0;
    }
    .container {
      background: #fff;
      padding: 30px;
      border-radius: 15px;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
      width: 100%;
      max-width: 420px;
    }
    h2 {
      text-align: center;
      color: #333;
    }
    label {
      margin-top: 15px;
      display: block;
      font-weight: bold;
    }
    select, input, textarea {
      width: 100%;
      padding: 10px;
      margin-top: 5px;
      border-radius: 8px;
      border: 1px solid #ccc;
      font-size: 16px;
    }
    .row {
      display: flex;
      gap: 10px;
      flex-wrap: wrap;
    }
    .row .half {
      flex: 1 1 48%;
    }
    button {
      margin-top: 20px;
      width: 100%;
      padding: 12px;
      background-color: #007BFF;
      color: white;
      border: none;
      border-radius: 8px;
      font-size: 16px;
      cursor: pointer;
    }
    button:hover {
      background-color: #0056b3;
    }
    .contact-info {
      margin-top: 25px;
      text-align: center;
      color: #555;
    }
    .company {
      font-weight: bold;
      margin-top: 8px;
    }
  </style>
</head>
<body>

  <div class="container">
    <h2>Plasează o Comandă</h2>
    <form action="https://formspree.io/f/mjkryvko" method="POST">
      <label for="serviciu">Alege serviciul:</label>
      <select id="serviciu" name="Serviciu dorit" required>
        <option value="">-- Selectează --</option>
        <option value="Diagnosticare PC">Diagnosticare PC/Laptop</option>
        <option value="Curățare sistem">Curățare sistem de răcire</option>
        <option value="Instalare Windows">Instalare Windows + drivere</option>
        <option value="Upgrade hardware">Upgrade hardware</option>
      </select>

      <label for="data">Alege data:</label>
      <input type="date" id="data" name="Data preferată" required>

      <label for="ora">Alege ora:</label>
      <input type="time" id="ora" name="Ora preferată" required>

      <div class="row">
<div class="half">
          <label for="telefon">Telefon:</label>
          <input type="tel" id="telefon" name="Telefon client" required>
        </div>
        <div class="half">
          <label for="email">Email:</label>
          <input type="email" id="email" name="Email client" required>
        </div>
      </div>

      <label for="comentariu">Comentariu (opțional):</label>
      <textarea id="comentariu" name="Comentariu" rows="3" placeholder="Scrie un detaliu opțional despre problemă..."></textarea>

      <button type="submit">Trimite Comanda</button>
    </form>

    <div class="contact-info">
      📞 Telefon: <strong>+373 (78) 806488</strong>
      <div class="company">🛠️ <strong>CTR Expert</strong></div>
    </div>
  </div>

</body>
</html>

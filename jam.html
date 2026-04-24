<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Fisch Sunken Chest Timer</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: linear-gradient(to right, #0f2027, #203a43, #2c5364);
      color: white;
      text-align: center;
      padding: 40px;
    }
    .container {
      background: rgba(0,0,0,0.4);
      padding: 30px;
      border-radius: 20px;
      display: inline-block;
      box-shadow: 0 0 20px rgba(0,0,0,0.5);
    }

    .input-group {
      display: flex;
      justify-content: center;
      align-items: center;
      gap: 10px;
    }

    #dayInput {
      width: 60px;
      padding: 10px;
      border-radius: 8px;
      border: none;
      text-align: center;
    }

    #timeInput {
      width: 160px;
      padding: 10px;
      border-radius: 8px;
      border: none;
      font-size: 16px;
    }

    button {
      padding: 10px 20px;
      font-size: 16px;
      margin-top: 15px;
      border-radius: 8px;
      border: none;
      background: #00c6ff;
      color: white;
      cursor: pointer;
    }

    #result, #countdown {
      margin-top: 15px;
      font-size: 18px;
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>🪙 Fisch Sunken Chest Timer</h1>

    <p>Input waktu (Hari + Jam)</p>
    <div class="input-group">
      <input type="number" id="dayInput" placeholder="d">
      <input type="time" id="timeInput">
    </div>

    <button onclick="hitungWaktu()">Hitung</button>

    <div id="result"></div>
    <div id="countdown"></div>
  </div>

  <script>
    let interval = null;

    function hitungWaktu() {
      const hari = parseInt(document.getElementById('dayInput').value) || 0;
      const timeValue = document.getElementById('timeInput').value;
      const result = document.getElementById('result');

      if (!timeValue) {
        result.innerHTML = "Masukkan waktu valid";
        return;
      }

      const [jam, menit] = timeValue.split(':').map(Number);

      // waktu input dalam menit total
      let inputTotalMenit = (hari * 24 * 60) + (jam * 60) + menit;

      let nextSpawn = null;

      // cari spawn berikutnya
      for (let k = 1; k < 10000; k++) {
        let spawnMenit = (k * 60) + ((k - 1) * 10);
        if (spawnMenit > inputTotalMenit) {
          nextSpawn = spawnMenit;
          break;
        }
      }

      let selisih = nextSpawn - inputTotalMenit;

      // konversi ke hari jam menit
      let totalMenit = nextSpawn;
      let hasilHari = Math.floor(totalMenit / (24 * 60));
      let sisaMenit = totalMenit % (24 * 60);
      let hasilJam = Math.floor(sisaMenit / 60);
      let hasilMenit = sisaMenit % 60;

      let jamStr = hasilJam.toString().padStart(2, '0');
      let menitStr = hasilMenit.toString().padStart(2, '0');

      result.innerHTML = `Spawn berikutnya: ${hasilHari}d ${jamStr}:${menitStr}`;

      // countdown dari waktu input
      if (interval) clearInterval(interval);

      let sisa = selisih * 60; // detik

      interval = setInterval(() => {
        if (sisa <= 0) {
          document.getElementById('countdown').innerHTML = "🪙 Chest muncul!";
          clearInterval(interval);
          return;
        }

        let menit = Math.floor(sisa / 60);
        let detik = sisa % 60;

        document.getElementById('countdown').innerHTML =
          `Countdown: ${menit} menit ${detik} detik`;

        sisa--;
      }, 1000);
    }
  </script>
</body>
</html>

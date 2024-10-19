<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Elastic Stickman with Fixed Foot</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      background-color: #4682B4;
      overflow: hidden;
    }

    svg {
      width: 200px;
      height: 400px;
    }

    /* Styling stickman lines */
    .line {
      stroke: white;
      stroke-width: 2;
      stroke-linecap: round;
    }

    /* Cursor style for draggable parts */
    .draggable {
      cursor: pointer;
    }

    /* Transisi elastis */
    .elastic {
      transition: transform 0.2s ease-out;
    }
  </style>
</head>
<body>

  <div class="stickman">
    <svg id="stickman" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 200">
      <!-- Head -->
      <circle cx="50" cy="30" r="15" fill="none" stroke="white" stroke-width="2" />

      <!-- Body -->
      <line x1="50" y1="45" x2="50" y2="100" class="line elastic" id="body" />

      <!-- Left Arm: Tangan Atas (dari badan ke siku) dan Tangan Bawah (dari siku ke kepala) -->
      <line x1="50" y1="45" x2="35" y2="70" class="line" id="left-arm-upper" /> <!-- Tangan atas -->
      <line x1="35" y1="70" x2="40" y2="30" class="line" id="left-arm-lower" /> <!-- Tangan bawah -->

      <!-- Right Arm: Tangan Atas (dari badan ke siku) dan Tangan Bawah (dari siku ke kepala) -->
      <line x1="50" y1="45" x2="65" y2="70" class="line" id="right-arm-upper" /> <!-- Tangan atas -->
      <line x1="65" y1="70" x2="60" y2="30" class="line" id="right-arm-lower" /> <!-- Tangan bawah -->

      <!-- Hip and Legs -->
      <line x1="50" y1="100" x2="50" y2="110" class="line draggable elastic" id="hip" />
      <line x1="50" y1="110" x2="30" y2="140" class="line elastic" id="left-leg" />
      <line x1="50" y1="110" x2="70" y2="140" class="line elastic" id="right-leg" />

      <!-- Fixed feet (Ujung kaki tidak bergerak) -->
      <circle cx="30" cy="140" r="3" fill="white" id="left-foot" />
      <circle cx="70" cy="140" r="3" fill="white" id="right-foot" />
    </svg>
  </div>

  <script>
    let isDragging = false;
    let draggedElement = null;
    let startX, startY;

    // Fungsi untuk memulai drag
    function startDrag(evt) {
      isDragging = true;
      draggedElement = evt.target;
      startX = evt.clientX;
      startY = evt.clientY;
    }

    // Fungsi untuk menghentikan drag
    function stopDrag() {
      isDragging = false;
      draggedElement = null;
    }

    // Fungsi untuk melakukan drag dan geser bagian pinggul serta lutut mengikuti
    function drag(evt) {
      if (isDragging && draggedElement) {
        let deltaX = evt.clientX - startX;
        let deltaY = evt.clientY - startY;

        if (draggedElement.id === "hip") {
          let hip = document.getElementById("hip");
          let leftLeg = document.getElementById("left-leg");
          let rightLeg = document.getElementById("right-leg");
          let leftFoot = document.getElementById("left-foot");
          let rightFoot = document.getElementById("right-foot");
          let body = document.getElementById("body");

          // Geser pinggul ke arah mouse
          hip.setAttribute("x1", parseFloat(hip.getAttribute("x1")) + deltaX);
          hip.setAttribute("x2", parseFloat(hip.getAttribute("x2")) + deltaX);
          hip.setAttribute("y1", parseFloat(hip.getAttribute("y1")) + deltaY);
          hip.setAttribute("y2", parseFloat(hip.getAttribute("y2")) + deltaY);

          // Geser lutut (x1) mengikuti gerakan pinggul, kaki bagian bawah tetap di tempat (x2, y2 tidak berubah)
          leftLeg.setAttribute("x1", hip.getAttribute("x1"));
          leftLeg.setAttribute("y1", hip.getAttribute("y2"));

          rightLeg.setAttribute("x1", hip.getAttribute("x1"));
          rightLeg.setAttribute("y1", hip.getAttribute("y2"));

          // Geser badan mengikuti gerakan pinggul
          body.setAttribute("x2", hip.getAttribute("x1"));
          body.setAttribute("y2", hip.getAttribute("y1"));

          // Perbarui posisi mouse
          startX = evt.clientX;
          startY = evt.clientY;
        }
      }
    }

    // Tambahkan event listener untuk bagian pinggul yang bisa ditarik
    document.getElementById("hip").addEventListener("mousedown", startDrag);

    // Event listener untuk menghentikan drag
    document.addEventListener("mouseup", stopDrag);
    document.addEventListener("mousemove", drag);
  </script>

</body>
</html>

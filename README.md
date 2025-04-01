<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Organizational Chart</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            text-align: center;
            margin: 0;
            padding: 0;
        }
        h1, h2 {
            margin: 20px 0;
        }
        .chart {
            display: flex;
            flex-direction: column;
            align-items: center;
        }
        .level {
            display: flex;
            justify-content: center;
            margin-bottom: 20px;
            flex-wrap: wrap;
        }
        .box {
            border: 1px solid #000;
            background-color: #fff;
            padding: 10px;
            margin: 10px;
            position: relative;
            width: 120px;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            box-sizing: border-box;
        }
        .line {
            width: 2px;
            background-color: #000;
            height: 40px;
            position: absolute;
            left: 50%;
            margin-left: -1px;
            top: 100%;
        }
        .sub-level {
            display: flex;
            justify-content: space-around;
            width: 100%;
            flex-wrap: wrap;
        }

        /* Mobile-Friendly Adjustments */
        @media (max-width: 600px) {
            .level, .sub-level {
                flex-direction: column;
            }
            .box {
                width: 90%;
                margin: 5px 0;
            }
            .sub-level .box {
                width: 100%;
            }
        }

        /* Adjustments for larger screens */
        @media (min-width: 601px) {
            .level {
                flex-wrap: nowrap;
            }
            .box {
                width: 120px;
            }
        }
    </style>
</head>
<body>

    <h1>Bicol College Inc.</h1>
    <h2>Office of College of Computer Studies</h2>

    <div class="chart">
        <div class="level">
            <div class="box">Jeymay B. Betiz<br>Department Dean</div>
        </div>
        <div class="level">
            <div class="box">Joan Pavia<br>Program Chair</div>
            <div class="box">Jose Alther M. Rivera<br>Director</div>
        </div>
        <div class="level">
            <div class="box">Arlene A. De Vera<br>Deputy Director, OSAS - Cultural Unit</div>
            <div class="box">Marivic N. Neri<br>Deputy Director, OSAS - Discipline Unit</div>
            <div class="box">Jose Alther M. Rivera<br>Deputy Director, OSAS - Sports Unit</div>
            <div class="box">Jose Alther M. Rivera<br>Deputy Director, OSAS - Scholarship Unit</div>
        </div>
        <div class="sub-level">
            <div class="level">
                <div class="box">MALABOG EXTENSION CAMPUS</div>
                <div class="box">MINTAL CAMPUS</div>
                <div class="box">TAGUM UNIT</div>
                <div class="box">MABINI UNIT</div>
                <div class="box">OBRERO CAMPUS</div>
            </div>
        </div>
        <div class="sub-level">
            <div class="box">Noel B. Bahian<br>Campus OSAS Coordinator</div>
            <div class="box">Karen E. Geneston<br>Campus OSAS Coordinator</div>
            <div class="box">Kendi B. Aristito<br>Campus OSAS Coordinator</div>
            <div class="box">Edwin L. Solilap<br>Campus OSAS Coordinator</div>
            <div class="box">College OSAS Coordinator</div>
        </div>
    </div>
</body>
</html>


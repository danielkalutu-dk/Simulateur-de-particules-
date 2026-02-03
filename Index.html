<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Simulation des Déplacements des Atomes en fonction de la Vitesse</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background: linear-gradient(135deg, #0c2461 0%, #1e3799 100%);
            color: #fff;
            min-height: 100vh;
            padding: 20px;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
        }
        
        header {
            text-align: center;
            padding: 20px 0;
            margin-bottom: 30px;
        }
        
        h1 {
            font-size: 2.5rem;
            margin-bottom: 10px;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.3);
        }
        
        .subtitle {
            font-size: 1.2rem;
            opacity: 0.9;
            max-width: 800px;
            margin: 0 auto;
            line-height: 1.6;
        }
        
        .content {
            display: flex;
            flex-wrap: wrap;
            gap: 30px;
            margin-bottom: 30px;
        }
        
        .simulation-container {
            flex: 1;
            min-width: 300px;
            background-color: rgba(255, 255, 255, 0.1);
            border-radius: 15px;
            padding: 20px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
            backdrop-filter: blur(10px);
        }
        
        .controls {
            flex: 1;
            min-width: 300px;
            background-color: rgba(255, 255, 255, 0.1);
            border-radius: 15px;
            padding: 20px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
            backdrop-filter: blur(10px);
        }
        
        .simulation-title {
            font-size: 1.5rem;
            margin-bottom: 15px;
            color: #4bcffa;
        }
        
        .canvas-container {
            width: 100%;
            height: 400px;
            background-color: rgba(0, 0, 0, 0.3);
            border-radius: 10px;
            overflow: hidden;
            margin-bottom: 15px;
            position: relative;
        }
        
        #simulationCanvas {
            width: 100%;
            height: 100%;
        }
        
        .control-group {
            margin-bottom: 25px;
        }
        
        .control-title {
            font-size: 1.2rem;
            margin-bottom: 10px;
            color: #4bcffa;
        }
        
        .slider-container {
            display: flex;
            align-items: center;
            margin-bottom: 10px;
        }
        
        .slider-label {
            width: 180px;
            font-weight: 500;
        }
        
        .slider-value {
            width: 60px;
            text-align: center;
            font-weight: bold;
            color: #4bcffa;
        }
        
        input[type="range"] {
            flex-grow: 1;
            height: 10px;
            -webkit-appearance: none;
            background: rgba(255, 255, 255, 0.2);
            border-radius: 5px;
            outline: none;
        }
        
        input[type="range"]::-webkit-slider-thumb {
            -webkit-appearance: none;
            width: 22px;
            height: 22px;
            border-radius: 50%;
            background: #4bcffa;
            cursor: pointer;
            box-shadow: 0 0 10px rgba(75, 207, 250, 0.5);
        }
        
        .buttons {
            display: flex;
            gap: 15px;
            margin-top: 20px;
        }
        
        button {
            padding: 12px 20px;
            border: none;
            border-radius: 8px;
            background-color: #4bcffa;
            color: #0c2461;
            font-weight: bold;
            cursor: pointer;
            transition: all 0.3s ease;
            flex: 1;
            font-size: 1rem;
        }
        
        button:hover {
            background-color: #0fbcf9;
            transform: translateY(-2px);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
        }
        
        button:active {
            transform: translateY(0);
        }
        
        .info-panel {
            background-color: rgba(255, 255, 255, 0.1);
            border-radius: 15px;
            padding: 20px;
            margin-top: 20px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
            backdrop-filter: blur(10px);
        }
        
        .info-title {
            font-size: 1.5rem;
            margin-bottom: 15px;
            color: #4bcffa;
        }
        
        .physics-explanation {
            line-height: 1.7;
            margin-bottom: 20px;
        }
        
        .data-display {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 15px;
            margin-top: 20px;
        }
        
        .data-item {
            background-color: rgba(255, 255, 255, 0.1);
            padding: 15px;
            border-radius: 10px;
            text-align: center;
        }
        
        .data-label {
            font-size: 0.9rem;
            opacity: 0.8;
            margin-bottom: 5px;
        }
        
        .data-value {
            font-size: 1.4rem;
            font-weight: bold;
            color: #4bcffa;
        }
        
        .atom-types {
            display: flex;
            justify-content: center;
            gap: 10px;
            margin-top: 10px;
            flex-wrap: wrap;
        }
        
        .atom-type {
            display: flex;
            align-items: center;
            gap: 5px;
            padding: 5px 10px;
            background-color: rgba(255, 255, 255, 0.1);
            border-radius: 20px;
        }
        
        .atom-color {
            width: 15px;
            height: 15px;
            border-radius: 50%;
        }
        
        .atom-legend {
            margin-top: 15px;
            text-align: center;
            font-size: 0.9rem;
            opacity: 0.8;
        }
        
        footer {
            text-align: center;
            margin-top: 30px;
            padding-top: 20px;
            border-top: 1px solid rgba(255, 255, 255, 0.2);
            font-size: 0.9rem;
            opacity: 0.8;
        }
        
        @media (max-width: 768px) {
            .content {
                flex-direction: column;
            }
            
            h1 {
                font-size: 2rem;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <h1>Simulation des Déplacements des Atomes</h1>
            <p class="subtitle">Cette simulation montre comment la vitesse affecte les déplacements des atomes dans un gaz. Augmentez la température pour observer l'augmentation de l'agitation thermique et du mouvement brownien.</p>
        </header>
        
        <div class="content">
            <div class="simulation-container">
                <h2 class="simulation-title">Simulation des atomes</h2>
                <div class="canvas-container">
                    <canvas id="simulationCanvas"></canvas>
                </div>
                <div class="atom-legend">Légende des atomes :</div>
                <div class="atom-types">
                    <div class="atom-type">
                        <div class="atom-color" style="background-color: #4bcffa;"></div>
                        <span>Hydrogène (H)</span>
                    </div>
                    <div class="atom-type">
                        <div class="atom-color" style="background-color: #ff9ff3;"></div>
                        <span>Oxygène (O)</span>
                    </div>
                    <div class="atom-type">
                        <div class="atom-color" style="background-color: #feca57;"></div>
                        <span>Azote (N)</span>
                    </div>
                    <div class="atom-type">
                        <div class="atom-color" style="background-color: #ff6b6b;"></div>
                        <span>Carbone (C)</span>
                    </div>
                </div>
            </div>
            
            <div class="controls">
                <h2 class="simulation-title">Contrôles de simulation</h2>
                
                <div class="control-group">
                    <h3 class="control-title">Paramètres de vitesse</h3>
                    
                    <div class="slider-container">
                        <div class="slider-label">Température (K)</div>
                        <input type="range" id="temperatureSlider" min="0" max="1000" value="300" step="10">
                        <div class="slider-value" id="temperatureValue">300 K</div>
                    </div>
                    
                    <div class="slider-container">
                        <div class="slider-label">Vitesse moyenne</div>
                        <input type="range" id="speedSlider" min="0" max="100" value="30" step="1">
                        <div class="slider-value" id="speedValue">30</div>
                    </div>
                    
                    <div class="slider-container">
                        <div class="slider-label">Nombre d'atomes</div>
                        <input type="range" id="atomsSlider" min="10" max="200" value="80" step="10">
                        <div class="slider-value" id="atomsValue">80</div>
                    </div>
                </div>
                
                <div class="control-group">
                    <h3 class="control-title">Paramètres d'affichage</h3>
                    
                    <div class="slider-container">
                        <div class="slider-label">Taille des atomes</div>
                        <input type="range" id="sizeSlider" min="1" max="10" value="5" step="0.5">
                        <div class="slider-value" id="sizeValue">5</div>
                    </div>
                    
                    <div class="slider-container">
                        <div class="slider-label">Traces de déplacement</div>
                        <input type="range" id="tracesSlider" min="0" max="100" value="20" step="5">
                        <div class="slider-value" id="tracesValue">20%</div>
                    </div>
                </div>
                
                <div class="buttons">
                    <button id="pauseBtn">Pause / Reprendre</button>
                    <button id="resetBtn">Réinitialiser</button>
                    <button id="randomBtn">Atomes aléatoires</button>
                </div>
            </div>
        </div>
        
        <div class="info-panel">
            <h2 class="info-title">Explications physiques</h2>
            <div class="physics-explanation">
                <p>Cette simulation illustre le mouvement des atomes dans un gaz en fonction de leur vitesse. Selon la théorie cinétique des gaz, la température est proportionnelle à l'énergie cinétique moyenne des particules. Ainsi, lorsque la température augmente :</p>
                <ul style="padding-left: 20px; margin-top: 10px;">
                    <li>La vitesse moyenne des atomes augmente</li>
                    <li>Les déplacements deviennent plus importants</li>
                    <li>Les collisions entre atomes sont plus fréquentes</li>
                    <li>Le mouvement brownien (mouvement aléatoire) est plus visible</li>
                </ul>
                <p style="margin-top: 15px;">Les différents types d'atomes (Hydrogène, Oxygène, Azote, Carbone) ont des masses différentes, ce qui influence leur vitesse à une température donnée (selon la formule: v = √(3kT/m)).</p>
            </div>
            
            <div class="data-display">
                <div class="data-item">
                    <div class="data-label">Énergie cinétique moyenne</div>
                    <div class="data-value" id="energyValue">6.21e-21 J</div>
                </div>
                <div class="data-item">
                    <div class="data-label">Vitesse quadratique moyenne</div>
                    <div class="data-value" id="rmsSpeedValue">517 m/s</div>
                </div>
                <div class="data-item">
                    <div class="data-label">Collisions par seconde</div>
                    <div class="data-value" id="collisionsValue">42</div>
                </div>
                <div class="data-item">
                    <div class="data-label">Pression relative</div>
                    <div class="data-value" id="pressureValue">1.0 atm</div>
                </div>
            </div>
        </div>
        
        <footer>
            <p>Simulation physique - Déplacements des atomes en fonction de la vitesse | Créé pour un devoir de physique</p>
            <p>Les valeurs affichées sont des approximations pour illustrer les concepts physiques.</p>
        </footer>
    </div>

    <script>
        // Initialisation du canvas
        const canvas = document.getElementById('simulationCanvas');
        const ctx = canvas.getContext('2d');
        
        // Ajustement de la taille du canvas
        function resizeCanvas() {
            const container = canvas.parentElement;
            canvas.width = container.clientWidth;
            canvas.height = container.clientHeight;
        }
        
        // Variables de simulation
        let atoms = [];
        let animationId = null;
        let isPaused = false;
        
        // Constantes physiques
        const BOLTZMANN = 1.380649e-23; // Constante de Boltzmann en J/K
        const AVOGADRO = 6.02214076e23; // Nombre d'Avogadro
        
        // Types d'atomes avec leurs propriétés (masse molaire en kg/mol)
        const atomTypes = [
            { name: "Hydrogène", symbol: "H", color: "#4bcffa", mass: 0.001008 },
            { name: "Oxygène", symbol: "O", color: "#ff9ff3", mass: 0.01600 },
            { name: "Azote", symbol: "N", color: "#feca57", mass: 0.01401 },
            { name: "Carbone", symbol: "C", color: "#ff6b6b", mass: 0.01201 }
        ];
        
        // Classe Atom pour représenter un atome
        class Atom {
            constructor(x, y, typeIndex) {
                this.x = x;
                this.y = y;
                this.typeIndex = typeIndex;
                this.vx = 0;
                this.vy = 0;
                this.radius = parseFloat(document.getElementById('sizeSlider').value);
                this.trail = [];
                this.maxTrailLength = 10;
                this.color = atomTypes[typeIndex].color;
                this.mass = atomTypes[typeIndex].mass / 1000; // Conversion en kg
            }
            
            // Mettre à jour la position en fonction de la vitesse
            update(speedFactor) {
                // Appliquer le facteur de vitesse
                this.x += this.vx * speedFactor;
                this.y += this.vy * speedFactor;
                
                // Gestion des collisions avec les bords
                if (this.x < this.radius) {
                    this.x = this.radius;
                    this.vx = Math.abs(this.vx);
                }
                if (this.x > canvas.width - this.radius) {
                    this.x = canvas.width - this.radius;
                    this.vx = -Math.abs(this.vx);
                }
                if (this.y < this.radius) {
                    this.y = this.radius;
                    this.vy = Math.abs(this.vy);
                }
                if (this.y > canvas.height - this.radius) {
                    this.y = canvas.height - this.radius;
                    this.vy = -Math.abs(this.vy);
                }
                
                // Mettre à jour la traîne
                this.trail.push({x: this.x, y: this.y});
                if (this.trail.length > this.maxTrailLength) {
                    this.trail.shift();
                }
            }
            
            // Dessiner l'atome et sa traîne
            draw(tracePercentage) {
                // Dessiner la traîne si activée
                if (tracePercentage > 0) {
                    for (let i = 0; i < this.trail.length; i++) {
                        const point = this.trail[i];
                        const alpha = (i / this.trail.length) * (tracePercentage / 100);
                        ctx.beginPath();
                        ctx.arc(point.x, point.y, this.radius * 0.5, 0, Math.PI * 2);
                        ctx.fillStyle = this.color.replace(')', `, ${alpha})`).replace('rgb', 'rgba');
                        ctx.fill();
                    }
                }
                
                // Dessiner l'atome
                ctx.beginPath();
                ctx.arc(this.x, this.y, this.radius, 0, Math.PI * 2);
                ctx.fillStyle = this.color;
                ctx.fill();
                
                // Dessiner un contour
                ctx.beginPath();
                ctx.arc(this.x, this.y, this.radius, 0, Math.PI * 2);
                ctx.strokeStyle = 'rgba(255, 255, 255, 0.7)';
                ctx.lineWidth = 1;
                ctx.stroke();
            }
        }
        
        // Initialiser les atomes
        function initAtoms(numAtoms) {
            atoms = [];
            for (let i = 0; i < numAtoms; i++) {
                const typeIndex = Math.floor(Math.random() * atomTypes.length);
                const radius = parseFloat(document.getElementById('sizeSlider').value);
                const x = radius + Math.random() * (canvas.width - 2 * radius);
                const y = radius + Math.random() * (canvas.height - 2 * radius);
                
                const atom = new Atom(x, y, typeIndex);
                atoms.push(atom);
            }
            updateAtomSpeeds();
        }
        
        // Mettre à jour les vitesses des atomes en fonction de la température
        function updateAtomSpeeds() {
            const temperature = parseFloat(document.getElementById('temperatureSlider').value);
            const speedFactor = parseFloat(document.getElementById('speedSlider').value) / 30;
            
            // Calcul de la vitesse quadratique moyenne de référence (pour l'hydrogène à 300K)
            const refMass = atomTypes[0].mass / 1000; // Masse de l'hydrogène en kg
            const refSpeed = Math.sqrt(3 * BOLTZMANN * 300 / refMass); // v = √(3kT/m)
            
            atoms.forEach(atom => {
                // Calcul de la vitesse basée sur la température et la masse
                const mass = atom.mass;
                const rmsSpeed = Math.sqrt(3 * BOLTZMANN * temperature / mass);
                
                // Ajuster par le facteur de vitesse manuel
                const baseSpeed = rmsSpeed / refSpeed * 5 * speedFactor;
                
                // Donner une vitesse aléatoire dans une direction aléatoire
                const angle = Math.random() * Math.PI * 2;
                atom.vx = Math.cos(angle) * baseSpeed * (0.8 + Math.random() * 0.4);
                atom.vy = Math.sin(angle) * baseSpeed * (0.8 + Math.random() * 0.4);
            });
            
            // Mettre à jour les données affichées
            updatePhysicsData(temperature);
        }
        
        // Mettre à jour les données physiques affichées
        function updatePhysicsData(temperature) {
            // Calcul de l'énergie cinétique moyenne
            const avgEnergy = (3/2) * BOLTZMANN * temperature;
            document.getElementById('energyValue').textContent = avgEnergy.toExponential(2) + " J";
            
            // Calcul de la vitesse quadratique moyenne pour l'hydrogène (comme référence)
            const refMass = atomTypes[0].mass / 1000

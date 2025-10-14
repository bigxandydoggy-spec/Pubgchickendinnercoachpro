PubgCoachPro/                              
📁 READ.md
│
├── 📄 index.html                         
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>PubgCoachluciodevs - Professional PUBG Mobile Coach</title>
    <meta name="description" content="Advanced PUBG Mobile coaching assistant with device optimization, weapon sensitivity, and interactive aim trainer. Powered by DeepSeek">
    
    <!-- Ícones Personalizados -->
    <link rel="apple-touch-icon" sizes="180x180" href="assets/icons/apple-touch-icon.png">
    <link rel="icon" type="image/png" sizes="32x32" href="assets/icons/favicon-32x32.png">
    <link rel="icon" type="image/png" sizes="16x16" href="assets/icons/favicon-16x16.png">
    <link rel="manifest" href="assets/icons/site.webmanifest">
    <meta name="msapplication-TileColor" content="#ff6b35">
    <meta name="theme-color" content="#ff6b35">
    
    <!-- CSS -->
    <link rel="stylesheet" href="assets/css/style.css">
    <link rel="stylesheet" href="assets/css/aim-trainer.css">
</head>
<body>
    <!-- Audio Elements -->
    <audio id="backgroundMusic" loop>
        <source src="assets/audio/opening-music.mp3" type="audio/mpeg">
        Your browser does not support the audio element.
    </audio>

    <!-- Header -->
    <header class="app-header">
        <div class="header-content">
            <h1 class="app-title" data-i18n="appTitle">PubgCoachluciodevs</h1>
            <p class="app-subtitle" data-i18n="welcomeSubtitle">Professional PUBG Mobile Coach - Powered by DeepSeek</p>
            
            <div class="header-controls">
                <select id="languageSelector" class="language-selector">
                    <option value="en">English</option>
                    <option value="pt">Português</option>
                    <option value="ja">日本語</option>
                    <option value="ko">한국어</option>
                    <option value="zh">中文</option>
                </select>
                <button id="musicToggle" class="audio-control-btn">🎵</button>
            </div>
        </div>
    </header>

    <!-- Navigation -->
    <nav class="nav-container">
        <button class="nav-button active" data-section="home" data-i18n="home">Home</button>
        <button class="nav-button" data-section="device-optimizer" data-i18n="deviceOptimizer">Device Optimizer</button>
        <button class="nav-button" data-section="weapon-master" data-i18n="weaponMaster">Weapon Master</button>
        <button class="nav-button" data-section="aim-trainer" data-i18n="aimTrainer">Aim Trainer</button>
        <button class="nav-button" data-section="strategies" data-i18n="strategies">Strategies</button>
        <button class="nav-button" data-section="saved-configs" data-i18n="savedConfigs">My Configs</button>
    </nav>

    <!-- Main Content -->
    <main>
        <!-- Home Section -->
        <section id="home" class="section active">
            <div class="hero-section">
                <h2 data-i18n="welcomeHome">Welcome to PubgCoachluciodevs!</h2>
                <p data-i18n="welcomeText">The most advanced PUBG Mobile coaching platform. Optimize your device, master weapons, and improve your skills.</p>
                
                <div class="feature-grid">
                    <div class="feature-card">
                        <div class="feature-icon">📱</div>
                        <h3 data-i18n="feature1">Device Optimizer</h3>
                        <p data-i18n="feature1Desc">Get perfect graphics settings for your device and each map</p>
                    </div>
                    <div class="feature-card">
                        <div class="feature-icon">🎯</div>
                        <h3 data-i18n="feature2">Weapon Master</h3>
                        <p data-i18n="feature2Desc">Best sensitivity settings for every weapon and scope</p>
                    </div>
                    <div class="feature-card">
                        <div class="feature-icon">🔫</div>
                        <h3 data-i18n="feature3">Aim Trainer</h3>
                        <p data-i18n="feature3Desc">Interactive recoil control practice with real weapon patterns</p>
                    </div>
                    <div class="feature-card">
                        <div class="feature-icon">🗺️</div>
                        <h3 data-i18n="feature4">Strategy Guide</h3>
                        <p data-i18n="feature4Desc">Pro rotation routes and hiding spots for each map</p>
                    </div>
                </div>

                <div class="audio-notice">
                    <p>🔊 <span data-i18n="audioNotice">Click anywhere to enable background music</span></p>
                </div>
            </div>
        </section>

        <!-- Device Optimizer Section -->
        <section id="device-optimizer" class="section">
            <div class="section-header">
                <h2 data-i18n="deviceOptimizer">Device Graphics Optimizer</h2>
                <p data-i18n="deviceOptimizerDesc">Get the perfect graphics settings for your device and each PUBG map</p>
            </div>

            <div class="optimizer-container">
                <div class="device-search">
                    <input type="text" id="deviceSearch" placeholder="Search your device..." data-i18n-placeholder="searchDevicePlaceholder">
                    <button id="searchDeviceBtn" data-i18n="search">Search</button>
                </div>

                <div id="searchResults" class="search-results"></div>

                <div id="deviceConfig" class="device-config hidden">
                    <div class="device-header">
                        <h3 id="selectedDeviceName">Device Name</h3>
                        <button id="saveDeviceConfig" class="btn-secondary" data-i18n="saveConfig">Save Configuration</button>
                    </div>

                    <div class="map-selector">
                        <h4 data-i18n="selectMap">Select Map:</h4>
                        <div class="map-buttons">
                            <button class="map-btn active" data-map="erangel">Erangel</button>
                            <button class="map-btn" data-map="miramar">Miramar</button>
                            <button class="map-btn" data-map="vikendi">Vikendi</button>
                            <button class="map-btn" data-map="livik">Livik</button>
                            <button class="map-btn" data-map="nusa">Nusa</button>
                        </div>
                    </div>

                    <div id="graphicsSettings" class="graphics-settings">
                        <!-- Graphics settings will be loaded here -->
                    </div>

                    <div class="optimization-tips">
                        <h4 data-i18n="optimizationTips">Optimization Tips:</h4>
                        <p id="optimizationTipText">Loading tips...</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Weapon Master Section -->
        <section id="weapon-master" class="section">
            <div class="section-header">
                <h2 data-i18n="weaponMaster">Weapon Sensitivity Master</h2>
                <p data-i18n="weaponMasterDesc">Perfect sensitivity settings for every weapon and scope combination</p>
            </div>

            <div class="weapon-container">
                <div class="weapon-selector">
                    <div class="filter-buttons">
                        <button class="filter-btn active" data-type="all" data-i18n="allWeapons">All Weapons</button>
                        <button class="filter-btn" data-type="assault_rifle" data-i18n="assaultRifles">Assault Rifles</button>
                        <button class="filter-btn" data-type="smg" data-i18n="smgs">SMGs</button>
                        <button class="filter-btn" data-type="sniper" data-i18n="snipers">Snipers</button>
                    </div>

                    <div class="weapon-list" id="weaponList">
                        <!-- Weapons will be loaded here -->
                    </div>
                </div>

                <div class="weapon-details" id="weaponDetails">
                    <div class="select-weapon-prompt">
                        <p data-i18n="selectWeaponPrompt">Select a weapon to view detailed sensitivity settings</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Aim Trainer Section -->
        <section id="aim-trainer" class="section">
            <div class="section-header">
                <h2 data-i18n="aimTrainer">Interactive Aim Trainer</h2>
                <p data-i18n="aimTrainerDesc">Practice recoil control with real weapon patterns and sensitivity</p>
            </div>

            <div class="aim-trainer-container">
                <div class="aim-controls">
                    <div class="control-group">
                        <label for="weaponSelect" data-i18n="selectWeapon">Select Weapon:</label>
                        <select id="weaponSelect">
                            <option value="m416">M416</option>
                            <option value="akm">AKM</option>
                            <option value="ump45">UMP45</option>
                            <option value="scar_l">SCAR-L</option>
                            <option value="m762">Beryl M762</option>
                            <option value="aug">AUG A3</option>
                        </select>
                    </div>

                    <div class="control-group">
                        <label for="sensitivitySlider" data-i18n="sensitivity">Sensitivity:</label>
                        <input type="range" id="sensitivitySlider" min="1" max="100" value="50">
                        <div class="sensitivity-display">
                            <span data-i18n="low">Low</span>
                            <span id="sensitivityValue">50</span>
                            <span data-i18n="high">High</span>
                        </div>
                    </div>

                    <div class="audio-controls">
                        <h4 data-i18n="audioControls">Audio Controls</h4>
                        <div class="control-group">
                            <label for="musicVolume" data-i18n="musicVolume">Music Volume:</label>
                            <input type="range" id="musicVolume" min="0" max="100" value="30">
                        </div>
                        <div class="control-group">
                            <label for="sfxVolume" data-i18n="sfxVolume">SFX Volume:</label>
                            <input type="range" id="sfxVolume" min="0" max="100" value="50">
                        </div>
                        <button id="muteToggle" class="btn-secondary">🔊</button>
                    </div>

                    <div class="weapon-stats">
                        <h4 data-i18n="weaponStats">Weapon Stats</h4>
                        <div class="stat-row">
                            <span class="stat-label" data-i18n="weapon">Weapon:</span>
                            <span class="stat-value" id="weaponName">M416</span>
                        </div>
                        <div class="stat-row">
                            <span class="stat-label" data-i18n="damage">Damage:</span>
                            <span class="stat-value" id="weaponDamage">41</span>
                        </div>
                        <div class="stat-row">
                            <span class="stat-label" data-i18n="fireRate">Fire Rate:</span>
                            <span class="stat-value" id="weaponFireRate">0.085ms</span>
                        </div>
                        <div class="stat-row">
                            <span class="stat-label" data-i18n="recoil">Recoil:</span>
                            <span class="stat-value" id="weaponRecoil">Medium</span>
                        </div>
                        <div class="stat-row">
                            <span class="stat-label" data-i18n="difficulty">Difficulty:</span>
                            <span class="stat-value" id="weaponDifficulty">Medium</span>
                        </div>
                    </div>

                    <div class="spray-tip">
                        <h4 data-i18n="sprayControlTip">Spray Control Tip:</h4>
                        <p id="sprayTip">Pull down slightly during the first 10 shots</p>
                    </div>
                </div>

                <div class="aim-canvas-container">
                    <canvas id="aimCanvas" width="800" height="600"></canvas>
                    <div class="aim-stats">
                        <div data-i18n="accuracy">Accuracy:</div>
                        <div id="accuracyValue">0%</div>
                        <button id="resetStats" class="btn-small" data-i18n="resetStats">Reset</button>
                    </div>
                </div>
            </div>

            <div class="practice-modes">
                <div class="practice-mode active" data-mode="precision">
                    <div class="mode-icon">🎯</div>
                    <div class="mode-name" data-i18n="precisionMode">Precision Mode</div>
                    <div class="mode-desc" data-i18n="precisionDesc">Small targets, focus on accuracy</div>
                </div>
                <div class="practice-mode" data-mode="speed">
                    <div class="mode-icon">⚡</div>
                    <div class="mode-name" data-i18n="speedMode">Speed Mode</div>
                    <div class="mode-desc" data-i18n="speedDesc">Fast targets, focus on reaction time</div>
                </div>
                <div class="practice-mode" data-mode="recoil">
                    <div class="mode-icon">🔫</div>
                    <div class="mode-name" data-i18n="recoilMode">Recoil Control</div>
                    <div class="mode-desc" data-i18n="recoilDesc">Practice weapon recoil patterns</div>
                </div>
            </div>
        </section>

        <!-- Strategies Section -->
        <section id="strategies" class="section">
            <div class="section-header">
                <h2 data-i18n="strategies">Advanced Strategies</h2>
                <p data-i18n="strategiesDesc">Pro rotation routes and hiding spots for each map</p>
            </div>

            <div class="strategies-container">
                <div class="map-selector-tabs">
                    <button class="map-tab active" data-map="erangel">Erangel</button>
                    <button class="map-tab" data-map="miramar">Miramar</button>
                    <button class="map-tab" data-map="vikendi">Vikendi</button>
                    <button class="map-tab" data-map="livik">Livik</button>
                </div>

                <div class="strategies-content">
                    <div class="rotation-routes">
                        <h3 data-i18n="rotationRoutes">Rotation Routes</h3>
                        <div id="rotationRoutesList">
                            <!-- Routes will be loaded here -->
                        </div>
                    </div>

                    <div class="hiding-spots">
                        <h3 data-i18n="hidingSpots">Best Hiding Spots</h3>
                        <div id="hidingSpotsList">
                            <!-- Hiding spots will be loaded here -->
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Saved Configs Section -->
        <section id="saved-configs" class="section">
            <div class="section-header">
                <h2 data-i18n="savedConfigs">My Saved Configurations</h2>
                <p data-i18n="savedConfigsDesc">Your saved device and sensitivity configurations</p>
            </div>

            <div class="saved-configs-container">
                <div class="config-actions">
                    <button id="exportConfigs" class="btn-secondary" data-i18n="exportConfigs">Export All Configs</button>
                    <button id="importConfigs" class="btn-secondary" data-i18n="importConfigs">Import Configs</button>
                    <button id="clearAllConfigs" class="btn-danger" data-i18n="clearAll">Clear All</button>
                </div>

                <div class="configs-list" id="configsList">
                    <!-- Saved configs will be loaded here -->
                </div>

                <div class="practice-stats">
                    <h3 data-i18n="practiceStats">Practice Statistics</h3>
                    <div class="stats-grid">
                        <div class="stat-card">
                            <div class="stat-number" id="totalShots">0</div>
                            <div class="stat-label" data-i18n="totalShots">Total Shots</div>
                        </div>
                        <div class="stat-card">
                            <div class="stat-number" id="totalHits">0</div>
                            <div class="stat-label" data-i18n="totalHits">Total Hits</div>
                        </div>
                        <div class="stat-card">
                            <div class="stat-number" id="accuracyPercent">0%</div>
                            <div class="stat-label" data-i18n="accuracy">Accuracy</div>
                        </div>
                        <div class="stat-card">
                            <div class="stat-number" id="sessionsCount">0</div>
                            <div class="stat-label" data-i18n="sessions">Sessions</div>
                        </div>
                    </div>
                </div>
            </div>
        </section>
    </main>

    <!-- Footer -->
    <footer class="app-footer">
        <div class="footer-content">
            <p data-i18n="appTitle">PubgCoachluciodevs</p>
            <p data-i18n="poweredBy">Powered by DeepSeek</p>
            <p class="footer-note" data-i18n="footerNote">Professional PUBG Mobile Coaching Platform - Global Version</p>
        </div>
    </footer>

    <!-- JavaScript -->
    <script src="assets/js/audio-manager.js"></script>
    <script src="assets/js/storage.js"></script>
    <script src="assets/js/aim-trainer.js"></script>
    <script src="assets/js/script.js"></script>
</body>
</html>
│
├── 📁 locales/                           🌍 **PASTA IDIOMAS** (criar depois)
│   ├── 📄 en.json
{
    "appTitle": "PubgCoachluciodevs",
    "welcomeSubtitle": "Professional PUBG Mobile Coach - Powered by DeepSeek",
    "home": "Home",
    "deviceOptimizer": "Device Optimizer",
    "weaponMaster": "Weapon Master",
    "aimTrainer": "Aim Trainer",
    "strategies": "Strategies",
    "savedConfigs": "My Configs",
    "welcomeHome": "Welcome to PubgCoachluciodevs!",
    "welcomeText": "The most advanced PUBG Mobile coaching platform. Optimize your device, master weapons, and improve your skills.",
    "feature1": "Device Optimizer",
    "feature1Desc": "Get perfect graphics settings for your device and each map",
    "feature2": "Weapon Master",
    "feature2Desc": "Best sensitivity settings for every weapon and scope",
    "feature3": "Aim Trainer",
    "feature3Desc": "Interactive recoil control practice with real weapon patterns",
    "feature4": "Strategy Guide",
    "feature4Desc": "Pro rotation routes and hiding spots for each map",
    "audioNotice": "Click anywhere to enable background music",
    "deviceOptimizerDesc": "Get the perfect graphics settings for your device and each PUBG map",
    "searchDevicePlaceholder": "Search your device...",
    "search": "Search",
    "saveConfig": "Save Configuration",
    "selectMap": "Select Map:",
    "optimizationTips": "Optimization Tips:",
    "weaponMasterDesc": "Perfect sensitivity settings for every weapon and scope combination",
    "allWeapons": "All Weapons",
    "assaultRifles": "Assault Rifles",
    "smgs": "SMGs",
    "snipers": "Snipers",
    "selectWeaponPrompt": "Select a weapon to view detailed sensitivity settings",
    "aimTrainerDesc": "Practice recoil control with real weapon patterns and sensitivity",
    "selectWeapon": "Select Weapon:",
    "sensitivity": "Sensitivity:",
    "low": "Low",
    "high": "High",
    "audioControls": "Audio Controls",
    "musicVolume": "Music Volume:",
    "sfxVolume": "SFX Volume:",
    "weaponStats": "Weapon Stats",
    "weapon": "Weapon:",
    "damage": "Damage:",
    "fireRate": "Fire Rate:",
    "recoil": "Recoil:",
    "difficulty": "Difficulty:",
    "sprayControlTip": "Spray Control Tip:",
    "accuracy": "Accuracy:",
    "resetStats": "Reset",
    "precisionMode": "Precision Mode",
    "precisionDesc": "Small targets, focus on accuracy",
    "speedMode": "Speed Mode",
    "speedDesc": "Fast targets, focus on reaction time",
    "recoilMode": "Recoil Control",
    "recoilDesc": "Practice weapon recoil patterns",
    "strategiesDesc": "Pro rotation routes and hiding spots for each map",
    "rotationRoutes": "Rotation Routes",
    "hidingSpots": "Best Hiding Spots",
    "savedConfigsDesc": "Your saved device and sensitivity configurations",
    "exportConfigs": "Export All Configs",
    "importConfigs": "Import Configs",
    "clearAll": "Clear All",
    "practiceStats": "Practice Statistics",
    "totalShots": "Total Shots",
    "totalHits": "Total Hits",
    "sessions": "Sessions",
    "poweredBy": "Powered by DeepSeek",
    "footerNote": "Professional PUBG Mobile Coaching Platform - Global Version"
}
│   ├── 📄 pt.json
{
    "appTitle": "PubgCoachluciodevs",
    "welcomeSubtitle": "Coach Profissional de PUBG Mobile - Powered by DeepSeek",
    "home": "Início",
    "deviceOptimizer": "Otimizador de Dispositivo",
    "weaponMaster": "Mestre de Armas",
    "aimTrainer": "Treinador de Mira",
    "strategies": "Estratégias",
    "savedConfigs": "Minhas Configs",
    "welcomeHome": "Bem-vindo ao PubgCoachluciodevs!",
    "welcomeText": "A plataforma de coaching mais avançada para PUBG Mobile. Otimize seu dispositivo, domine armas e melhore suas habilidades.",
    "feature1": "Otimizador de Dispositivo",
    "feature1Desc": "Obtenha configurações gráficas perfeitas para seu dispositivo e cada mapa",
    "feature2": "Mestre de Armas",
    "feature2Desc": "Melhores configurações de sensibilidade para cada arma e mira",
    "feature3": "Treinador de Mira",
    "feature3Desc": "Prática interativa de controle de recuo com padrões reais de armas",
    "feature4": "Guia de Estratégias",
    "feature4Desc": "Rotas de rotação pro e melhores esconderijos para cada mapa",
    "audioNotice": "Clique em qualquer lugar para ativar a música de fundo",
    "deviceOptimizerDesc": "Obtenha as configurações gráficas perfeitas para seu dispositivo e cada mapa do PUBG",
    "searchDevicePlaceholder": "Pesquise seu dispositivo...",
    "search": "Pesquisar",
    "saveConfig": "Salvar Configuração",
    "selectMap": "Selecionar Mapa:",
    "optimizationTips": "Dicas de Otimização:",
    "weaponMasterDesc": "Configurações de sensibilidade perfeitas para cada combinação de arma e mira",
    "allWeapons": "Todas as Armas",
    "assaultRifles": "Rifles de Assalto",
    "smgs": "Submetralhadoras",
    "snipers": "Sniper Rifles",
    "selectWeaponPrompt": "Selecione uma arma para ver configurações detalhadas de sensibilidade",
    "aimTrainerDesc": "Pratique controle de recuo com padrões reais de armas e sensibilidade",
    "selectWeapon": "Selecionar Arma:",
    "sensitivity": "Sensibilidade:",
    "low": "Baixa",
    "high": "Alta",
    "audioControls": "Controles de Áudio",
    "musicVolume": "Volume da Música:",
    "sfxVolume": "Volume dos Efeitos:",
    "weaponStats": "Estatísticas da Arma",
    "weapon": "Arma:",
    "damage": "Dano:",
    "fireRate": "Taxa de Tiro:",
    "recoil": "Recuo:",
    "difficulty": "Dificuldade:",
    "sprayControlTip": "Dica de Controle de Spray:",
    "accuracy": "Precisão:",
    "resetStats": "Resetar",
    "precisionMode": "Modo Precisão",
    "precisionDesc": "Alvos pequenos, foco na precisão",
    "speedMode": "Modo Velocidade",
    "speedDesc": "Alvos rápidos, foco no tempo de reação",
    "recoilMode": "Controle de Recuo",
    "recoilDesc": "Pratique padrões de recuo das armas",
    "strategiesDesc": "Rotas de rotação pro e melhores esconderijos para cada mapa",
    "rotationRoutes": "Rotas de Rotação",
    "hidingSpots": "Melhores Esconderijos",
    "savedConfigsDesc": "Suas configurações salvas de dispositivo e sensibilidade",
    "exportConfigs": "Exportar Todas as Configs",
    "importConfigs": "Importar Configs",
    "clearAll": "Limpar Tudo",
    "practiceStats": "Estatísticas de Prática",
    "totalShots": "Total de Tiros",
    "totalHits": "Total de Acertos",
    "sessions": "Sessões",
    "poweredBy": "Powered by DeepSeek",
    "footerNote": "Plataforma Profissional de Coaching para PUBG Mobile - Versão Global"
}
│   ├── 📄 ja.json
{
  "devices": [
    {
      "id": "samsung_galaxy_s24_ultra",
      "name": "Samsung Galaxy S24 Ultra",
      "brand": "Samsung",
      "popularity": ["global", "korea", "japan"],
      "performance": "ultra_high",
      "graphics": {
        "erangel": {"quality": "Ultra HD", "fps": "90 FPS", "shadows": "Ultra", "anti_aliasing": "On", "reflections": "On"},
        "miramar": {"quality": "Ultra HD", "fps": "90 FPS", "shadows": "High", "anti_aliasing": "On", "reflections": "On"},
        "vikendi": {"quality": "HDR", "fps": "90 FPS", "shadows": "Ultra", "anti_aliasing": "On", "reflections": "On"},
        "livik": {"quality": "Ultra HD", "fps": "90 FPS", "shadows": "Ultra", "anti_aliasing": "On", "reflections": "On"},
        "nusa": {"quality": "Ultra HD", "fps": "90 FPS", "shadows": "High", "anti_aliasing": "On", "reflections": "On"}
      },
      "optimization_tips": {
        "global": "Use 90 FPS for competitive advantage in close combat",
        "korea": "90 FPS 활성화하여 근접 전투에서 경쟁력 확보",
        "japan": "近接戦闘で競争力を得るために90 FPSを使用"
      }
    },
    {
      "id": "iphone_15_pro_max", 
      "name": "iPhone 15 Pro Max",
      "brand": "Apple",
      "popularity": ["global", "japan", "korea"],
      "performance": "ultra_high",
      "graphics": {
        "erangel": {"quality": "Ultra HD", "fps": "120 FPS", "shadows": "Ultra", "anti_aliasing": "On", "reflections": "On"},
        "miramar": {"quality": "HDR", "fps": "120 FPS", "shadows": "High", "anti_aliasing": "On", "reflections": "On"},
        "vikendi": {"quality": "Ultra HD", "fps": "120 FPS", "shadows": "Ultra", "anti_aliasing": "On", "reflections": "On"},
        "livik": {"quality": "Ultra HD", "fps": "120 FPS", "shadows": "Ultra", "anti_aliasing": "On", "reflections": "On"},
        "nusa": {"quality": "HDR", "fps": "120 FPS", "shadows": "High", "anti_aliasing": "On", "reflections": "On"}
      },
      "optimization_tips": {
        "global": "120 FPS provides ultra-fast response for competitive play",
        "japan": "競技プレイには120 FPSで超高速応答を実現",
        "korea": "경쟁적 플레이를 위한 초고속 응답을 위해 120 FPS 사용"
      }
    }
  ]
}
│   ├── 📄 ko.json
{
  "devices": [
    {
      "id": "samsung_galaxy_s24_ultra",
      "name": "Samsung Galaxy S24 Ultra",
      "brand": "Samsung",
      "popularity": ["global", "korea", "japan"],
      "performance": "ultra_high",
      "graphics": {
        "erangel": {"quality": "Ultra HD", "fps": "90 FPS", "shadows": "Ultra", "anti_aliasing": "On", "reflections": "On"},
        "miramar": {"quality": "Ultra HD", "fps": "90 FPS", "shadows": "High", "anti_aliasing": "On", "reflections": "On"},
        "vikendi": {"quality": "HDR", "fps": "90 FPS", "shadows": "Ultra", "anti_aliasing": "On", "reflections": "On"},
        "livik": {"quality": "Ultra HD", "fps": "90 FPS", "shadows": "Ultra", "anti_aliasing": "On", "reflections": "On"},
        "nusa": {"quality": "Ultra HD", "fps": "90 FPS", "shadows": "High", "anti_aliasing": "On", "reflections": "On"}
      },
      "optimization_tips": {
        "global": "Use 90 FPS for competitive advantage in close combat",
        "korea": "90 FPS 활성화하여 근접 전투에서 경쟁력 확보",
        "japan": "近接戦闘で競争力を得るために90 FPSを使用"
      }
    },
    {
      "id": "iphone_15_pro_max", 
      "name": "iPhone 15 Pro Max",
      "brand": "Apple",
      "popularity": ["global", "japan", "korea"],
      "performance": "ultra_high",
      "graphics": {
        "erangel": {"quality": "Ultra HD", "fps": "120 FPS", "shadows": "Ultra", "anti_aliasing": "On", "reflections": "On"},
        "miramar": {"quality": "HDR", "fps": "120 FPS", "shadows": "High", "anti_aliasing": "On", "reflections": "On"},
        "vikendi": {"quality": "Ultra HD", "fps": "120 FPS", "shadows": "Ultra", "anti_aliasing": "On", "reflections": "On"},
        "livik": {"quality": "Ultra HD", "fps": "120 FPS", "shadows": "Ultra", "anti_aliasing": "On", "reflections": "On"},
        "nusa": {"quality": "HDR", "fps": "120 FPS", "shadows": "High", "anti_aliasing": "On", "reflections": "On"}
      },
      "optimization_tips": {
        "global": "120 FPS provides ultra-fast response for competitive play",
        "japan": "競技プレイには120 FPSで超高速応答を実現",
        "korea": "경쟁적 플레이를 위한 초고속 응답을 위해 120 FPS 사용"
      }
    }
  ]
}
│   └── 📄 zh.json
│
├── 📁 data/                              🗃️ **PASTA DATABASES** (criar depois)
│   ├── 📄 devices.json
{
  "devices": [
    {
      "id": "samsung_galaxy_s24_ultra",
      "name": "Samsung Galaxy S24 Ultra",
      "brand": "Samsung",
      "popularity": ["global", "korea", "japan"],
      "performance": "ultra_high",
      "graphics": {
        "erangel": {"quality": "Ultra HD", "fps": "90 FPS", "shadows": "Ultra", "anti_aliasing": "On", "reflections": "On"},
        "miramar": {"quality": "Ultra HD", "fps": "90 FPS", "shadows": "High", "anti_aliasing": "On", "reflections": "On"},
        "vikendi": {"quality": "HDR", "fps": "90 FPS", "shadows": "Ultra", "anti_aliasing": "On", "reflections": "On"},
        "livik": {"quality": "Ultra HD", "fps": "90 FPS", "shadows": "Ultra", "anti_aliasing": "On", "reflections": "On"},
        "nusa": {"quality": "Ultra HD", "fps": "90 FPS", "shadows": "High", "anti_aliasing": "On", "reflections": "On"}
      },
      "optimization_tips": {
        "korea": "90 FPS ativado para vantagem competitiva",
        "japan": "Use Ultra HD para melhor experiência visual",
        "global": "Mantenha sombras ativas para spotting de inimigos"
      }
    },
    {
      "id": "iphone_15_pro_max", 
      "name": "iPhone 15 Pro Max",
      "brand": "Apple",
      "popularity": ["global", "japan", "korea"],
      "performance": "ultra_high",
      "graphics": {
        "erangel": {"quality": "Ultra HD", "fps": "120 FPS", "shadows": "Ultra", "anti_aliasing": "On", "reflections": "On"},
        "miramar": {"quality": "HDR", "fps": "120 FPS", "shadows": "High", "anti_aliasing": "On", "reflections": "On"},
        "vikendi": {"quality": "Ultra HD", "fps": "120 FPS", "shadows": "Ultra", "anti_aliasing": "On", "reflections": "On"},
        "livik": {"quality": "Ultra HD", "fps": "120 FPS", "shadows": "Ultra", "anti_aliasing": "On", "reflections": "On"},
        "nusa": {"quality": "HDR", "fps": "120 FPS", "shadows": "High", "anti_aliasing": "On", "reflections": "On"}
      },
      "optimization_tips": {
        "japan": "120 FPS para resposta ultra rápida",
        "korea": "Qualidade Ultra HD recomendada", 
        "global": "Aproveite os 120 FPS para vantagem competitiva"
      }
    },
    {
      "id": "xiaomi_13t_pro",
      "name": "Xiaomi 13T Pro",
      "brand": "Xiaomi",
      "popularity": ["global", "japan"],
      "performance": "high",
      "graphics": {
        "erangel": {"quality": "HDR", "fps": "90 FPS", "shadows": "Medium", "anti_aliasing": "On", "reflections": "Off"},
        "miramar": {"quality": "HD", "fps": "90 FPS", "shadows": "Low", "anti_aliasing": "On", "reflections": "Off"},
        "vikendi": {"quality": "HDR", "fps": "60 FPS", "shadows": "Medium", "anti_aliasing": "On", "reflections": "Off"},
        "livik": {"quality": "HDR", "fps": "90 FPS", "shadows": "Medium", "anti_aliasing": "On", "reflections": "Off"},
        "nusa": {"quality": "HD", "fps": "90 FPS", "shadows": "Low", "anti_aliasing": "On", "reflections": "Off"}
      },
      "optimization_tips": {
        "japan": "Use HDR para melhor qualidade visual",
        "global": "90 FPS disponível para melhor desempenho"
      }
    },
    {
      "id": "poco_f5_pro",
      "name": "POCO F5 Pro", 
      "brand": "POCO",
      "popularity": ["global", "korea"],
      "performance": "high",
      "graphics": {
        "erangel": {"quality": "HDR", "fps": "90 FPS", "shadows": "High", "anti_aliasing": "On", "reflections": "Off"},
        "miramar": {"quality": "HD", "fps": "90 FPS", "shadows": "Medium", "anti_aliasing": "On", "reflections": "Off"},
        "vikendi": {"quality": "HDR", "fps": "60 FPS", "shadows": "High", "anti_aliasing": "On", "reflections": "Off"},
        "livik": {"quality": "HDR", "fps": "90 FPS", "shadows": "High", "anti_aliasing": "On", "reflections": "Off"},
        "nusa": {"quality": "HD", "fps": "90 FPS", "shadows": "Medium", "anti_aliasing": "On", "reflections": "Off"}
      },
      "optimization_tips": {
        "korea": "90 FPS ativado para jogabilidade suave",
        "global": "Ajuste sombras conforme o mapa"
      }
    },
    {
      "id": "huawei_p60_pro",
      "name": "Huawei P60 Pro",
      "brand": "Huawei", 
      "popularity": ["global", "japan"],
      "performance": "high",
      "graphics": {
        "erangel": {"quality": "HDR", "fps": "60 FPS", "shadows": "High", "anti_aliasing": "On", "reflections": "On"},
        "miramar": {"quality": "HD", "fps": "60 FPS", "shadows": "Medium", "anti_aliasing": "On", "reflections": "On"},
        "vikendi": {"quality": "HDR", "fps": "60 FPS", "shadows": "High", "anti_aliasing": "On", "reflections": "On"},
        "livik": {"quality": "HDR", "fps": "60 FPS", "shadows": "High", "anti_aliasing": "On", "reflections": "On"},
        "nusa": {"quality": "HD", "fps": "60 FPS", "shadows": "Medium", "anti_aliasing": "On", "reflections": "On"}
      },
      "optimization_tips": {
        "japan": "HDR ativado para cores vibrantes",
        "global": "Performance estável em 60 FPS"
      }
    },
    {
      "id": "asus_rog_phone_7",
      "name": "ASUS ROG Phone 7",
      "brand": "ASUS",
      "popularity": ["global", "korea", "japan"], 
      "performance": "gaming_ultra",
      "graphics": {
        "erangel": {"quality": "Ultra HD", "fps": "144 FPS", "shadows": "Ultra", "anti_aliasing": "On", "reflections": "On"},
        "miramar": {"quality": "Ultra HD", "fps": "144 FPS", "shadows": "Ultra", "anti_aliasing": "On", "reflections": "On"},
        "vikendi": {"quality": "Ultra HD", "fps": "120 FPS", "shadows": "Ultra", "anti_aliasing": "On", "reflections": "On"},
        "livik": {"quality": "Ultra HD", "fps": "144 FPS", "shadows": "Ultra", "anti_aliasing": "On", "reflections": "On"},
        "nusa": {"quality": "Ultra HD", "fps": "144 FPS", "shadows": "Ultra", "anti_aliasing": "On", "reflections": "On"}
      },
      "optimization_tips": {
        "korea": "144 FPS para vantagem extrema",
        "japan": "Modo gaming ativado para melhor performance", 
        "global": "Aproveite todos os recursos do modo X"
      }
    }
  ]
}
{
  "devices": [
    {
      "id": "samsung_galaxy_a54",
      "name": "Samsung Galaxy A54",
      "brand": "Samsung",
      "popularity": ["global", "brazil", "india"],
      "performance": "medium",
      "graphics": {
        "erangel": {"quality": "HD", "fps": "60 FPS", "shadows": "Low", "anti_aliasing": "Off", "reflections": "Off"},
        "miramar": {"quality": "Smooth", "fps": "60 FPS", "shadows": "Off", "anti_aliasing": "Off", "reflections": "Off"},
        "vikendi": {"quality": "HD", "fps": "45 FPS", "shadows": "Low", "anti_aliasing": "Off", "reflections": "Off"},
        "livik": {"quality": "HD", "fps": "60 FPS", "shadows": "Low", "anti_aliasing": "Off", "reflections": "Off"},
        "nusa": {"quality": "Smooth", "fps": "60 FPS", "shadows": "Off", "anti_aliasing": "Off", "reflections": "Off"}
      },
      "optimization_tips": {
        "global": "Use Smooth para FPS estável em combate",
        "brazil": "Desative sombras para melhor desempenho",
        "india": "HD quality recommended for better visibility"
      }
    },
    {
      "id": "redmi_note_12",
      "name": "Redmi Note 12",
      "brand": "Xiaomi", 
      "popularity": ["global", "india", "indonesia"],
      "performance": "medium",
      "graphics": {
        "erangel": {"quality": "Smooth", "fps": "60 FPS", "shadows": "Off", "anti_aliasing": "Off", "reflections": "Off"},
        "miramar": {"quality": "Smooth", "fps": "60 FPS", "shadows": "Off", "anti_aliasing": "Off", "reflections": "Off"},
        "vikendi": {"quality": "Smooth", "fps": "45 FPS", "shadows": "Off", "anti_aliasing": "Off", "reflections": "Off"},
        "livik": {"quality": "Smooth", "fps": "60 FPS", "shadows": "Off", "anti_aliasing": "Off", "reflections": "Off"},
        "nusa": {"quality": "Smooth", "fps": "60 FPS", "shadows": "Off", "anti_aliasing": "Off", "reflections": "Off"}
      },
      "optimization_tips": {
        "global": "Smooth quality for best performance",
        "india": "Use 60 FPS for competitive gameplay",
        "indonesia": "Matikan shadow untuk FPS lebih baik"
      }
    },
    {
      "id": "oneplus_nord_3",
      "name": "OnePlus Nord 3",
      "brand": "OnePlus",
      "popularity": ["global", "europe", "india"],
      "performance": "high", 
      "graphics": {
        "erangel": {"quality": "HDR", "fps": "90 FPS", "shadows": "Medium", "anti_aliasing": "On", "reflections": "Off"},
        "miramar": {"quality": "HD", "fps": "90 FPS", "shadows": "Low", "anti_aliasing": "On", "reflections": "Off"},
        "vikendi": {"quality": "HDR", "fps": "60 FPS", "shadows": "Medium", "anti_aliasing": "On", "reflections": "Off"},
        "livik": {"quality": "HDR", "fps": "90 FPS", "shadows": "Medium", "anti_aliasing": "On", "reflections": "Off"},
        "nusa": {"quality": "HD", "fps": "90 FPS", "shadows": "Low", "anti_aliasing": "On", "reflections": "Off"}
      },
      "optimization_tips": {
        "global": "90 FPS enabled for smooth gameplay",
        "europe": "HDR quality recommended for better graphics",
        "india": "Use 90 FPS for competitive advantage"
      }
    }
  ]
}
│   ├── 📄 weapons.json  
{
  "weapons": [
    {
      "id": "m416",
      "name": "M416",
      "type": "assault_rifle",
      "recoil_pattern": "vertical_moderate",
      "sensitivity": {
        "red_dot": {"general": 50, "ads": 45, "gyro": 30},
        "holo_sight": {"general": 48, "ads": 43, "gyro": 28},
        "x2_scope": {"general": 45, "ads": 40, "gyro": 25},
        "x3_scope": {"general": 42, "ads": 38, "gyro": 22},
        "x4_scope": {"general": 40, "ads": 35, "gyro": 20},
        "x6_scope": {"general": 38, "ads": 32, "gyro": 18}
      },
      "spray_control": "Puxe levemente para baixo durante os primeiros 10 tiros",
      "best_attachments": ["Vertical Grip", "Compensator", "Tactical Stock"],
      "damage": 41,
      "fire_rate": "high"
    },
    {
      "id": "akm",
      "name": "AKM",
      "type": "assault_rifle", 
      "recoil_pattern": "vertical_high",
      "sensitivity": {
        "red_dot": {"general": 45, "ads": 40, "gyro": 25},
        "holo_sight": {"general": 43, "ads": 38, "gyro": 23},
        "x2_scope": {"general": 40, "ads": 35, "gyro": 20},
        "x3_scope": {"general": 38, "ads": 32, "gyro": 18},
        "x4_scope": {"general": 35, "ads": 30, "gyro": 15},
        "x6_scope": {"general": 32, "ads": 28, "gyro": 12}
      },
      "spray_control": "Puxe firmemente para baixo - recuo forte mas previsível",
      "best_attachments": ["Compensator", "Vertical Grip"],
      "damage": 49,
      "fire_rate": "medium"
    },
    {
      "id": "ump45",
      "name": "UMP45",
      "type": "smg",
      "recoil_pattern": "low_easy",
      "sensitivity": {
        "red_dot": {"general": 55, "ads": 50, "gyro": 35},
        "holo_sight": {"general": 53, "ads": 48, "gyro": 33},
        "x2_scope": {"general": 50, "ads": 45, "gyro": 30}
      },
      "spray_control": "Recuo mínimo - ideal para combates médios e controle fácil",
      "best_attachments": ["Half Grip", "Suppressor", "Extended Quickdraw Mag"],
      "damage": 39,
      "fire_rate": "high"
    }
  ]
}
{
  "weapons": [
    {
      "id": "m416",
      "name": "M416",
      "name_jp": "M416",
      "name_kr": "M416",
      "type": "assault_rifle",
      "recoil_pattern": "vertical_moderate",
      "difficulty": "medium",
      "spray_pattern": [0, -2, -4, -6, -8, -7, -5, -3, -1, 0, 2, 4, 6, 8, 10],
      "sensitivity": {
        "red_dot": {"general": 50, "ads": 45, "gyro": 30, "vertical_multiplier": 1.0},
        "holo_sight": {"general": 48, "ads": 43, "gyro": 28, "vertical_multiplier": 1.0},
        "x2_scope": {"general": 45, "ads": 40, "gyro": 25, "vertical_multiplier": 0.9},
        "x3_scope": {"general": 42, "ads": 38, "gyro": 22, "vertical_multiplier": 0.8},
        "x4_scope": {"general": 40, "ads": 35, "gyro": 20, "vertical_multiplier": 0.7},
        "x6_scope": {"general": 38, "ads": 32, "gyro": 18, "vertical_multiplier": 0.6}
      },
      "spray_control": {
        "global": "Puxe levemente para baixo durante os primeiros 10 tiros, depois suavize",
        "korea": "초기 10발 동안 살짝 아래로 당기고, 이후 부드럽게 조절하세요",
        "japan": "最初の10発は軽く下に引き、その後は滑らかに調整します"
      },
      "best_attachments": ["Vertical Grip", "Compensator", "Tactical Stock", "Extended Quickdraw Mag"],
      "damage": 41,
      "fire_rate": 0.085,
      "optimal_range": "50-150m"
    },
    {
      "id": "akm",
      "name": "AKM",
      "name_jp": "AKM", 
      "name_kr": "AKM",
      "type": "assault_rifle",
      "recoil_pattern": "vertical_high",
      "difficulty": "hard",
      "spray_pattern": [0, -4, -8, -12, -16, -14, -12, -10, -8, -6, -4, -2, 0, 2, 4],
      "sensitivity": {
        "red_dot": {"general": 45, "ads": 40, "gyro": 25, "vertical_multiplier": 1.2},
        "holo_sight": {"general": 43, "ads": 38, "gyro": 23, "vertical_multiplier": 1.2},
        "x2_scope": {"general": 40, "ads": 35, "gyro": 20, "vertical_multiplier": 1.1},
        "x3_scope": {"general": 38, "ads": 32, "gyro": 18, "vertical_multiplier": 1.0},
        "x4_scope": {"general": 35, "ads": 30, "gyro": 15, "vertical_multiplier": 0.9},
        "x6_scope": {"general": 32, "ads": 28, "gyro": 12, "vertical_multiplier": 0.8}
      },
      "spray_control": {
        "global": "Puxe firmemente para baixo - recuo forte mas previsível. Foque em bursts de 5-7 tiros",
        "korea": "강하게 아래로 당기세요 - 반동이 강하지만 예측 가능합니다. 5-7발 버스트에 집중하세요",
        "japan": "強く下に引いてください - 反動は強いが予測可能です。5-7発のバーストに集中します"
      },
      "best_attachments": ["Compensator", "Vertical Grip", "Extended Mag"],
      "damage": 49,
      "fire_rate": 0.100,
      "optimal_range": "30-100m"
    },
    {
      "id": "ump45",
      "name": "UMP45",
      "name_jp": "UMP45",
      "name_kr": "UMP45",
      "type": "smg", 
      "recoil_pattern": "low_easy",
      "difficulty": "easy",
      "spray_pattern": [0, -1, -2, -2, -1, 0, 1, 2, 2, 1, 0, -1, -2, -2, -1],
      "sensitivity": {
        "red_dot": {"general": 55, "ads": 50, "gyro": 35, "vertical_multiplier": 0.8},
        "holo_sight": {"general": 53, "ads": 48, "gyro": 33, "vertical_multiplier": 0.8},
        "x2_scope": {"general": 50, "ads": 45, "gyro": 30, "vertical_multiplier": 0.7}
      },
      "spray_control": {
        "global": "Recuo mínimo - ideal para combates médios e controle fácil. Spray contínuo eficiente",
        "korea": "최소 반동 - 중거리 전투와 쉬운 제어에 이상적입니다. 지속적인 사격이 효율적입니다",
        "japan": "最小反動 - 中距離戦闘と簡単な制御に最適です。連続射撃が効率的です"
      },
      "best_attachments": ["Half Grip", "Suppressor", "Extended Quickdraw Mag"],
      "damage": 39,
      "fire_rate": 0.092,
      "optimal_range": "20-80m"
    },
    {
      "id": "scar_l",
      "name": "SCAR-L",
      "name_jp": "SCAR-L",
      "name_kr": "SCAR-L", 
      "type": "assault_rifle",
      "recoil_pattern": "vertical_low",
      "difficulty": "easy",
      "spray_pattern": [0, -1, -2, -3, -4, -3, -2, -1, 0, 1, 2, 3, 4, 5, 6],
      "sensitivity": {
        "red_dot": {"general": 52, "ads": 47, "gyro": 32, "vertical_multiplier": 0.9},
        "holo_sight": {"general": 50, "ads": 45, "gyro": 30, "vertical_multiplier": 0.9},
        "x2_scope": {"general": 47, "ads": 42, "gyro": 27, "vertical_multiplier": 0.8},
        "x3_scope": {"general": 44, "ads": 39, "gyro": 24, "vertical_multiplier": 0.7},
        "x4_scope": {"general": 42, "ads": 37, "gyro": 22, "vertical_multiplier": 0.6},
        "x6_scope": {"general": 40, "ads": 35, "gyro": 20, "vertical_multiplier": 0.5}
      },
      "spray_control": {
        "global": "Recuo muito estável - perfeito para jogadores iniciantes. Controle linear e previsível",
        "korea": "매우 안정적인 반동 - 초보자에게 완벽합니다. 선형적이고 예측 가능한 제어",
        "japan": "非常に安定した反動 - 初心者に最適です。直線的で予測可能な制御"
      },
      "best_attachments": ["Angled Grip", "Compensator", "Extended Mag"],
      "damage": 43,
      "fire_rate": 0.096,
      "optimal_range": "50-200m"
    }
  ]
}
{
  "weapons": [
    {
      "id": "m762",
      "name": "Beryl M762",
      "name_jp": "ベリル M762",
      "name_kr": "베릴 M762", 
      "type": "assault_rifle",
      "recoil_pattern": "vertical_high_horizontal",
      "difficulty": "hard",
      "spray_pattern": [0, -3, -6, -9, -12, -10, -8, -6, -4, -2, 0, 2, 4, 6, 8],
      "sensitivity": {
        "red_dot": {"general": 44, "ads": 39, "gyro": 24, "vertical_multiplier": 1.3},
        "holo_sight": {"general": 42, "ads": 37, "gyro": 22, "vertical_multiplier": 1.3},
        "x2_scope": {"general": 39, "ads": 34, "gyro": 19, "vertical_multiplier": 1.2},
        "x3_scope": {"general": 36, "ads": 31, "gyro": 16, "vertical_multiplier": 1.1},
        "x4_scope": {"general": 34, "ads": 29, "gyro": 14, "vertical_multiplier": 1.0},
        "x6_scope": {"general": 32, "ads": 27, "gyro": 12, "vertical_multiplier": 0.9}
      },
      "spray_control": {
        "global": "Strong vertical + horizontal recoil. Pull down and slightly right. Best for close combat",
        "korea": "강한 수직 + 수평 반동. 아래로 그리고 약간 오른쪽으로 당기세요. 근접전에 최적",
        "japan": "強い垂直＋水平反動。下にそして少し右に引いてください。近接戦闘に最適"
      },
      "best_attachments": ["Vertical Grip", "Compensator", "Extended Mag"],
      "damage": 46,
      "fire_rate": 0.086,
      "optimal_range": "10-80m",
      "meta_rank": 2
    },
    {
      "id": "aug",
      "name": "AUG A3",
      "name_jp": "AUG A3", 
      "name_kr": "AUG A3",
      "type": "assault_rifle",
      "recoil_pattern": "vertical_low",
      "difficulty": "easy",
      "spray_pattern": [0, -1, -2, -2, -1, 0, 1, 1, 0, -1, -2, -2, -1, 0, 1],
      "sensitivity": {
        "red_dot": {"general": 53, "ads": 48, "gyro": 33, "vertical_multiplier": 0.8},
        "holo_sight": {"general": 51, "ads": 46, "gyro": 31, "vertical_multiplier": 0.8},
        "x2_scope": {"general": 48, "ads": 43, "gyro": 28, "vertical_multiplier": 0.7},
        "x3_scope": {"general": 45, "ads": 40, "gyro": 25, "vertical_multiplier": 0.6},
        "x4_scope": {"general": 43, "ads": 38, "gyro": 23, "vertical_multiplier": 0.5},
        "x6_scope": {"general": 41, "ads": 36, "gyro": 21, "vertical_multiplier": 0.4}
      },
      "spray_control": {
        "global": "Extremely stable - easiest AR to control. Perfect for all ranges",
        "korea": "극도로 안정적 - 제어하기 가장 쉬운 AR. 모든 거리에 완벽",
        "japan": "非常に安定 - 制御が最も簡単なAR。全距離に完璧"
      },
      "best_attachments": ["Any Grip", "Suppressor", "Extended Mag"],
      "damage": 43,
      "fire_rate": 0.083,
      "optimal_range": "50-200m",
      "meta_rank": 1
    }
  ]
}
{
  "weapons": [
    {
      "id": "m416",
      "name": "M416",
      "name_jp": "M416",
      "name_kr": "M416",
      "type": "assault_rifle",
      "recoil_pattern": "vertical_moderate",
      "difficulty": "medium",
      "spray_pattern": [0, -2, -4, -6, -8, -7, -5, -3, -1, 0, 2, 4, 6, 8, 10],
      "sensitivity": {
        "red_dot": {"general": 50, "ads": 45, "gyro": 30, "vertical_multiplier": 1.0},
        "holo_sight": {"general": 48, "ads": 43, "gyro": 28, "vertical_multiplier": 1.0},
        "x2_scope": {"general": 45, "ads": 40, "gyro": 25, "vertical_multiplier": 0.9},
        "x3_scope": {"general": 42, "ads": 38, "gyro": 22, "vertical_multiplier": 0.8},
        "x4_scope": {"general": 40, "ads": 35, "gyro": 20, "vertical_multiplier": 0.7},
        "x6_scope": {"general": 38, "ads": 32, "gyro": 18, "vertical_multiplier": 0.6}
      },
      "spray_control": {
        "global": "Pull down slightly during the first 10 shots, then smooth out",
        "korea": "처음 10발 동안 살짝 아래로 당기고, 이후 부드럽게 조절하세요",
        "japan": "最初の10発は軽く下に引き、その後は滑らかに調整します"
      },
      "best_attachments": ["Vertical Grip", "Compensator", "Tactical Stock", "Extended Quickdraw Mag"],
      "damage": 41,
      "fire_rate": 0.085,
      "optimal_range": "50-150m",
      "meta_rank": 1
    }
  ]
}
│   ├── 📄 strategies.json
{
  "strategies": {
    "erangel": {
      "name": "Erangel",
      "name_jp": "エランジェル",
      "name_kr": "에란겔",
      "rotation_routes": [
        {
          "id": "erangel_military_to_georgopol",
          "name": "Military to Georgopol",
          "difficulty": "advanced",
          "description": {
            "global": "Drop Military Base, loot quickly, rotate early to Georgopol through bridges. Control high ground near apartments.",
            "japan": "ミリタリーベースに降り、素早く戦利品を集め、橋を通ってジョージポルに早期に移動します。アパート近くの高台を制圧してください。",
            "korea": "밀리터리 베이스에 떨어져 빠르게 전리품을 수집하고 다리를 통해 조지폴로 일찍 이동하세요. 아파트 근처 고지를 장악하세요."
          },
          "safe_zone_timing": "Move before 2nd zone closure",
          "vehicle_recommendation": "Buggy or Motorcycle",
          "ambush_spots": ["Georgopol Apartments", "Bridge Camping Spots", "Hill near Rozhok"]
        },
        {
          "id": "erangel_school_to_rozhok", 
          "name": "School to Rozhok",
          "difficulty": "medium",
          "description": {
            "global": "Hot drop School, secure basic loot, rotate to Rozhok for better gear. Use buildings for cover during rotation.",
            "japan": "スクールにホットドロップし、基本的な戦利品を確保し、より良い装備のためにロジョークに移動します。移動中は建物をカバーとして使用してください。",
            "korea": "학교에 핫드롭하여 기본 전리품을 확보하고 더 좋은 장비를 위해 로조크로 이동하세요. 이동 중에는 건물을 엄폐물로 활용하세요."
          },
          "safe_zone_timing": "Move during 1st zone",
          "vehicle_recommendation": "Dacia or UAZ",
          "ambush_spots": ["School Rooftop", "Rozhok Hill", "Apartments Windows"]
        }
      ],
      "hiding_spots": [
        {
          "location": "Georgopol Apartments",
          "effectiveness": "high",
          "description": "Upper floors with window visibility. Perfect for ambushing players rotating from Military Base.",
          "visibility": "360-degree view",
          "escape_routes": 3
        },
        {
          "location": "School Rooftop",
          "effectiveness": "medium", 
          "description": "High ground with cover. Great for spotting enemies but vulnerable to snipers.",
          "visibility": "270-degree view",
          "escape_routes": 2
        }
      ]
    },
    "miramar": {
      "name": "Miramar", 
      "name_jp": "ミラマー",
      "name_kr": "미라마",
      "rotation_routes": [
        {
          "id": "miramar_pecado_to_power_grid",
          "name": "Pecado to Power Grid",
          "difficulty": "hard",
          "description": {
            "global": "Drop Pecado for early fights, loot quickly, rotate to Power Grid through open areas. Use terrain for cover.",
            "japan": "早期の戦闘のためにペカドに降り、素早く戦利品を集め、開けた地域を通ってパワーグリッドに移動します。地形をカバーとして使用してください。",
            "korea": "초기 전투를 위해 페카도에 떨어져 빠르게 전리품을 수집하고 열린 지역을 통해 파워 그리드로 이동하세요. 지형을 엄폐물로 활용하세요."
          },
          "safe_zone_timing": "Move before 3rd zone",
          "vehicle_recommendation": "Pickup Truck",
          "ambush_spots": ["Power Grid Towers", "Mountain Ridges", "Desert Hills"]
        }
      ],
      "hiding_spots": [
        {
          "location": "Power Grid Towers",
          "effectiveness": "very_high",
          "description": "Elevated position with metal cover. Hard to spot, excellent for ambushing.",
          "visibility": "180-degree view", 
          "escape_routes": 2
        }
      ]
    },
    "vikendi": {
      "name": "Vikendi",
      "name_jp": "ヴィケンディ",
      "name_kr": "비켄디",
      "rotation_routes": [
        {
          "id": "vikendi_cosmodrome_to_dino_park",
          "name": "Cosmodrome to Dino Park",
          "difficulty": "medium",
          "description": {
            "global": "Drop Cosmodrome for good loot, rotate to Dino Park using snow terrain for cover. Watch for snipers in hills.",
            "japan": "良い戦利品のためにコスモドロームに降り、雪の地形をカバーとして使用してディノパークに移動します。丘のスナイパーに注意してください。",
            "korea": "좋은 전리품을 위해 코스모드롬에 떨어져 눈 지형을 엄폐물로 활용하여 디노 파크로 이동하세요. 언덕의 저격수를 조심하세요."
          },
          "safe_zone_timing": "Move during 2nd zone",
          "vehicle_recommendation": "Snowmobile",
          "ambush_spots": ["Dino Park Structures", "Mountain Passes", "Forest Areas"]
        }
      ],
      "hiding_spots": [
        {
          "location": "Dino Park Main Building",
          "effectiveness": "high",
          "description": "Multiple floors with windows overlooking entire park. Great for defensive positions.",
          "visibility": "270-degree view",
          "escape_routes": 4
        }
      ]
    }
  }
}
│   └── 📄 sensitivity.json
│
└── 📁 assets/                            📦 **PASTA RECURSOS** (criar depois)
    ├── 📁 audio/                         🎵 **PASTA ÁUDIO** (criar dentro de assets)
    │   ├── 📄 opening-music.mp3
    │   ├── 📄 m416-shot.mp3
    │   ├── 📄 akm-shot.mp3
    │   ├── 📄 ump45-shot.mp3
    │   ├── 📄 scar-l-shot.mp3
    │   ├── 📄 m762-shot.mp3
    │   └── 📄 aug-shot.mp3
    │
    ├── 📁 css/                           🎨 **PASTA ESTILOS** (criar dentro de assets)
    │   ├── 📄 style.css
    /* ===== VARIÁVEIS E RESET ===== */
:root {
    --color-primary: #ff6b35;
    --color-primary-dark: #e55a2b;
    --color-dark: #1a1a1a;
    --color-darker: #141414;
    --color-gray: #2d2d2d;
    --color-light: #ffffff;
    --color-gold: #ffd700;
    --color-success: #4CAF50;
    --color-error: #f44336;
    --color-warning: #ff9800;
    --font-main: 'Arial', 'Segoe UI', sans-serif;
}

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
}

body {
    font-family: var(--font-main);
    background: linear-gradient(135deg, var(--color-darker) 0%, var(--color-dark) 100%);
    color: var(--color-light);
    line-height: 1.6;
    min-height: 100vh;
    overflow-x: hidden;
}

/* ===== HEADER ===== */
.app-header {
    background: rgba(26, 26, 26, 0.95);
    backdrop-filter: blur(10px);
    padding: 2rem 1rem;
    text-align: center;
    border-bottom: 3px solid var(--color-primary);
    position: relative;
    box-shadow: 0 4px 20px rgba(0, 0, 0, 0.3);
}

.header-content {
    max-width: 1200px;
    margin: 0 auto;
}

.app-title {
    font-size: 2.5rem;
    font-weight: 800;
    margin-bottom: 0.5rem;
    background: linear-gradient(45deg, var(--color-primary), var(--color-gold));
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    text-shadow: 0 2px 10px rgba(255, 107, 53, 0.3);
}

.app-subtitle {
    color: #cccccc;
    font-size: 1.1rem;
    font-weight: 300;
    margin-bottom: 1rem;
}

.language-selector {
    background: var(--color-gray);
    color: white;
    border: 1px solid #444;
    padding: 0.5rem 1rem;
    border-radius: 6px;
    cursor: pointer;
    font-size: 0.9rem;
    transition: all 0.3s ease;
}

.language-selector:hover {
    border-color: var(--color-primary);
    box-shadow: 0 0 10px rgba(255, 107, 53, 0.3);
}

/* ===== NAVEGAÇÃO ===== */
.nav-container {
    display: flex;
    justify-content: center;
    gap: 1rem;
    padding: 1.5rem;
    background: rgba(255, 107, 53, 0.1);
    backdrop-filter: blur(5px);
    flex-wrap: wrap;
    border-bottom: 1px solid rgba(255, 107, 53, 0.2);
}

.nav-button {
    background: var(--color-gray);
    color: white;
    border: none;
    padding: 1rem 2rem;
    border-radius: 8px;
    cursor: pointer;
    transition: all 0.3s ease;
    font-weight: 600;
    border: 2px solid transparent;
    min-width: 140px;
    font-size: 0.95rem;
}

.nav-button:hover {
    background: var(--color-primary);
    transform: translateY(-2px);
    box-shadow: 0 5px 15px rgba(255, 107, 53, 0.3);
}

.nav-button.active {
    background: var(--color-primary);
    border-color: var(--color-gold);
    box-shadow: 0 5px 15px rgba(255, 107, 53, 0.4);
    transform: translateY(-1px);
}

/* ===== SEÇÕES ===== */
.section {
    display: none;
    padding: 3rem 2rem;
    max-width: 1400px;
    margin: 0 auto;
    animation: fadeIn 0.5s ease;
    min-height: 70vh;
}

@keyframes fadeIn {
    from { 
        opacity: 0; 
        transform: translateY(20px); 
    }
    to { 
        opacity: 1; 
        transform: translateY(0); 
    }
}

.section.active {
    display: block;
}

.section-header {
    text-align: center;
    margin-bottom: 3rem;
}

.section-header h2 {
    font-size: 2.5rem;
    margin-bottom: 1rem;
    color: var(--color-primary);
}

.section-header p {
    font-size: 1.2rem;
    color: #cccccc;
    max-width: 600px;
    margin: 0 auto;
}

/* ===== HOME SECTION ===== */
.hero-section {
    text-align: center;
    max-width: 1000px;
    margin: 0 auto;
}

.hero-section h2 {
    font-size: 3rem;
    margin-bottom: 1.5rem;
    color: var(--color-primary);
}

.hero-section p {
    font-size: 1.3rem;
    margin-bottom: 3rem;
    color: #cccccc;
}

.feature-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 2rem;
    margin-top: 3rem;
}

.feature-card {
    background: rgba(255, 107, 53, 0.1);
    padding: 2.5rem 2rem;
    border-radius: 15px;
    border-left: 4px solid var(--color-primary);
    transition: all 0.3s ease;
    text-align: center;
    backdrop-filter: blur(10px);
}

.feature-card:hover {
    transform: translateY(-8px);
    box-shadow: 0 10px 30px rgba(255, 107, 53, 0.2);
}

.feature-card:nth-child(2) {
    border-left-color: var(--color-gold);
}

.feature-card:nth-child(3) {
    border-left-color: #4CAF50;
}

.feature-card:nth-child(4) {
    border-left-color: #2196F3;
}

.feature-icon {
    font-size: 3rem;
    margin-bottom: 1.5rem;
}

.feature-card h3 {
    color: var(--color-primary);
    margin-bottom: 1rem;
    font-size: 1.4rem;
    font-weight: 700;
}

.feature-card p {
    color: #cccccc;
    font-size: 1rem;
    text-align: center;
}

/* ===== DEVICE OPTIMIZER ===== */
.optimizer-container {
    max-width: 1000px;
    margin: 0 auto;
}

.device-search {
    display: flex;
    gap: 1rem;
    margin-bottom: 2rem;
}

.device-search input {
    flex: 1;
    padding: 1rem 1.5rem;
    background: #1a1a1a;
    color: white;
    border: 2px solid #444;
    border-radius: 8px;
    font-size: 1.1rem;
}

.device-search button {
    background: var(--color-primary);
    color: white;
    border: none;
    padding: 1rem 2rem;
    border-radius: 8px;
    cursor: pointer;
    font-weight: bold;
}

.search-results {
    background: var(--color-gray);
    border-radius: 10px;
    max-height: 300px;
    overflow-y: auto;
    margin-bottom: 2rem;
}

.search-result-item {
    padding: 1rem 1.5rem;
    border-bottom: 1px solid #444;
    cursor: pointer;
    transition: background 0.3s ease;
}

.search-result-item:hover {
    background: rgba(255, 107, 53, 0.1);
}

.search-result-item:last-child {
    border-bottom: none;
}

.device-config {
    background: var(--color-gray);
    padding: 2rem;
    border-radius: 15px;
    border-left: 4px solid var(--color-primary);
}

.device-header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 2rem;
}

.device-header h3 {
    color: var(--color-primary);
    font-size: 1.5rem;
}

.map-selector {
    margin-bottom: 2rem;
}

.map-buttons {
    display: flex;
    gap: 1rem;
    flex-wrap: wrap;
    margin-top: 1rem;
}

.map-btn {
    background: #1a1a1a;
    color: white;
    border: 2px solid #444;
    padding: 0.8rem 1.5rem;
    border-radius: 8px;
    cursor: pointer;
    transition: all 0.3s ease;
}

.map-btn.active {
    background: var(--color-primary);
    border-color: var(--color-primary);
}

.graphics-settings {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 1.5rem;
    margin-bottom: 2rem;
}

.setting-item {
    background: #1a1a1a;
    padding: 1.5rem;
    border-radius: 8px;
    text-align: center;
}

.setting-label {
    color: #cccccc;
    margin-bottom: 0.5rem;
    font-size: 0.9rem;
}

.setting-value {
    color: var(--color-gold);
    font-size: 1.2rem;
    font-weight: bold;
}

.optimization-tips {
    background: rgba(255, 107, 53, 0.1);
    padding: 1.5rem;
    border-radius: 8px;
    border-left: 4px solid var(--color-gold);
}

.optimization-tips h4 {
    color: var(--color-gold);
    margin-bottom: 1rem;
}

/* ===== WEAPON MASTER ===== */
.weapon-container {
    display: grid;
    grid-template-columns: 300px 1fr;
    gap: 2rem;
}

.filter-buttons {
    display: flex;
    flex-wrap: wrap;
    gap: 0.5rem;
    margin-bottom: 1.5rem;
}

.filter-btn {
    background: #1a1a1a;
    color: white;
    border: 1px solid #444;
    padding: 0.5rem 1rem;
    border-radius: 6px;
    cursor: pointer;
    font-size: 0.9rem;
    transition: all 0.3s ease;
}

.filter-btn.active {
    background: var(--color-primary);
    border-color: var(--color-primary);
}

.weapon-list {
    background: var(--color-gray);
    border-radius: 10px;
    max-height: 600px;
    overflow-y: auto;
}

.weapon-item {
    padding: 1rem 1.5rem;
    border-bottom: 1px solid #444;
    cursor: pointer;
    transition: background 0.3s ease;
}

.weapon-item:hover {
    background: rgba(255, 107, 53, 0.1);
}

.weapon-item.active {
    background: rgba(255, 107, 53, 0.2);
    border-left: 4px solid var(--color-primary);
}

.weapon-item:last-child {
    border-bottom: none;
}

.weapon-details {
    background: var(--color-gray);
    padding: 2rem;
    border-radius: 15px;
    min-height: 400px;
}

.select-weapon-prompt {
    text-align: center;
    color: #cccccc;
    font-style: italic;
    margin-top: 8rem;
}

/* ===== STRATEGIES SECTION ===== */
.strategies-container {
    max-width: 1200px;
    margin: 0 auto;
}

.map-selector-tabs {
    display: flex;
    gap: 1rem;
    margin-bottom: 2rem;
    flex-wrap: wrap;
}

.map-tab {
    background: #1a1a1a;
    color: white;
    border: 2px solid #444;
    padding: 1rem 2rem;
    border-radius: 8px;
    cursor: pointer;
    transition: all 0.3s ease;
    font-weight: bold;
}

.map-tab.active {
    background: var(--color-primary);
    border-color: var(--color-primary);
}

.strategies-content {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 2rem;
}

.rotation-routes, .hiding-spots {
    background: var(--color-gray);
    padding: 2rem;
    border-radius: 15px;
}

.rotation-routes h3, .hiding-spots h3 {
    color: var(--color-primary);
    margin-bottom: 1.5rem;
    font-size: 1.5rem;
}

/* ===== SAVED CONFIGS ===== */
.saved-configs-container {
    max-width: 1000px;
    margin: 0 auto;
}

.config-actions {
    display: flex;
    gap: 1rem;
    margin-bottom: 2rem;
    flex-wrap: wrap;
}

.btn-secondary {
    background: #1a1a1a;
    color: white;
    border: 2px solid #444;
    padding: 1rem 2rem;
    border-radius: 8px;
    cursor: pointer;
    transition: all 0.3s ease;
}

.btn-secondary:hover {
    border-color: var(--color-primary);
}

.btn-danger {
    background: var(--color-error);
    color: white;
    border: none;
    padding: 1rem 2rem;
    border-radius: 8px;
    cursor: pointer;
    transition: all 0.3s ease;
}

.configs-list {
    display: grid;
    gap: 1.5rem;
    margin-bottom: 3rem;
}

.config-item {
    background: var(--color-gray);
    padding: 1.5rem;
    border-radius: 10px;
    border-left: 4px solid var(--color-primary);
}

.practice-stats {
    background: var(--color-gray);
    padding: 2rem;
    border-radius: 15px;
}

.stats-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
    gap: 1.5rem;
    margin-top: 1.5rem;
}

.stat-card {
    background: #1a1a1a;
    padding: 1.5rem;
    border-radius: 8px;
    text-align: center;
}

.stat-number {
    font-size: 2rem;
    font-weight: bold;
    color: var(--color-gold);
    margin-bottom: 0.5rem;
}

.stat-label {
    color: #cccccc;
    font-size: 0.9rem;
}

/* ===== FOOTER ===== */
.app-footer {
    background: rgba(26, 26, 26, 0.95);
    padding: 2rem 1rem;
    text-align: center;
    border-top: 1px solid #444;
    margin-top: 4rem;
}

.footer-content p {
    margin-bottom: 0.5rem;
    color: #cccccc;
}

.footer-note {
    font-size: 0.9rem;
    color: #888 !important;
    margin-top: 1rem;
}

/* ===== UTILITY CLASSES ===== */
.hidden {
    display: none !important;
}

.text-center {
    text-align: center;
}

.text-gold {
    color: var(--color-gold);
}

.text-primary {
    color: var(--color-primary);
}

.mt-2 {
    margin-top: 2rem;
}

.mb-2 {
    margin-bottom: 2rem;
}

.fade-in {
    animation: fadeIn 0.5s ease;
}

/* ===== RESPONSIVIDADE ===== */
@media (max-width: 768px) {
    .app-title { 
        font-size: 2rem; 
    }
    
    .app-header {
        padding: 1.5rem 1rem;
    }
    
    .nav-container { 
        flex-direction: column; 
        gap: 0.8rem; 
        padding: 1rem;
    }
    
    .nav-button { 
        padding: 1rem 1.5rem; 
        min-width: auto;
        font-size: 0.9rem;
    }
    
    .section { 
        padding: 2rem 1rem; 
    }
    
    .feature-grid {
        grid-template-columns: 1fr;
        gap: 1.5rem;
    }
    
    .hero-section h2 {
        font-size: 2rem;
    }
    
    .device-search {
        flex-direction: column;
    }
    
    .weapon-container {
        grid-template-columns: 1fr;
    }
    
    .strategies-content {
        grid-template-columns: 1fr;
    }
    
    .config-actions {
        flex-direction: column;
    }
}

@media (max-width: 480px) {
    .app-title {
        font-size: 1.8rem;
    }
    
    .app-subtitle {
        font-size: 1rem;
    }
    
    .language-selector {
        position: static;
        margin-top: 1rem;
        width: 100%;
        max-width: 200px;
    }
    
    .feature-card,
    .strategy-card {
        padding: 1.5rem 1rem;
    }
    
    .section-header h2 {
        font-size: 2rem;
    }
}
    │   └── 📄 aim-trainer.css
    // === SIMULADOR DE MIRA E RECOIL ===
class AimTrainer {
    constructor() {
        this.canvas = null;
        this.ctx = null;
        this.targets = [];
        this.currentWeapon = null;
        this.sensitivity = 50;
        this.isAiming = false;
        this.recoilPattern = [];
        this.currentRecoilStep = 0;
    }

    init() {
        this.canvas = document.getElementById('aimCanvas');
        this.ctx = this.canvas.getContext('2d');
        this.setupEventListeners();
        this.createTargets();
        this.animate();
    }

    setupEventListeners() {
        // Controles de sensibilidade
        const sensitivitySlider = document.getElementById('sensitivitySlider');
        if (sensitivitySlider) {
            sensitivitySlider.addEventListener('input', (e) => {
                this.sensitivity = parseInt(e.target.value);
                document.getElementById('sensitivityValue').textContent = this.sensitivity;
            });
        }

        // Seleção de arma
        const weaponSelect = document.getElementById('weaponSelect');
        if (weaponSelect) {
            weaponSelect.addEventListener('change', (e) => {
                this.loadWeapon(e.target.value);
            });
        }

        // Controles de mira
        this.canvas.addEventListener('mousedown', (e) => this.startAim(e));
        this.canvas.addEventListener('mousemove', (e) => this.moveAim(e));
        this.canvas.addEventListener('mouseup', () => this.stopAim());
        this.canvas.addEventListener('touchstart', (e) => this.startAim(e.touches[0]));
        this.canvas.addEventListener('touchmove', (e) => this.moveAim(e.touches[0]));
        this.canvas.addEventListener('touchend', () => this.stopAim());
    }

    loadWeapon(weaponId) {
        // Carregar dados da arma do database
        fetch('data/weapons.json')
            .then(response => response.json())
            .then(data => {
                const weapon = data.weapons.find(w => w.id === weaponId);
                if (weapon) {
                    this.currentWeapon = weapon;
                    this.recoilPattern = weapon.spray_pattern || [];
                    this.updateWeaponDisplay(weapon);
                }
            });
    }

    updateWeaponDisplay(weapon) {
        document.getElementById('weaponName').textContent = weapon.name;
        document.getElementById('weaponDamage').textContent = weapon.damage;
        document.getElementById('weaponFireRate').textContent = (weapon.fire_rate * 1000).toFixed(1) + 'ms';
        document.getElementById('weaponRecoil').textContent = weapon.recoil_pattern;
        document.getElementById('weaponDifficulty').textContent = weapon.difficulty;
        
        // Atualizar dicas de controle
        const currentLang = document.getElementById('languageSelector').value;
        const sprayTip = weapon.spray_control[currentLang] || weapon.spray_control['global'];
        document.getElementById('sprayTip').textContent = sprayTip;
    }

    createTargets() {
        this.targets = [];
        for (let i = 0; i < 5; i++) {
            this.targets.push({
                x: Math.random() * (this.canvas.width - 60) + 30,
                y: Math.random() * (this.canvas.height - 60) + 30,
                radius: 25,
                hit: false
            });
        }
    }

    startAim(event) {
        const rect = this.canvas.getBoundingClientRect();
        const x = event.clientX - rect.left;
        const y = event.clientY - rect.top;

        this.isAiming = true;
        this.checkTargetHit(x, y);
    }

    moveAim(event) {
        if (!this.isAiming) return;

        const rect = this.canvas.getBoundingClientRect();
        const x = event.clientX - rect.left;
        const y = event.clientY - rect.top;

        // Aplicar recoil baseado na arma atual
        if (this.currentWeapon && this.recoilPattern.length > 0) {
            const recoilY = this.recoilPattern[this.currentRecoilStep] || 0;
            this.applyRecoil(recoilY);
            this.currentRecoilStep = (this.currentRecoilStep + 1) % this.recoilPattern.length;
        }
    }

    applyRecoil(recoilAmount) {
        // Simular efeito de recoil no canvas
        const sensitivityFactor = this.sensitivity / 50;
        const adjustedRecoil = recoilAmount * sensitivityFactor;
        
        // Aqui você implementaria o efeito visual do recoil
        console.log(`Recoil aplicado: ${adjustedRecoil}`);
    }

    stopAim() {
        this.isAiming = false;
        this.currentRecoilStep = 0;
    }

    checkTargetHit(x, y) {
        this.targets.forEach(target => {
            const distance = Math.sqrt((x - target.x) ** 2 + (y - target.y) ** 2);
            if (distance <= target.radius && !target.hit) {
                target.hit = true;
                this.showHitEffect(target.x, target.y);
                setTimeout(() => {
                    target.hit = false;
                    // Reposicionar alvo
                    target.x = Math.random() * (this.canvas.width - 60) + 30;
                    target.y = Math.random() * (this.canvas.height - 60) + 30;
                }, 500);
            }
        });
    }

    showHitEffect(x, y) {
        // Efeito visual de acerto
        this.ctx.fillStyle = '#00ff00';
        this.ctx.beginPath();
        this.ctx.arc(x, y, 35, 0, Math.PI * 2);
        this.ctx.fill();
        
        setTimeout(() => {
            this.draw(); // Redesenhar para remover o efeito
        }, 100);
    }

    draw() {
        // Limpar canvas
        this.ctx.fillStyle = '#1a1a1a';
        this.ctx.fillRect(0, 0, this.canvas.width, this.canvas.height);

        // Desenhar alvos
        this.targets.forEach(target => {
            this.ctx.fillStyle = target.hit ? '#ff4444' : '#ff6b35';
            this.ctx.beginPath();
            this.ctx.arc(target.x, target.y, target.radius, 0, Math.PI * 2);
            this.ctx.fill();

            // Centro do alvo
            this.ctx.fillStyle = '#ffffff';
            this.ctx.beginPath();
            this.ctx.arc(target.x, target.y, 8, 0, Math.PI * 2);
            this.ctx.fill();
        });

        // Desenhar mira central
        this.ctx.strokeStyle = '#00ff00';
        this.ctx.lineWidth = 2;
        const centerX = this.canvas.width / 2;
        const centerY = this.canvas.height / 2;
        
        this.ctx.beginPath();
        this.ctx.moveTo(centerX - 15, centerY);
        this.ctx.lineTo(centerX + 15, centerY);
        this.ctx.moveTo(centerX, centerY - 15);
        this.ctx.lineTo(centerX, centerY + 15);
        this.ctx.stroke();
    }

    animate() {
        this.draw();
        requestAnimationFrame(() => this.animate());
    }
}

// Inicializar simulador quando a página carregar
let aimTrainer;
document.addEventListener('DOMContentLoaded', () => {
    aimTrainer = new AimTrainer();
    aimTrainer.init();
});
    /* === SIMULADOR DE MIRA === */
.aim-trainer-section {
    padding: 2rem;
    max-width: 1200px;
    margin: 0 auto;
}

.aim-trainer-container {
    display: grid;
    grid-template-columns: 300px 1fr;
    gap: 2rem;
    margin-top: 2rem;
}

.aim-controls {
    background: var(--color-gray);
    padding: 1.5rem;
    border-radius: 10px;
    border-left: 4px solid var(--color-primary);
}

.control-group {
    margin-bottom: 1.5rem;
}

.control-group label {
    display: block;
    margin-bottom: 0.5rem;
    color: var(--color-primary);
    font-weight: bold;
}

.control-group select,
.control-group input[type="range"] {
    width: 100%;
    padding: 0.5rem;
    background: #1a1a1a;
    color: white;
    border: 1px solid #444;
    border-radius: 5px;
}

.sensitivity-display {
    display: flex;
    justify-content: space-between;
    margin-top: 0.5rem;
    color: #ccc;
    font-size: 0.9rem;
}

.weapon-stats {
    background: rgba(255, 107, 53, 0.1);
    padding: 1rem;
    border-radius: 8px;
    margin-top: 1rem;
}

.stat-row {
    display: flex;
    justify-content: space-between;
    margin-bottom: 0.5rem;
    font-size: 0.9rem;
}

.stat-label {
    color: #ccc;
}

.stat-value {
    color: var(--color-gold);
    font-weight: bold;
}

.spray-tip {
    background: rgba(255, 107, 53, 0.2);
    padding: 1rem;
    border-radius: 8px;
    margin-top: 1rem;
    font-style: italic;
    color: #ffd700;
}

.aim-canvas-container {
    position: relative;
    background: #1a1a1a;
    border-radius: 10px;
    overflow: hidden;
    border: 2px solid var(--color-primary);
}

#aimCanvas {
    width: 100%;
    height: 600px;
    display: block;
    cursor: crosshair;
}

.aim-stats {
    position: absolute;
    top: 1rem;
    left: 1rem;
    background: rgba(0, 0, 0, 0.8);
    padding: 1rem;
    border-radius: 8px;
    color: white;
}

.practice-modes {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 1rem;
    margin-top: 2rem;
}

.practice-mode {
    background: var(--color-gray);
    padding: 1.5rem;
    border-radius: 10px;
    text-align: center;
    cursor: pointer;
    transition: all 0.3s ease;
    border: 2px solid transparent;
}

.practice-mode:hover {
    border-color: var(--color-primary);
    transform: translateY(-2px);
}

.practice-mode.active {
    border-color: var(--color-gold);
    background: rgba(255, 107, 53, 0.1);
}

.mode-icon {
    font-size: 2rem;
    margin-bottom: 0.5rem;
}

.mode-name {
    font-weight: bold;
    color: var(--color-primary);
    margin-bottom: 0.5rem;
}

.mode-desc {
    color: #ccc;
    font-size: 0.9rem;
}

/* Responsividade do Simulador */
@media (max-width: 968px) {
    .aim-trainer-container {
        grid-template-columns: 1fr;
    }
    
    .aim-controls {
        order: 2;
    }
    
    .aim-canvas-container {
        order: 1;
    }
    
    #aimCanvas {
        height: 400px;
    }
}

@media (max-width: 480px) {
    .aim-trainer-section {
        padding: 1rem;
    }
    
    #aimCanvas {
        height: 300px;
    }
    
    .practice-modes {
        grid-template-columns: 1fr;
    }
}
// === SIMULADOR DE MIRA E RECOIL COM SONS ===
class AimTrainer {
    constructor() {
        this.canvas = null;
        this.ctx = null;
        this.targets = [];
        this.currentWeapon = null;
        this.sensitivity = 50;
        this.isAiming = false;
        this.recoilPattern = [];
        this.currentRecoilStep = 0;
        this.shotCount = 0;
        this.hitCount = 0;
        this.lastShotTime = 0;
        this.fireRate = 100; // ms entre tiros
    }

    init() {
        this.canvas = document.getElementById('aimCanvas');
        this.ctx = this.canvas.getContext('2d');
        this.setupEventListeners();
        this.createTargets();
        this.animate();
        
        // Carregar primeira arma
        this.loadWeapon('m416');
    }

    setupEventListeners() {
        // Controles de sensibilidade
        const sensitivitySlider = document.getElementById('sensitivitySlider');
        if (sensitivitySlider) {
            sensitivitySlider.addEventListener('input', (e) => {
                this.sensitivity = parseInt(e.target.value);
                document.getElementById('sensitivityValue').textContent = this.sensitivity;
            });
        }

        // Seleção de arma
        const weaponSelect = document.getElementById('weaponSelect');
        if (weaponSelect) {
            weaponSelect.addEventListener('change', (e) => {
                this.loadWeapon(e.target.value);
            });
        }

        // Controles de mira - MOUSE
        this.canvas.addEventListener('mousedown', (e) => this.startAim(e));
        this.canvas.addEventListener('mousemove', (e) => this.moveAim(e));
        this.canvas.addEventListener('mouseup', () => this.stopAim());
        
        // Controles de mira - TOUCH
        this.canvas.addEventListener('touchstart', (e) => {
            e.preventDefault();
            this.startAim(e.touches[0]);
        });
        this.canvas.addEventListener('touchmove', (e) => {
            e.preventDefault();
            this.moveAim(e.touches[0]);
        });
        this.canvas.addEventListener('touchend', (e) => {
            e.preventDefault();
            this.stopAim();
        });

        // Controles de áudio
        this.setupAudioControls();
    }

    setupAudioControls() {
        const musicVolumeSlider = document.getElementById('musicVolume');
        const sfxVolumeSlider = document.getElementById('sfxVolume');
        const muteToggle = document.getElementById('muteToggle');

        if (musicVolumeSlider) {
            musicVolumeSlider.addEventListener('input', (e) => {
                audioManager.setMusicVolume(parseInt(e.target.value) / 100);
            });
        }

        if (sfxVolumeSlider) {
            sfxVolumeSlider.addEventListener('input', (e) => {
                audioManager.setSfxVolume(parseInt(e.target.value) / 100);
            });
        }

        if (muteToggle) {
            muteToggle.addEventListener('click', () => {
                const isMuted = audioManager.toggleMute();
                muteToggle.textContent = isMuted ? '🔇' : '🔊';
            });
        }
    }

    loadWeapon(weaponId) {
        fetch('data/weapons.json')
            .then(response => response.json())
            .then(data => {
                const weapon = data.weapons.find(w => w.id === weaponId);
                if (weapon) {
                    this.currentWeapon = weapon;
                    this.recoilPattern = weapon.spray_pattern || [];
                    this.fireRate = weapon.fire_rate * 1000; // Converter para ms
                    this.updateWeaponDisplay(weapon);
                }
            })
            .catch(error => {
                console.error('Erro ao carregar arma:', error);
            });
    }

    updateWeaponDisplay(weapon) {
        document.getElementById('weaponName').textContent = weapon.name;
        document.getElementById('weaponDamage').textContent = weapon.damage;
        document.getElementById('weaponFireRate').textContent = (weapon.fire_rate * 1000).toFixed(1) + 'ms';
        document.getElementById('weaponRecoil').textContent = this.getRecoilText(weapon.recoil_pattern);
        document.getElementById('weaponDifficulty').textContent = weapon.difficulty;
        
        // Atualizar dicas de controle
        const currentLang = document.getElementById('languageSelector').value;
        const sprayTip = weapon.spray_control[currentLang] || weapon.spray_control['global'];
        document.getElementById('sprayTip').textContent = sprayTip;

        // Atualizar estatísticas de precisão
        this.updateAccuracyDisplay();
    }

    getRecoilText(recoilPattern) {
        const patterns = {
            'vertical_low': 'Low Vertical',
            'vertical_moderate': 'Medium Vertical', 
            'vertical_high': 'High Vertical',
            'vertical_high_horizontal': 'High Vertical + Horizontal',
            'low_easy': 'Very Low'
        };
        return patterns[recoilPattern] || recoilPattern;
    }

    createTargets() {
        this.targets = [];
        const targetCount = 6;
        
        for (let i = 0; i < targetCount; i++) {
            this.targets.push({
                x: Math.random() * (this.canvas.width - 80) + 40,
                y: Math.random() * (this.canvas.height - 80) + 40,
                radius: 20 + Math.random() * 15, // Tamanhos variados
                hit: false,
                hitTime: 0
            });
        }
    }

    startAim(event) {
        const rect = this.canvas.getBoundingClientRect();
        const x = event.clientX - rect.left;
        const y = event.clientY - rect.top;

        this.isAiming = true;
        this.handleShot(x, y);
    }

    moveAim(event) {
        if (!this.isAiming) return;

        const rect = this.canvas.getBoundingClientRect();
        const x = event.clientX - rect.left;
        const y = event.clientY - rect.top;

        // Verificar rate limiting para tiros
        const now = Date.now();
        if (now - this.lastShotTime >= this.fireRate) {
            this.handleShot(x, y);
            this.lastShotTime = now;
        }

        // Aplicar efeito de recoil visual
        this.applyRecoilEffect();
    }

    handleShot(x, y) {
        this.shotCount++;
        
        // Tocar som da arma
        if (this.currentWeapon) {
            audioManager.playWeaponSound(this.currentWeapon.id);
        } else {
            audioManager.playRandomWeaponSound();
        }

        // Verificar acerto
        const hit = this.checkTargetHit(x, y);
        if (hit) {
            this.hitCount++;
            audioManager.playHitSound();
        }

        this.updateAccuracyDisplay();
    }

    applyRecoilEffect() {
        if (this.currentWeapon && this.recoilPattern.length > 0) {
            // Aqui você implementaria o efeito visual de recoil
            // Por exemplo, mover a mira para cima baseado no padrão de recoil
            const recoilY = this.recoilPattern[this.currentRecoilStep] || 0;
            this.currentRecoilStep = (this.currentRecoilStep + 1) % this.recoilPattern.length;
            
            // Efeito visual sutil (pode ser expandido)
            this.canvas.style.transform = `translateY(${recoilY * 0.1}px)`;
            setTimeout(() => {
                this.canvas.style.transform = 'translateY(0)';
            }, 50);
        }
    }

    stopAim() {
        this.isAiming = false;
        this.currentRecoilStep = 0;
        this.canvas.style.transform = 'translateY(0)';
    }

    checkTargetHit(x, y) {
        let hit = false;
        
        this.targets.forEach(target => {
            const distance = Math.sqrt((x - target.x) ** 2 + (y - target.y) ** 2);
            if (distance <= target.radius && !target.hit) {
                target.hit = true;
                target.hitTime = Date.now();
                hit = true;
                
                this.showHitEffect(target.x, target.y);
                
                // Resetar alvo após 1 segundo
                setTimeout(() => {
                    target.hit = false;
                    target.x = Math.random() * (this.canvas.width - 80) + 40;
                    target.y = Math.random() * (this.canvas.height - 80) + 40;
                    target.radius = 20 + Math.random() * 15;
                }, 1000);
            }
        });
        
        return hit;
    }

    showHitEffect(x, y) {
        // Efeito visual de acerto
        this.ctx.fillStyle = '#00ff00';
        this.ctx.beginPath();
        this.ctx.arc(x, y, 30, 0, Math.PI * 2);
        this.ctx.fill();
        
        setTimeout(() => {
            this.draw(); // Redesenhar para remover o efeito
        }, 100);
    }

    updateAccuracyDisplay() {
        const accuracy = this.shotCount > 0 ? (this.hitCount / this.shotCount) * 100 : 0;
        document.getElementById('accuracyValue').textContent = accuracy.toFixed(1) + '%';
        
        // Atualizar estatísticas no storage
        if (this.shotCount > 0) {
            storageManager.updatePracticeStats(this.shotCount, this.hitCount);
        }
    }

    draw() {
        // Limpar canvas
        this.ctx.fillStyle = '#1a1a1a';
        this.ctx.fillRect(0, 0, this.canvas.width, this.canvas.height);

        // Desenhar grade de fundo sutil
        this.drawGrid();

        // Desenhar alvos
        this.targets.forEach(target => {
            // Cor baseada no estado do alvo
            if (target.hit) {
                this.ctx.fillStyle = '#00ff00';
            } else {
                const gradient = this.ctx.createRadialGradient(
                    target.x, target.y, 0,
                    target.x, target.y, target.radius
                );
                gradient.addColorStop(0, '#ff6b35');
                gradient.addColorStop(1, '#e55a2b');
                this.ctx.fillStyle = gradient;
            }

            this.ctx.beginPath();
            this.ctx.arc(target.x, target.y, target.radius, 0, Math.PI * 2);
            this.ctx.fill();

            // Centro do alvo
            this.ctx.fillStyle = target.hit ? '#ffffff' : '#ffd700';
            this.ctx.beginPath();
            this.ctx.arc(target.x, target.y, 6, 0, Math.PI * 2);
            this.ctx.fill();

            // Anel externo
            this.ctx.strokeStyle = target.hit ? '#00ff00' : '#ffffff';
            this.ctx.lineWidth = 2;
            this.ctx.beginPath();
            this.ctx.arc(target.x, target.y, target.radius + 2, 0, Math.PI * 2);
            this.ctx.stroke();
        });

        // Desenhar mira central
        this.drawCrosshair();
    }

    drawGrid() {
        this.ctx.strokeStyle = '#2a2a2a';
        this.ctx.lineWidth = 1;
        
        // Linhas verticais
        for (let x = 0; x <= this.canvas.width; x += 50) {
            this.ctx.beginPath();
            this.ctx.moveTo(x, 0);
            this.ctx.lineTo(x, this.canvas.height);
            this.ctx.stroke();
        }
        
        // Linhas horizontais
        for (let y = 0; y <= this.canvas.height; y += 50) {
            this.ctx.beginPath();
            this.ctx.moveTo(0, y);
            this.ctx.lineTo(this.canvas.width, y);
            this.ctx.stroke();
        }
    }

    drawCrosshair() {
        this.ctx.strokeStyle = '#00ff00';
        this.ctx.lineWidth = 2;
        const centerX = this.canvas.width / 2;
        const centerY = this.canvas.height / 2;
        
        // Cruz central
        this.ctx.beginPath();
        this.ctx.moveTo(centerX - 15, centerY);
        this.ctx.lineTo(centerX + 15, centerY);
        this.ctx.moveTo(centerX, centerY - 15);
        this.ctx.lineTo(centerX, centerY + 15);
        this.ctx.stroke();
        
        // Círculo externo
        this.ctx.beginPath();
        this.ctx.arc(centerX, centerY, 25, 0, Math.PI * 2);
        this.ctx.stroke();
        
        // Ponto central
        this.ctx.fillStyle = '#ff0000';
        this.ctx.beginPath();
        this.ctx.arc(centerX, centerY, 3, 0, Math.PI * 2);
        this.ctx.fill();
    }

    animate() {
        this.draw();
        requestAnimationFrame(() => this.animate());
    }

    resetStats() {
        this.shotCount = 0;
        this.hitCount = 0;
        this.updateAccuracyDisplay();
    }
}

// Inicializar simulador quando a página carregar
let aimTrainer;
document.addEventListener('DOMContentLoaded', () => {
    aimTrainer = new AimTrainer();
    aimTrainer.init();
});
    <!-- Controles de Áudio - Adicionar na seção Aim Trainer -->
<div class="audio-controls">
    <h4 data-i18n="audioControls">Audio Controls</h4>
    <div class="control-group">
        <label for="musicVolume" data-i18n="musicVolume">Music Volume:</label>
        <input type="range" id="musicVolume" min="0" max="100" value="30">
    </div>
    <div class="control-group">
        <label for="sfxVolume" data-i18n="sfxVolume">SFX Volume:</label>
        <input type="range" id="sfxVolume" min="0" max="100" value="50">
    </div>
    <button id="muteToggle" class="btn-secondary">🔊</button>
</div>
    /* === SIMULADOR DE MIRA === */
.aim-trainer-section {
    padding: 2rem;
    max-width: 1200px;
    margin: 0 auto;
}

.aim-trainer-container {
    display: grid;
    grid-template-columns: 350px 1fr;
    gap: 2rem;
    margin-top: 2rem;
}

.aim-controls {
    background: var(--color-gray);
    padding: 1.5rem;
    border-radius: 10px;
    border-left: 4px solid var(--color-primary);
}

.control-group {
    margin-bottom: 1.5rem;
}

.control-group label {
    display: block;
    margin-bottom: 0.5rem;
    color: var(--color-primary);
    font-weight: bold;
}

.control-group select,
.control-group input[type="range"] {
    width: 100%;
    padding: 0.5rem;
    background: #1a1a1a;
    color: white;
    border: 1px solid #444;
    border-radius: 5px;
}

.sensitivity-display {
    display: flex;
    justify-content: space-between;
    margin-top: 0.5rem;
    color: #ccc;
    font-size: 0.9rem;
}

.audio-controls {
    background: rgba(255, 107, 53, 0.1);
    padding: 1rem;
    border-radius: 8px;
    margin: 1.5rem 0;
}

.audio-controls h4 {
    color: var(--color-primary);
    margin-bottom: 1rem;
}

.weapon-stats {
    background: rgba(255, 107, 53, 0.1);
    padding: 1rem;
    border-radius: 8px;
    margin-top: 1rem;
}

.stat-row {
    display: flex;
    justify-content: space-between;
    margin-bottom: 0.5rem;
    font-size: 0.9rem;
}

.stat-label {
    color: #ccc;
}

.stat-value {
    color: var(--color-gold);
    font-weight: bold;
}

.spray-tip {
    background: rgba(255, 107, 53, 0.2);
    padding: 1rem;
    border-radius: 8px;
    margin-top: 1rem;
    font-style: italic;
    color: #ffd700;
}

.aim-canvas-container {
    position: relative;
    background: #1a1a1a;
    border-radius: 10px;
    overflow: hidden;
    border: 2px solid var(--color-primary);
}

#aimCanvas {
    width: 100%;
    height: 600px;
    display: block;
    cursor: crosshair;
}

.aim-stats {
    position: absolute;
    top: 1rem;
    left: 1rem;
    background: rgba(0, 0, 0, 0.8);
    padding: 1rem;
    border-radius: 8px;
    color: white;
    text-align: center;
}

.aim-stats div:first-child {
    margin-bottom: 0.5rem;
    color: #ccc;
}

#accuracyValue {
    font-size: 1.5rem;
    font-weight: bold;
    color: var(--color-gold);
    margin-bottom: 0.5rem;
}

.btn-small {
    background: var(--color-primary);
    color: white;
    border: none;
    padding: 0.5rem 1rem;
    border-radius: 5px;
    cursor: pointer;
    font-size: 0.8rem;
}

.practice-modes {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 1rem;
    margin-top: 2rem;
}

.practice-mode {
    background: var(--color-gray);
    padding: 1.5rem;
    border-radius: 10px;
    text-align: center;
    cursor: pointer;
    transition: all 0.3s ease;
    border: 2px solid transparent;
}

.practice-mode:hover {
    border-color: var(--color-primary);
    transform: translateY(-2px);
}

.practice-mode.active {
    border-color: var(--color-gold);
    background: rgba(255, 107, 53, 0.1);
}

.mode-icon {
    font-size: 2rem;
    margin-bottom: 0.5rem;
}

.mode-name {
    font-weight: bold;
    color: var(--color-primary);
    margin-bottom: 0.5rem;
}

.mode-desc {
    color: #ccc;
    font-size: 0.9rem;
}

/* Header Audio Controls */
.header-controls {
    display: flex;
    gap: 1rem;
    align-items: center;
    justify-content: center;
    margin-top: 1rem;
}

.audio-control-btn {
<button id="testSoundsBtn" class="btn-small" data-i18n="testSounds">Test Sounds</button>
    background: var(--color-primary);
    color: white;
    border: none;
    padding: 0.5rem;
    border-radius: 50%;
    width: 40px;
    height: 40px;
    cursor: pointer;
    font-size: 1.2rem;
}

.audio-notice {
    margin-top: 2rem;
    padding: 1rem;
    background: rgba(255, 107, 53, 0.1);
    border-radius: 8px;
    text-align: center;
}

.audio-notice p {
    margin: 0;
    color: var(--color-gold);
}

/* Responsividade do Simulador */
@media (max-width: 968px) {
    .aim-trainer-container {
        grid-template-columns: 1fr;
    }
    
    .aim-controls {
        order: 2;
    }
    
    .aim-canvas-container {
        order: 1;
    }
    
    #aimCanvas {
        height: 400px;
    }
}

@media (max-width: 480px) {
    .aim-trainer-section {
        padding: 1rem;
    }
    
    #aimCanvas {
        height: 300px;
    }
    
    .practice-modes {
        grid-template-columns: 1fr;
    }
    
    .header-controls {
        flex-direction: column;
        gap: 0.5rem;
    }
}
    │
    ├── 📁 js/                            ⚙️ **PASTA JAVASCRIPT** (criar dentro de assets)
    │   ├── 📄 script.js
    // No início do script.js, adicione:
import './audio-manager.js'; // Se usar modules
// OU adicione no HTML: <script src="assets/js/audio-manager.js"></script>
    │   ├── 📄 aim-trainer.js
    // No arquivo assets/js/aim-trainer.js, adicione:

setupAudioControls() {
    const musicVolumeSlider = document.getElementById('musicVolume');
    const sfxVolumeSlider = document.getElementById('sfxVolume');
    const muteToggle = document.getElementById('muteToggle');
    const testSoundsBtn = document.getElementById('testSoundsBtn');

    if (musicVolumeSlider) {
        musicVolumeSlider.addEventListener('input', (e) => {
            audioManager.setMusicVolume(parseInt(e.target.value) / 100);
        });
    }

    if (sfxVolumeSlider) {
        sfxVolumeSlider.addEventListener('input', (e) => {
            audioManager.setSfxVolume(parseInt(e.target.value) / 100);
        });
    }

    if (muteToggle) {
        muteToggle.addEventListener('click', () => {
            const isMuted = audioManager.toggleMute();
            muteToggle.textContent = isMuted ? '🔇' : '🔊';
            muteToggle.title = isMuted ? 'Unmute' : 'Mute';
        });
    }

    if (testSoundsBtn) {
        testSoundsBtn.addEventListener('click', () => {
            audioManager.testAllWeaponSounds();
        });
    }
}
    │   ├── 📄 storage.js
    // === SISTEMA DE SALVAMENTO DE CONFIGURAÇÕES ===
class StorageManager {
    constructor() {
        this.storageKey = 'pubgCoachSettings';
        this.defaultSettings = {
            savedConfigs: [],
            favoriteWeapons: [],
            customSensitivity: {},
            practiceStats: {
                totalShots: 0,
                hits: 0,
                accuracy: 0,
                sessions: 0
            }
        };
    }

    // Carregar todas as configurações
    loadSettings() {
        const saved = localStorage.getItem(this.storageKey);
        if (saved) {
            return JSON.parse(saved);
        }
        return this.defaultSettings;
    }

    // Salvar configurações
    saveSettings(settings) {
        localStorage.setItem(this.storageKey, JSON.stringify(settings));
    }

    // Salvar configuração de dispositivo
    saveDeviceConfig(deviceName, map, settings) {
        const currentSettings = this.loadSettings();
        
        const newConfig = {
            id: Date.now(),
            deviceName: deviceName,
            map: map,
            settings: settings,
            timestamp: new Date().toISOString()
        };

        // Manter apenas as 10 configurações mais recentes
        currentSettings.savedConfigs.unshift(newConfig);
        if (currentSettings.savedConfigs.length > 10) {
            currentSettings.savedConfigs = currentSettings.savedConfigs.slice(0, 10);
        }

        this.saveSettings(currentSettings);
        return newConfig;
    }

    // Salvar sensibilidade personalizada
    saveCustomSensitivity(weaponId, scope, values) {
        const currentSettings = this.loadSettings();
        
        if (!currentSettings.customSensitivity[weaponId]) {
            currentSettings.customSensitivity[weaponId] = {};
        }
        
        currentSettings.customSensitivity[weaponId][scope] = values;
        this.saveSettings(currentSettings);
    }

    // Adicionar arma aos favoritos
    toggleFavoriteWeapon(weaponId) {
        const currentSettings = this.loadSettings();
        const index = currentSettings.favoriteWeapons.indexOf(weaponId);
        
        if (index > -1) {
            currentSettings.favoriteWeapons.splice(index, 1);
        } else {
            currentSettings.favoriteWeapons.push(weaponId);
        }
        
        this.saveSettings(currentSettings);
        return currentSettings.favoriteWeapons;
    }

    // Atualizar estatísticas de treino
    updatePracticeStats(shots, hits) {
        const currentSettings = this.loadSettings();
        
        currentSettings.practiceStats.totalShots += shots;
        currentSettings.practiceStats.hits += hits;
        currentSettings.practiceStats.sessions += 1;
        currentSettings.practiceStats.accuracy = 
            (currentSettings.practiceStats.hits / currentSettings.practiceStats.totalShots) * 100;
        
        this.saveSettings(currentSettings);
        return currentSettings.practiceStats;
    }

    // Exportar configurações
    exportSettings() {
        const settings = this.loadSettings();
        const dataStr = JSON.stringify(settings, null, 2);
        const dataUri = 'data:application/json;charset=utf-8,'+ encodeURIComponent(dataStr);
        
        const exportFileDefaultName = `pubg_coach_backup_${new Date().toISOString().split('T')[0]}.json`;
        
        const linkElement = document.createElement('a');
        linkElement.setAttribute('href', dataUri);
        linkElement.setAttribute('download', exportFileDefaultName);
        linkElement.click();
    }

    // Importar configurações
    importSettings(file) {
        return new Promise((resolve, reject) => {
            const reader = new FileReader();
            
            reader.onload = (e) => {
                try {
                    const importedSettings = JSON.parse(e.target.result);
                    this.saveSettings(importedSettings);
                    resolve(importedSettings);
                } catch (error) {
                    reject('Invalid file format');
                }
            };
            
            reader.onerror = () => reject('Error reading file');
            reader.readAsText(file);
        });
    }

    // Limpar todos os dados
    clearAllData() {
        localStorage.removeItem(this.storageKey);
        return this.defaultSettings;
    }
}

// Instância global do gerenciador de armazenamento
const storageManager = new StorageManager();
    │   └── 📄 audio-manager.js
    // === SISTEMA DE GERENCIAMENTO DE ÁUDIO ===
class AudioManager {
    constructor() {
        this.audioContext = null;
        this.sounds = {};
        this.backgroundMusic = null;
        this.isMusicPlaying = false;
        this.musicVolume = 0.3;
        this.sfxVolume = 0.5;
        this.isMuted = false;
        
        this.init();
    }

    init() {
        // Inicializar AudioContext
        try {
            this.audioContext = new (window.AudioContext || window.webkitAudioContext)();
        } catch (error) {
            console.warn('AudioContext não suportado:', error);
        }

        // Carregar sons
        this.loadSounds();
        
        // Configurar eventos de usuário para destravar áudio
        this.setupUserInteraction();
    }

    setupUserInteraction() {
        // Destravar áudio na primeira interação do usuário
        const unlockAudio = () => {
            if (this.audioContext && this.audioContext.state === 'suspended') {
                this.audioContext.resume();
            }
            
            // Iniciar música de fundo após interação
            if (!this.isMusicPlaying) {
                this.playBackgroundMusic();
            }
            
            // Remover event listeners após primeira interação
            document.removeEventListener('click', unlockAudio);
            document.removeEventListener('touchstart', unlockAudio);
        };

        document.addEventListener('click', unlockAudio);
        document.addEventListener('touchstart', unlockAudio);
    }

    loadSounds() {
        // Mapeamento de sons das armas
        const weaponSounds = {
            'm416': 'assets/audio/m416-shot.mp3',
            'akm': 'assets/audio/akm-shot.mp3',
            'ump45': 'assets/audio/ump45-shot.mp3',
            'scar_l': 'assets/audio/scar-l-shot.mp3',
            'm762': 'assets/audio/m762-shot.mp3',
            'aug': 'assets/audio/aug-shot.mp3'
        };

        // Carregar cada som
        Object.entries(weaponSounds).forEach(([weaponId, soundPath]) => {
            this.loadSound(weaponId, soundPath);
        });

        // Carregar música de fundo
        this.loadBackgroundMusic('assets/audio/opening-music.mp3');
    }

    loadSound(soundId, soundPath) {
        fetch(soundPath)
            .then(response => response.arrayBuffer())
            .then(arrayBuffer => this.audioContext.decodeAudioData(arrayBuffer))
            .then(audioBuffer => {
                this.sounds[soundId] = audioBuffer;
            })
            .catch(error => {
                console.warn(`Erro ao carregar som ${soundId}:`, error);
            });
    }

    loadBackgroundMusic(musicPath) {
        this.backgroundMusic = new Audio(musicPath);
        this.backgroundMusic.loop = true;
        this.backgroundMusic.volume = this.musicVolume;
        
        // Configurar eventos da música
        this.backgroundMusic.addEventListener('canplaythrough', () => {
            console.log('Música de fundo carregada e pronta');
        });
        
        this.backgroundMusic.addEventListener('error', (e) => {
            console.warn('Erro ao carregar música de fundo:', e);
        });
    }

    playBackgroundMusic() {
        if (this.backgroundMusic && !this.isMuted && !this.isMusicPlaying) {
            this.backgroundMusic.play()
                .then(() => {
                    this.isMusicPlaying = true;
                    console.log('Música de fundo iniciada');
                })
                .catch(error => {
                    console.warn('Não foi possível reproduzir música de fundo:', error);
                });
        }
    }

    stopBackgroundMusic() {
        if (this.backgroundMusic && this.isMusicPlaying) {
            this.backgroundMusic.pause();
            this.backgroundMusic.currentTime = 0;
            this.isMusicPlaying = false;
        }
    }

    playWeaponSound(weaponId) {
        if (this.isMuted || !this.sounds[weaponId] || !this.audioContext) {
            return;
        }

        try {
            const source = this.audioContext.createBufferSource();
            const gainNode = this.audioContext.createGain();
            
            source.buffer = this.sounds[weaponId];
            gainNode.gain.value = this.sfxVolume;
            
            source.connect(gainNode);
            gainNode.connect(this.audioContext.destination);
            
            source.start(0);
            
            // Limpar após tocar
            source.onended = () => {
                source.disconnect();
                gainNode.disconnect();
            };
        } catch (error) {
            console.warn('Erro ao reproduzir som da arma:', error);
        }
    }

    playRandomWeaponSound() {
        const weapons = Object.keys(this.sounds);
        if (weapons.length > 0) {
            const randomWeapon = weapons[Math.floor(Math.random() * weapons.length)];
            this.playWeaponSound(randomWeapon);
        }
    }

    setMusicVolume(volume) {
        this.musicVolume = Math.max(0, Math.min(1, volume));
        if (this.backgroundMusic) {
            this.backgroundMusic.volume = this.musicVolume;
        }
    }

    setSfxVolume(volume) {
        this.sfxVolume = Math.max(0, Math.min(1, volume));
    }

    toggleMute() {
        this.isMuted = !this.isMuted;
        
        if (this.backgroundMusic) {
            this.backgroundMusic.muted = this.isMuted;
        }
        
        return this.isMuted;
    }

    // Efeitos sonoros especiais
    playHitSound() {
        // Criar som de acerto simples (pode ser substituído por arquivo posteriormente)
        if (this.isMuted || !this.audioContext) return;
        
        try {
            const oscillator = this.audioContext.createOscillator();
            const gainNode = this.audioContext.createGain();
            
            oscillator.type = 'sine';
            oscillator.frequency.setValueAtTime(800, this.audioContext.currentTime);
            oscillator.frequency.exponentialRampToValueAtTime(300, this.audioContext.currentTime + 0.1);
            
            gainNode.gain.setValueAtTime(this.sfxVolume * 0.3, this.audioContext.currentTime);
            gainNode.gain.exponentialRampToValueAtTime(0.001, this.audioContext.currentTime + 0.1);
            
            oscillator.connect(gainNode);
            gainNode.connect(this.audioContext.destination);
            
            oscillator.start();
            oscillator.stop(this.audioContext.currentTime + 0.1);
        } catch (error) {
            console.warn('Erro ao reproduzir som de acerto:', error);
        }
    }

    playReloadSound() {
        // Som de recarga simples
        if (this.isMuted || !this.audioContext) return;
        
        try {
            const oscillator = this.audioContext.createOscillator();
            const gainNode = this.audioContext.createGain();
            
            oscillator.type = 'sawtooth';
            oscillator.frequency.setValueAtTime(200, this.audioContext.currentTime);
            oscillator.frequency.linearRampToValueAtTime(100, this.audioContext.currentTime + 0.5);
            
            gainNode.gain.setValueAtTime(this.sfxVolume * 0.2, this.audioContext.currentTime);
            gainNode.gain.exponentialRampToValueAtTime(0.001, this.audioContext.currentTime + 0.5);
            
            oscillator.connect(gainNode);
            gainNode.connect(this.audioContext.destination);
            
            oscillator.start();
            oscillator.stop(this.audioContext.currentTime + 0.5);
        } catch (error) {
            console.warn('Erro ao reproduzir som de recarga:', error);
        }
    }
}

// Instância global do gerenciador de áudio
const audioManager = new AudioManager();
    assets/audio/
├── 📄 vlog-beat-background-349853.mp3    # Sua música
├── 📄 m416-shot.mp3                      # (Opcional - se quiser adicionar depois)
├── 📄 akm-shot.mp3                       # (Opcional)
├── 📄 ump45-shot.mp3                     # (Opcional)
├── 📄 scar-l-shot.mp3                    # (Opcional)
├── 📄 m762-shot.mp3                      # (Opcional)
└── 📄 aug-shot.mp3                       # (Opcional)
    // === SISTEMA DE GERENCIAMENTO DE ÁUDIO ===
class AudioManager {
    constructor() {
        this.audioContext = null;
        this.backgroundMusic = null;
        this.isMusicPlaying = false;
        this.musicVolume = 0.4;
        this.sfxVolume = 0.6;
        this.isMuted = false;
        
        this.init();
    }

    init() {
        // Inicializar AudioContext
        try {
            this.audioContext = new (window.AudioContext || window.webkitAudioContext)();
            console.log('AudioContext inicializado com sucesso');
        } catch (error) {
            console.warn('AudioContext não suportado:', error);
            this.createFallbackAudioSystem();
            return;
        }

        // Carregar música de fundo do arquivo
        this.loadBackgroundMusic();
        
        // Configurar eventos de usuário para destravar áudio
        this.setupUserInteraction();
    }

    createFallbackAudioSystem() {
        console.log('Usando sistema de áudio fallback');
        // Sistema simples baseado em HTML5 Audio para dispositivos sem Web Audio API
        this.fallbackSounds = {};
    }

    loadBackgroundMusic() {
        this.backgroundMusic = new Audio('assets/audio/vlog-beat-background-349853.mp3');
        this.backgroundMusic.loop = true;
        this.backgroundMusic.volume = this.musicVolume;
        
        this.backgroundMusic.addEventListener('canplaythrough', () => {
            console.log('Música de fundo carregada e pronta');
        });
        
        this.backgroundMusic.addEventListener('error', (e) => {
            console.warn('Erro ao carregar música de fundo, usando áudio procedural:', e);
            this.createProceduralMusic();
        });
    }

    createProceduralMusic() {
        // Música procedural de fallback
        try {
            if (!this.audioContext) return;

            const createNote = (frequency, duration, startTime, volume = 0.2) => {
                const oscillator = this.audioContext.createOscillator();
                const gainNode = this.audioContext.createGain();
                
                oscillator.type = 'sine';
                oscillator.frequency.value = frequency;
                
                gainNode.gain.setValueAtTime(volume, startTime);
                gainNode.gain.exponentialRampToValueAtTime(0.001, startTime + duration);
                
                oscillator.connect(gainNode);
                gainNode.connect(this.audioContext.destination);
                
                oscillator.start(startTime);
                oscillator.stop(startTime + duration);
            };

            // Padrão musical simples
            const melody = [261.63, 329.63, 392.00, 523.25, 392.00, 329.63];
            const now = this.audioContext.currentTime;
            
            melody.forEach((freq, index) => {
                createNote(freq, 0.5, now + (index * 0.6));
                createNote(freq * 1.5, 0.3, now + (index * 0.6) + 0.1, 0.1);
            });

            // Repetir a cada 4 segundos
            setTimeout(() => this.createProceduralMusic(), 4000);
            
        } catch (error) {
            console.warn('Erro na música procedural:', error);
        }
    }

    setupUserInteraction() {
        const unlockAudio = () => {
            if (this.audioContext && this.audioContext.state === 'suspended') {
                this.audioContext.resume().then(() => {
                    console.log('AudioContext destravado');
                    this.playBackgroundMusic();
                });
            } else {
                this.playBackgroundMusic();
            }
            
            document.removeEventListener('click', unlockAudio);
            document.removeEventListener('touchstart', unlockAudio);
        };

        document.addEventListener('click', unlockAudio);
        document.addEventListener('touchstart', unlockAudio);
    }

    playBackgroundMusic() {
        if (this.backgroundMusic && !this.isMuted && !this.isMusicPlaying) {
            this.backgroundMusic.play()
                .then(() => {
                    this.isMusicPlaying = true;
                    console.log('Música de fundo iniciada');
                })
                .catch(error => {
                    console.warn('Não foi possível reproduzir música de fundo:', error);
                    this.createProceduralMusic();
                });
        }
    }

    stopBackgroundMusic() {
        if (this.backgroundMusic && this.isMusicPlaying) {
            this.backgroundMusic.pause();
            this.backgroundMusic.currentTime = 0;
            this.isMusicPlaying = false;
        }
    }

    playWeaponSound(weaponId) {
        if (this.isMuted) return;

        if (this.audioContext) {
            this.playWeaponSoundWebAudio(weaponId);
        } else {
            this.playWeaponSoundFallback(weaponId);
        }
    }

    playWeaponSoundWebAudio(weaponId) {
        try {
            const config = this.getWeaponSoundConfig(weaponId);
            
            // Criar oscilador principal para o tiro
            const oscillator = this.audioContext.createOscillator();
            const gainNode = this.audioContext.createGain();
            const filter = this.audioContext.createBiquadFilter();
            
            // Configurar som base
            oscillator.type = config.type;
            oscillator.frequency.setValueAtTime(config.frequency, this.audioContext.currentTime);
            
            // Efeito de decay do tiro
            gainNode.gain.setValueAtTime(this.sfxVolume * config.volume, this.audioContext.currentTime);
            gainNode.gain.exponentialRampToValueAtTime(0.001, this.audioContext.currentTime + config.duration);
            
            // Filtro para dar característica de "tiro"
            filter.type = 'bandpass';
            filter.frequency.value = 800;
            filter.Q.value = 1.0;
            
            // Conectar e tocar
            oscillator.connect(filter);
            filter.connect(gainNode);
            gainNode.connect(this.audioContext.destination);
            
            oscillator.start();
            oscillator.stop(this.audioContext.currentTime + config.duration);
            
            // Adicionar ruído branco para realismo
            this.addGunshotNoise(config);
            
        } catch (error) {
            console.warn('Erro no som Web Audio:', error);
            this.playWeaponSoundFallback(weaponId);
        }
    }

    addGunshotNoise(config) {
        try {
            const bufferSize = this.audioContext.sampleRate * config.duration;
            const noiseBuffer = this.audioContext.createBuffer(1, bufferSize, this.audioContext.sampleRate);
            const output = noiseBuffer.getChannelData(0);
            
            // Gerar ruído branco
            for (let i = 0; i < bufferSize; i++) {
                output[i] = Math.random() * 2 - 1;
            }
            
            const noiseSource = this.audioContext.createBufferSource();
            const noiseGain = this.audioContext.createGain();
            const noiseFilter = this.audioContext.createBiquadFilter();
            
            noiseSource.buffer = noiseBuffer;
            noiseGain.gain.setValueAtTime(this.sfxVolume * config.volume * 0.3, this.audioContext.currentTime);
            noiseGain.gain.exponentialRampToValueAtTime(0.001, this.audioContext.currentTime + config.duration * 0.5);
            
            noiseFilter.type = 'highpass';
            noiseFilter.frequency.value = 500;
            
            noiseSource.connect(noiseFilter);
            noiseFilter.connect(noiseGain);
            noiseGain.connect(this.audioContext.destination);
            
            noiseSource.start();
            
        } catch (error) {
            console.warn('Erro ao adicionar ruído:', error);
        }
    }

    playWeaponSoundFallback(weaponId) {
        // Fallback usando osciladores simples mesmo sem AudioContext
        try {
            const config = this.getWeaponSoundConfig(weaponId);
            
            // Criar oscilador usando Web Audio API básica
            const oscillator = this.audioContext.createOscillator();
            const gainNode = this.audioContext.createGain();
            
            oscillator.type = config.type;
            oscillator.frequency.value = config.frequency;
            
            gainNode.gain.value = this.sfxVolume * config.volume;
            gainNode.gain.exponentialRampToValueAtTime(0.001, this.audioContext.currentTime + config.duration);
            
            oscillator.connect(gainNode);
            gainNode.connect(this.audioContext.destination);
            
            oscillator.start();
            oscillator.stop(this.audioContext.currentTime + config.duration);
            
        } catch (error) {
            console.warn('Erro no fallback de áudio:', error);
        }
    }

    getWeaponSoundConfig(weaponId) {
        const configs = {
            'm416': { 
                type: 'sawtooth', 
                frequency: 120, 
                duration: 0.15, 
                volume: 0.5,
                description: "Rifle estável com recuo moderado"
            },
            'akm': { 
                type: 'sawtooth', 
                frequency: 90, 
                duration: 0.18, 
                volume: 0.7,
                description: "Rifle potente com recuo forte"
            },
            'ump45': { 
                type: 'square', 
                frequency: 180, 
                duration: 0.12, 
                volume: 0.4,
                description: "SMG rápida com recuo baixo"
            },
            'scar_l': { 
                type: 'sawtooth', 
                frequency: 110, 
                duration: 0.16, 
                volume: 0.55,
                description: "Rifle preciso com som característico"
            },
            'm762': { 
                type: 'sawtooth', 
                frequency: 85, 
                duration: 0.2, 
                volume: 0.75,
                description: "Rifle de alto dano com recuo agressivo"
            },
            'aug': { 
                type: 'sine', 
                frequency: 130, 
                duration: 0.14, 
                volume: 0.45,
                description: "Rifle de assalto premium com som suave"
            }
        };
        
        return configs[weaponId] || configs['m416'];
    }

    playHitSound() {
        if (this.isMuted) return;

        if (this.audioContext) {
            try {
                const oscillator = this.audioContext.createOscillator();
                const gainNode = this.audioContext.createGain();
                
                oscillator.type = 'sine';
                oscillator.frequency.setValueAtTime(800, this.audioContext.currentTime);
                oscillator.frequency.exponentialRampToValueAtTime(400, this.audioContext.currentTime + 0.1);
                
                gainNode.gain.setValueAtTime(this.sfxVolume * 0.4, this.audioContext.currentTime);
                gainNode.gain.exponentialRampToValueAtTime(0.001, this.audioContext.currentTime + 0.1);
                
                oscillator.connect(gainNode);
                gainNode.connect(this.audioContext.destination);
                
                oscillator.start();
                oscillator.stop(this.audioContext.currentTime + 0.1);
                
            } catch (error) {
                console.warn('Erro no som de acerto:', error);
            }
        }
    }

    playReloadSound() {
        if (this.isMuted) return;

        if (this.audioContext) {
            try {
                // Som de carregamento de pente
                const oscillator = this.audioContext.createOscillator();
                const gainNode = this.audioContext.createGain();
                
                oscillator.type = 'triangle';
                oscillator.frequency.setValueAtTime(150, this.audioContext.currentTime);
                oscillator.frequency.linearRampToValueAtTime(80, this.audioContext.currentTime + 0.3);
                
                gainNode.gain.setValueAtTime(this.sfxVolume * 0.3, this.audioContext.currentTime);
                gainNode.gain.exponentialRampToValueAtTime(0.001, this.audioContext.currentTime + 0.3);
                
                oscillator.connect(gainNode);
                gainNode.connect(this.audioContext.destination);
                
                oscillator.start();
                oscillator.stop(this.audioContext.currentTime + 0.3);
                
            } catch (error) {
                console.warn('Erro no som de recarga:', error);
            }
        }
    }

    playHeadshotSound() {
        if (this.isMuted) return;

        if (this.audioContext) {
            try {
                const oscillator = this.audioContext.createOscillator();
                const gainNode = this.audioContext.createGain();
                
                oscillator.type = 'sine';
                oscillator.frequency.setValueAtTime(1200, this.audioContext.currentTime);
                oscillator.frequency.exponentialRampToValueAtTime(300, this.audioContext.currentTime + 0.2);
                
                gainNode.gain.setValueAtTime(this.sfxVolume * 0.6, this.audioContext.currentTime);
                gainNode.gain.exponentialRampToValueAtTime(0.001, this.audioContext.currentTime + 0.2);
                
                oscillator.connect(gainNode);
                gainNode.connect(this.audioContext.destination);
                
                oscillator.start();
                oscillator.stop(this.audioContext.currentTime + 0.2);
                
            } catch (error) {
                console.warn('Erro no som de headshot:', error);
            }
        }
    }

    setMusicVolume(volume) {
        this.musicVolume = Math.max(0, Math.min(1, volume));
        if (this.backgroundMusic) {
            this.backgroundMusic.volume = this.musicVolume;
        }
    }

    setSfxVolume(volume) {
        this.sfxVolume = Math.max(0, Math.min(1, volume));
    }

    toggleMute() {
        this.isMuted = !this.isMuted;
        
        if (this.backgroundMusic) {
            this.backgroundMusic.muted = this.isMuted;
        }
        
        if (this.isMuted) {
            this.stopBackgroundMusic();
        } else {
            this.playBackgroundMusic();
        }
        
        return this.isMuted;
    }

    // Testar todos os sons
    testAllWeaponSounds() {
        const weapons = ['m416', 'akm', 'ump45', 'scar_l', 'm762', 'aug'];
        let index = 0;
        
        const playNextSound = () => {
            if (index < weapons.length) {
                this.playWeaponSound(weapons[index]);
                index++;
                setTimeout(playNextSound, 500);
            }
        };
        
        playNextSound();
    }
}

// Instância global do gerenciador de áudio
const audioManager = new AudioManager();
    // === SISTEMA DE GERENCIAMENTO DE ÁUDIO ===
class AudioManager {
    constructor() {
        this.audioContext = null;
        this.sounds = {};
        this.backgroundMusic = null;
        this.isMusicPlaying = false;
        this.musicVolume = 0.3;
        this.sfxVolume = 0.5;
        this.isMuted = false;
        
        this.init();
    }

    init() {
        // Inicializar AudioContext
        try {
            this.audioContext = new (window.AudioContext || window.webkitAudioContext)();
            console.log('AudioContext inicializado com sucesso');
        } catch (error) {
            console.warn('AudioContext não suportado:', error);
            return;
        }

        // Configurar eventos de usuário para destravar áudio
        this.setupUserInteraction();
        
        // Inicializar música de fundo procedural
        this.createBackgroundMusic();
    }

    setupUserInteraction() {
        const unlockAudio = () => {
            if (this.audioContext && this.audioContext.state === 'suspended') {
                this.audioContext.resume().then(() => {
                    console.log('AudioContext destravado');
                });
            }
            
            // Iniciar música de fundo após interação
            if (!this.isMusicPlaying && !this.isMuted) {
                this.playBackgroundMusic();
            }
            
            // Remover event listeners após primeira interação
            document.removeEventListener('click', unlockAudio);
            document.removeEventListener('touchstart', unlockAudio);
        };

        document.addEventListener('click', unlockAudio);
        document.addEventListener('touchstart', unlockAudio);
    }

    createBackgroundMusic() {
        // Criar música procedural épica
        try {
            if (!this.audioContext) return;

            // Configurar nós de áudio
            const oscillator1 = this.audioContext.createOscillator();
            const oscillator2 = this.audioContext.createOscillator();
            const gainNode1 = this.audioContext.createGain();
            const gainNode2 = this.audioContext.createGain();
            const filter = this.audioContext.createBiquadFilter();
            
            // Configurar oscillators
            oscillator1.type = 'sine';
            oscillator1.frequency.value = 220; // Lá
            oscillator2.type = 'triangle';
            oscillator2.frequency.value = 277.18; // Dó#
            
            // Configurar filter
            filter.type = 'lowpass';
            filter.frequency.value = 800;
            
            // Configurar ganhos
            gainNode1.gain.value = this.musicVolume * 0.3;
            gainNode2.gain.value = this.musicVolume * 0.2;
            
            // Conectar nós
            oscillator1.connect(gainNode1);
            oscillator2.connect(gainNode2);
            gainNode1.connect(filter);
            gainNode2.connect(filter);
            filter.connect(this.audioContext.destination);
            
            // Iniciar oscillators
            oscillator1.start();
            oscillator2.start();
            
            // Criar padrão musical
            this.createMusicPattern(oscillator1, oscillator2, gainNode1, gainNode2);
            
        } catch (error) {
            console.warn('Erro ao criar música procedural:', error);
        }
    }

    createMusicPattern(osc1, osc2, gain1, gain2) {
        const now = this.audioContext.currentTime;
        const bpm = 85;
        const beatDuration = 60 / bpm;
        
        // Padrão melódico épico
        const melody = [261.63, 293.66, 329.63, 349.23, 392.00, 440.00, 493.88, 523.25];
        
        melody.forEach((freq, index) => {
            const time = now + (index * beatDuration * 2);
            
            // Oscillator 1 - melodia principal
            osc1.frequency.setValueAtTime(freq, time);
            gain1.gain.setValueAtTime(this.musicVolume * 0.3, time);
            gain1.gain.exponentialRampToValueAtTime(0.01, time + beatDuration * 1.8);
            
            // Oscillator 2 - harmonia
            osc2.frequency.setValueAtTime(freq * 1.5, time + beatDuration);
            gain2.gain.setValueAtTime(this.musicVolume * 0.2, time + beatDuration);
            gain2.gain.exponentialRampToValueAtTime(0.01, time + beatDuration * 2.8);
        });
        
        // Repetir padrão
        setTimeout(() => {
            this.createMusicPattern(osc1, osc2, gain1, gain2);
        }, melody.length * beatDuration * 2 * 1000);
    }

    playBackgroundMusic() {
        if (this.audioContext && !this.isMuted && !this.isMusicPlaying) {
            this.isMusicPlaying = true;
            console.log('Música de fundo iniciada');
        }
    }

    stopBackgroundMusic() {
        this.isMusicPlaying = false;
    }

    playWeaponSound(weaponId) {
        if (this.isMuted || !this.audioContext) {
            return;
        }

        try {
            const oscillator = this.audioContext.createOscillator();
            const gainNode = this.audioContext.createGain();
            const filter = this.audioContext.createBiquadFilter();
            
            // Configurar baseado no tipo de arma
            const weaponConfig = this.getWeaponSoundConfig(weaponId);
            
            oscillator.type = weaponConfig.type;
            oscillator.frequency.setValueAtTime(weaponConfig.frequency, this.audioContext.currentTime);
            oscillator.frequency.exponentialRampToValueAtTime(weaponConfig.frequency * 0.3, this.audioContext.currentTime + weaponConfig.duration);
            
            filter.type = 'highpass';
            filter.frequency.value = 500;
            
            gainNode.gain.setValueAtTime(this.sfxVolume * weaponConfig.volume, this.audioContext.currentTime);
            gainNode.gain.exponentialRampToValueAtTime(0.001, this.audioContext.currentTime + weaponConfig.duration);
            
            oscillator.connect(filter);
            filter.connect(gainNode);
            gainNode.connect(this.audioContext.destination);
            
            oscillator.start();
            oscillator.stop(this.audioContext.currentTime + weaponConfig.duration);
            
        } catch (error) {
            console.warn('Erro ao reproduzir som da arma:', error);
        }
    }

    getWeaponSoundConfig(weaponId) {
        const configs = {
            'm416': { type: 'sawtooth', frequency: 180, duration: 0.1, volume: 0.4 },
            'akm': { type: 'sawtooth', frequency: 160, duration: 0.12, volume: 0.6 },
            'ump45': { type: 'square', frequency: 200, duration: 0.08, volume: 0.3 },
            'scar_l': { type: 'sawtooth', frequency: 190, duration: 0.09, volume: 0.35 },
            'm762': { type: 'sawtooth', frequency: 150, duration: 0.13, volume: 0.7 },
            'aug': { type: 'sine', frequency: 210, duration: 0.07, volume: 0.25 }
        };
        
        return configs[weaponId] || configs['m416'];
    }

    playHitSound() {
        if (this.isMuted || !this.audioContext) return;
        
        try {
            const oscillator = this.audioContext.createOscillator();
            const gainNode = this.audioContext.createGain();
            
            oscillator.type = 'sine';
            oscillator.frequency.setValueAtTime(800, this.audioContext.currentTime);
            oscillator.frequency.exponentialRampToValueAtTime(300, this.audioContext.currentTime + 0.1);
            
            gainNode.gain.setValueAtTime(this.sfxVolume * 0.3, this.audioContext.currentTime);
            gainNode.gain.exponentialRampToValueAtTime(0.001, this.audioContext.currentTime + 0.1);
            
            oscillator.connect(gainNode);
            gainNode.connect(this.audioContext.destination);
            
            oscillator.start();
            oscillator.stop(this.audioContext.currentTime + 0.1);
        } catch (error) {
            console.warn('Erro ao reproduzir som de acerto:', error);
        }
    }

    setMusicVolume(volume) {
        this.musicVolume = Math.max(0, Math.min(1, volume));
    }

    setSfxVolume(volume) {
        this.sfxVolume = Math.max(0, Math.min(1, volume));
    }

    toggleMute() {
        this.isMuted = !this.isMuted;
        
        if (this.isMuted) {
            this.stopBackgroundMusic();
        } else {
            this.playBackgroundMusic();
        }
        
        return this.isMuted;
    }
}

// Instância global do gerenciador de áudio
const audioManager = new AudioManager();
    │
    └── 📁 icons/                         🐔 **PASTA ÍCONES** (criar dentro de assets)
        ├── 📄 site.webmanifest
        {
  "name": "PubgCoachluciodevs",
  "short_name": "PUBG Coach",
  "description": "Professional PUBG Mobile coaching assistant - Powered by DeepSeek",
  "start_url": "/",
  "display": "standalone",
  "background_color": "#1a1a1a",
  "theme_color": "#ff6b35",
  "orientation": "portrait",
  "icons": [
    {
      "src": "favicon-16x16.png",
      "sizes": "16x16",
      "type": "image/png"
    },
    {
      "src": "favicon-32x32.png",
      "sizes": "32x32",
      "type": "image/png"
    },
    {
      "src": "apple-touch-icon.png",
      "sizes": "180x180",
      "type": "image/png"
    },
    {
      "src": "icon-512x512.png",
      "sizes": "512x512",
      "type": "image/png"
    }
  ],
  "categories": ["games", "entertainment", "education"]
}
        ├── 📄 apple-touch-icon.png
        ├── 📄 favicon-32x32.png
        ├── 📄 favicon-16x16.png
        └── 📄 icon-512x512.png
PubgCoachPro/                              
📁 READ.md
│
├── 📄 index.html                         
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>PUBG Chicken Dinner Coach Pro</title>
    <link rel="icon" type="image/png" href="images/favicon.png">
    <link rel="stylesheet" href="css/style.css">
</head>
<body>
    <!-- Header -->
    <header>
        <nav>
            <div class="logo">
                <h1>PUBG Chicken Dinner Coach Pro</h1>
            </div>
            <div class="nav-links">
                <a href="#sensitivity">Sensitivity</a>
                <a href="#strategies">Strategies</a>
                <a href="#graphics">Graphics</a>
                <a href="#crates">Crates</a>
                <a href="#nickname">Nickname</a>
            </div>
        </nav>
    </header>

    <main>
        <!-- Graphics Optimizer Section -->
<section id="graphics" class="feature-section">
    <h2>Graphics Optimizer</h2>
    <button onclick="optimizeGraphics()">Optimize My Device</button>
    <div id="graphicsSettings">
        <p>Click the button above to get optimized graphics settings.</p>
    </div>
</section>

<!-- Crate Simulator Section -->
<section id="crates" class="feature-section">
    <h2>Crate Simulator</h2>
    <button onclick="openCrate()">Open Crate (10 UC)</button>
    <div id="crateResult">
        <p>Open a crate to see what you get!</p>
    </div>
</section>

<!-- Nickname Generator Section -->
<section id="nickname" class="feature-section">
    <h2>Nickname Generator</h2>
    <input type="text" id="baseName" placeholder="Your name" value="Player">
    <select id="nicknameStyle">
        <option value="professional">Professional</option>
        <option value="aggressive">Aggressive</option>
        <option value="tactical">Tactical</option>
        <option value="funny">Funny</option>
    </select>
    <button onclick="generateNickname()">Generate</button>
    <button onclick="copyNickname()">Copy</button>
    <div id="nicknameResult">Your nickname will appear here</div>
</section>
        <!-- Sensitivity Trainer Section -->
        <section id="sensitivity" class="feature-section">
            <h2>Sensitivity Trainer</h2>
            <div class="sensitivity-tester">
                <select id="weaponSelect">
                    <option value="akm">AKM</option>
                    <option value="m416">M416</option>
                    <option value="scar-l">SCAR-L</option>
                </select>
                <div class="target-area" id="targetArea">
                    <div class="target" id="target"></div>
                </div>
                <div class="sensitivity-info">
                    <p id="weaponStats">Select a weapon to see recommended settings.</p>
                </div>
            </div>
        </section>

        <!-- Strategies Section -->
        <section id="strategies" class="feature-section">
            <h2>Battle Strategies</h2>
            <div class="strategy-content">
                <div class="strategy-category">
                    <h3>Landing Phase</h3>
                    <ul>
                        <li><strong>Hot Drop:</strong> School, Pochinki - high risk, high reward.</li>
                        <li><strong>Safe Drop:</strong> Georgopol containers, Farm - medium loot.</li>
                        <li><strong>Stealth Drop:</strong> Stalber, Primorsk - avoid early combat.</li>
                    </ul>
                </div>
                <div class="strategy-category">
                    <h3>Mid-Game Rotation</h3>
                    <ul>
                        <li><strong>Edge Play:</strong> Stay at the safe zone edge to clear enemies behind.</li>
                        <li><strong>Center Hold:</strong> Secure a central position with 360-degree vision.</li>
                        <li><strong>Early Rotate:</strong> Move to opposite corner of next zone early.</li>
                    </ul>
                </div>
                <div class="strategy-category">
                    <h3>Combat Tactics</h3>
                    <ul>
                        <li><strong>Peek and Shoot:</strong> Use cover, shoot, and return to cover.</li>
                        <li><strong>Flanking:</strong> Attack from sides while team distracts.</li>
                        <li><strong>Grenade Tactics:</strong> Use smoke for revives, flash for rushing.</li>
                    </ul>
                </div>
            </div>
        </section>

        <!-- Graphics Optimizer Section -->
        <section id="graphics" class="feature-section">
            <h2>Graphics Optimizer</h2>
            <div class="graphics-optimizer">
                <button class="optimize-btn" onclick="optimizeGraphics()">
                    Optimize My Device
                </button>
                <div id="graphicsSettings">
                    <p>Click the button above to get optimized graphics settings for your device.</p>
                </div>
            </div>
        </section>

        <!-- Crate Simulator Section -->
        <section id="crates" class="feature-section">
            <h2>Crate Simulator</h2>
            <div class="crate-simulator">
                <button class="crate-btn" onclick="openCrate()">
                    Open Crate (10 UC)
                </button>
                <div id="crateResult">
                    <p>Open a crate to see what you get!</p>
                </div>
            </div>
        </section>

        <!-- Nickname Generator Section -->
        <section id="nickname" class="feature-section">
            <h2>Nickname Generator</h2>
            <div class="nickname-generator">
                <div class="nickname-controls">
                    <input type="text" id="baseName" class="nickname-input" placeholder="Your name" value="Player">
                    <select id="nicknameStyle" class="nickname-select">
                        <option value="professional">Professional</option>
                        <option value="aggressive">Aggressive</option>
                        <option value="tactical">Tactical</option>
                        <option value="funny">Funny</option>
                    </select>
                </div>
                <div class="nickname-buttons">
                    <button class="nickname-btn" onclick="generateNickname()">Generate</button>
                    <button class="nickname-btn" onclick="copyNickname()">Copy</button>
                </div>
                <div id="nicknameResult">
                    Your nickname will appear here
                </div>
            </div>
        </section>
    </main>

    <script src="js/app.js"></script>
</body>
</html>
│
├── 📁 locales/                           
🌍 **PASTA IDIOMAS** 
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
├── 📁 data/                              
🗃️ **PASTA DATABASES**
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
└── 📁 assets/                            
📦 **PASTA RECURSOS** (criar depois)
    ├── 📁 audio/                         
    │   ├── 📄 opening-music.mp3
    vlog-beat-background-349853.zip
    │   ├── 📄 m416-shot.mp3
    │   ├── 📄 akm-shot.mp3
    │   ├── 📄 ump45-shot.mp3
    │   ├── 📄 scar-l-shot.mp3
    │   ├── 📄 m762-shot.mp3
    │   └── 📄 aug-shot.mp3
    │
    ├── 📁 css/                           
    │   ├── 📄 style.css
 * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Arial', sans-serif;
    background: linear-gradient(135deg, #1a1a2e, #16213e);
    color: #ffffff;
    line-height: 1.6;
}

/* Header */
header {
    background: rgba(0, 0, 0, 0.9);
    padding: 1rem 2rem;
}

nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.logo h1 {
    color: #f0a500;
    font-size: 1.5rem;
}

.nav-links {
    display: flex;
    gap: 2rem;
}

.nav-links a {
    color: white;
    text-decoration: none;
    padding: 0.5rem 1rem;
    border-radius: 5px;
    transition: all 0.3s ease;
}

.nav-links a:hover {
    background: #f0a500;
    color: black;
}

/* Main Content */
main {
    padding: 2rem;
    max-width: 1200px;
    margin: 0 auto;
}

.feature-section {
    background: rgba(255, 255, 255, 0.05);
    padding: 2rem;
    margin: 2rem 0;
    border-radius: 15px;
    border: 1px solid rgba(255, 255, 255, 0.1);
}

.feature-section h2 {
    color: #f0a500;
    margin-bottom: 1.5rem;
    font-size: 1.8rem;
    text-align: center;
}

/* Music Player */
.music-player {
    position: fixed;
    top: 20px;
    right: 20px;
    z-index: 1000;
}

.music-btn {
    background: rgba(255, 255, 255, 0.1);
    border: 2px solid #f0a500;
    color: white;
    padding: 10px 15px;
    border-radius: 25px;
    cursor: pointer;
}

/* Sensitivity Tester */
.sensitivity-tester {
    border: 2px solid #444;
    padding: 20px;
    border-radius: 10px;
    text-align: center;
}

#weaponSelect {
    background: #2a2a2a;
    color: white;
    padding: 10px;
    border: 1px solid #f0a500;
    border-radius: 5px;
    font-size: 1.1rem;
    margin-bottom: 1rem;
}

.target-area {
    width: 300px;
    height: 200px;
    background: #1a1a1a;
    position: relative;
    margin: 20px auto;
    border: 2px solid #333;
    border-radius: 10px;
}

.target {
    width: 50px;
    height: 50px;
    background: red;
    border-radius: 50%;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
}

/* Buttons */
button {
    background: linear-gradient(45deg, #f0a500, #ff6b00);
    color: white;
    border: none;
    padding: 12px 24px;
    border-radius: 25px;
    cursor: pointer;
    font-size: 1rem;
    margin: 5px;
}

/* Responsive */
@media (max-width: 768px) {
    .nav-links {
        flex-direction: column;
        gap: 0.5rem;
    }
    
    .target-area {
        width: 250px;
        height: 150px;
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
    │   ├──js/app.js
 // Sistema de Música
let musicPlaying = false;
const backgroundMusic = new Audio('audio/background-music.mp3');
backgroundMusic.loop = true;

function toggleMusic() {
    if (musicPlaying) {
        backgroundMusic.pause();
        musicPlaying = false;
        event.target.textContent = "🔇 Music";
    } else {
        backgroundMusic.play().catch(error => {
            alert("Click 'Music' again to play!");
        });
        musicPlaying = true;
        event.target.textContent = "🔊 Music";
    }
}

// Dados das Armas
const weaponData = {
    akm: {
        sensitivity: "38-45%",
        recoil: "High vertical recoil → pull down",
        pattern: "Pattern: Vertical with slight right curve",
        tips: "Tip: Use compensator and stock"
    },
    m416: {
        sensitivity: "45-55%", 
        recoil: "Moderate recoil → smooth control",
        pattern: "Pattern: Light 'S' shape",
        tips: "Tip: Very stable with full attachments"
    },
    scar-l: {
        sensitivity: "42-50%",
        recoil: "Low recoil → easy control", 
        pattern: "Pattern: Almost vertical",
        tips: "Tip: Excellent for beginners"
    }
};

// Atualizar informações da arma
function updateWeaponInfo() {
    const selectedWeapon = document.getElementById('weaponSelect').value;
    const stats = weaponData[selectedWeapon];
    
    document.getElementById('weaponStats').innerHTML = `
        <strong>Recommended Sensitivity:</strong> ${stats.sensitivity}<br>
        <strong>Recoil Control:</strong> ${stats.recoil}<br>
        <strong>${stats.pattern}</strong><br>
        <em>${stats.tips}</em>
    `;
}

// Otimizador de Gráficos
function optimizeGraphics() {
    const profiles = {
        lowEnd: {
            graphics: "Smooth", fps: "Medium", shadows: "Disabled",
            tips: "Focus on performance - best FPS"
        },
        midRange: {
            graphics: "Balanced", fps: "High", shadows: "Disabled", 
            tips: "Perfect balance between visuals and performance"
        },
        highEnd: {
            graphics: "HDR", fps: "Ultra", shadows: "Enabled",
            tips: "Best visual experience - for flagship devices"
        }
    };
    
    const userAgent = navigator.userAgent;
    let profile = profiles.midRange; // padrão
    
    if (/iPhone X|iPhone 1[1-5]|Galaxy S2[0-9]|Pixel/i.test(userAgent)) {
        profile = profiles.highEnd;
    } else if (/iPhone [6-9]|Galaxy A|Redmi Note|Moto G/i.test(userAgent)) {
        profile = profiles.lowEnd;
    }
    
    document.getElementById('graphicsSettings').innerHTML = `
        <h3>⚙️ Optimized Settings:</h3>
        <p>🎨 Graphics: <strong>${profile.graphics}</strong></p>
        <p>📊 FPS: <strong>${profile.fps}</strong></p>
        <p>🌑 Shadows: <strong>${profile.shadows}</strong></p>
        <p>💡 ${profile.tips}</p>
    `;
}

// Simulador de Caixas
function openCrate() {
    const items = {
        common: [
            { name: "Blue T-Shirt", probability: 0.35, rarity: "common" },
            { name: "Jeans Pants", probability: 0.30, rarity: "common" }
        ],
        rare: [
            { name: "AKM Gold Skin", probability: 0.15, rarity: "rare" },
            { name: "Military Outfit", probability: 0.12, rarity: "rare" }
        ],
        epic: [
            { name: "M416 Legendary Skin", probability: 0.04, rarity: "epic" }
        ]
    };
    
    const random = Math.random();
    let item;
    
    if (random < 0.60) item = items.common[Math.floor(Math.random() * items.common.length)];
    else if (random < 0.90) item = items.rare[Math.floor(Math.random() * items.rare.length)];
    else item = items.epic[Math.floor(Math.random() * items.epic.length)];
    
    const rarityColor = item.rarity === 'common' ? 'blue' : 
                       item.rarity === 'rare' ? 'purple' : 'gold';
    
    document.getElementById('crateResult').innerHTML = `
        <div style="padding: 1rem; margin: 1rem 0; border-radius: 10px; border: 2px solid ${rarityColor}">
            <h3 style="color: ${rarityColor}">🎁 ${item.name}</h3>
            <p><strong>Rarity:</strong> ${item.rarity.toUpperCase()}</p>
            <p><strong>Probability:</strong> ${(item.probability * 100).toFixed(1)}%</p>
        </div>
    `;
}

// Gerador de Nickname
function generateNickname() {
    const styles = {
        professional: ["Pro", "Elite", "Master", "Ace"],
        aggressive: ["Killer", "Slayer", "Hunter", "Predator"],
        tactical: ["Ghost", "Shadow", "Phantom", "Stealth"],
        funny: ["Chicken", "Noob", "Camper", "Potato"]
    };
    
    const style = document.getElementById('nicknameStyle').value;
    const baseName = document.getElementById('baseName').value || "Player";
    const templates = styles[style];
    const randomTemplate = templates[Math.floor(Math.random() * templates.length)];
    const symbols = ["×", "★", "☆", "㊣"];
    const randomSymbol = symbols[Math.floor(Math.random() * symbols.length)];
    
    const nickname = `${baseName}${randomSymbol}${randomTemplate}`;
    document.getElementById('nicknameResult').textContent = nickname;
}

function copyNickname() {
    const nickname = document.getElementById('nicknameResult').textContent;
    if (!nickname) {
        alert("Generate a nickname first!");
        return;
    }
    navigator.clipboard.writeText(nickname);
    alert("✅ Nickname copied!");
}

// Inicialização
document.addEventListener('DOMContentLoaded', function() {
    updateWeaponInfo();
    document.getElementById('weaponSelect').addEventListener('change', updateWeaponInfo);
    
    // Adicionar player de música se não existir
    if (!document.querySelector('.music-player')) {
        const musicPlayer = document.createElement('div');
        musicPlayer.className = 'music-player';
        musicPlayer.innerHTML = '<button class="music-btn" onclick="toggleMusic()">🔇 Music</button>';
        document.body.appendChild(musicPlayer);
    }
});
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
    ├── audio/
        └── background-music.mp3
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
        ├── images/
            └──favicon.pgn
        ├── 📄 apple-touch-icon.png
        ├── 📄 favicon-32x32.png
        ├── 📄 favicon-16x16.png
        └── 📄 icon-512x512.png
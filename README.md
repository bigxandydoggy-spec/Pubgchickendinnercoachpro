Pubgchickendinnercoachpro/          
locales/en.json
│
├── 📄 index.html                   
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>PUBG Chicken Dinner Coach Pro - Ultimate Gaming Assistant</title>
    <meta name="description" content="Professional PUBG Mobile coach - Strategies, calculators, and tips for chicken dinners">
    
    <!-- ✅ ÍCONES PROFISSIONAIS -->
    <link rel="apple-touch-icon" sizes="180x180" href="assets/icons/apple-touch-icon.png">
    <link rel="icon" type="image/png" sizes="32x32" href="assets/icons/favicon-32x32.png">
    <link rel="icon" type="image/png" sizes="16x16" href="assets/icons/favicon-16x16.png">
    <link rel="icon" type="image/x-icon" href="assets/icons/favicon.ico">
    <link rel="manifest" href="assets/icons/site.webmanifest">
    <meta name="msapplication-TileColor" content="#ff6b35">
    <meta name="theme-color" content="#ff6b35">
    
    <!-- Open Graph -->
    <meta property="og:title" content="PUBG Chicken Dinner Coach Pro">
    <meta property="og:description" content="Your professional PUBG Mobile coaching assistant">
    <meta property="og:image" content="assets/icons/icon-512x512.png">
    <meta property="og:type" content="website">
    <meta property="og:url" content="https://bigxandydoggy-spec.github.io/Pubgchickendinnercoachpro/">
    
    <style>
        :root {
            --color-primary: #ff6b35;
            --color-primary-dark: #e55a2b;
            --color-dark: #1a1a1a;
            --color-darker: #141414;
            --color-gray: #2d2d2d;
            --color-light: #ffffff;
            --font-main: 'Arial', 'Segoe UI', sans-serif;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: var(--font-main);
            background: linear-gradient(135deg, var(--color-darker) 0%, var(--color-dark) 100%);
            color: var(--color-light);
            line-height: 1.6;
            min-height: 100vh;
        }

        .app-header {
            background: rgba(26, 26, 26, 0.95);
            backdrop-filter: blur(10px);
            padding: 2rem 1rem;
            text-align: center;
            border-bottom: 3px solid var(--color-primary);
            position: relative;
        }

        .app-title {
            font-size: 2.5rem;
            font-weight: 800;
            margin-bottom: 0.5rem;
            background: linear-gradient(45deg, var(--color-primary), #ffd700);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        .app-subtitle {
            color: #cccccc;
            font-size: 1.1rem;
            font-weight: 300;
        }

        .language-selector {
            position: absolute;
            top: 1rem;
            right: 1rem;
            background: var(--color-gray);
            color: white;
            border: 1px solid #444;
            padding: 0.5rem 1rem;
            border-radius: 6px;
            cursor: pointer;
        }

        .nav-container {
            display: flex;
            justify-content: center;
            gap: 1rem;
            padding: 1.5rem;
            background: rgba(255, 107, 53, 0.1);
            backdrop-filter: blur(5px);
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
        }

        .nav-button:hover {
            background: var(--color-primary);
            transform: translateY(-2px);
            box-shadow: 0 5px 15px rgba(255, 107, 53, 0.3);
        }

        .nav-button.active {
            background: var(--color-primary);
            border-color: #ffd700;
            box-shadow: 0 5px 15px rgba(255, 107, 53, 0.4);
        }

        .section {
            display: none;
            padding: 3rem 2rem;
            max-width: 1000px;
            margin: 0 auto;
            animation: fadeIn 0.5s ease;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        .section.active {
            display: block;
        }

        .calculator-card {
            background: linear-gradient(135deg, var(--color-gray) 0%, #333 100%);
            padding: 2.5rem;
            border-radius: 15px;
            border-left: 5px solid var(--color-primary);
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
        }

        .form-group {
            margin-bottom: 2rem;
        }

        .form-input {
            width: 100%;
            padding: 1.2rem;
            background: #1a1a1a;
            color: white;
            border: 2px solid #444;
            border-radius: 8px;
            font-size: 1.1rem;
            transition: all 0.3s ease;
        }

        .form-input:focus {
            outline: none;
            border-color: var(--color-primary);
            box-shadow: 0 0 0 3px rgba(255, 107, 53, 0.2);
        }

        .btn-primary {
            background: linear-gradient(45deg, var(--color-primary), var(--color-primary-dark));
            color: white;
            border: none;
            padding: 1.2rem 2.5rem;
            border-radius: 8px;
            cursor: pointer;
            font-size: 1.1rem;
            font-weight: bold;
            width: 100%;
            transition: all 0.3s ease;
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        .btn-primary:hover {
            transform: translateY(-2px);
            box-shadow: 0 8px 25px rgba(255, 107, 53, 0.4);
        }

        #result {
            margin-top: 2rem;
            padding: 1.5rem;
            background: rgba(255, 107, 53, 0.1);
            border-radius: 10px;
            border: 1px solid rgba(255, 107, 53, 0.3);
        }

        /* Responsive */
        @media (max-width: 768px) {
            .app-title { font-size: 2rem; }
            .nav-container { flex-direction: column; gap: 0.5rem; }
            .nav-button { padding: 0.8rem 1rem; }
            .section { padding: 2rem 1rem; }
        }
    </style>
</head>
<body>
    <header class="app-header">
        <h1 class="app-title" data-i18n="appTitle">PUBG Coach Pro</h1>
        <p class="app-subtitle" data-i18n="welcomeSubtitle">Your personal assistant for chicken dinners</p>
        <select id="languageSelector" class="language-selector">
            <option value="en">English</option>
            <option value="pt">Português</option>
            <option value="es">Español</option>
            <option value="fr">Français</option>
        </select>
    </header>

    <nav class="nav-container">
        <button class="nav-button active" onclick="showSection('home')" data-i18n="home">Home</button>
        <button class="nav-button" onclick="showSection('calculator')" data-i18n="calculateRewards">Calculate Rewards</button>
        <button class="nav-button" onclick="showSection('strategies')" data-i18n="strategies">Strategies</button>
        <button class="nav-button" onclick="showSection('weapons')" data-i18n="weapons">Weapons Guide</button>
    </nav>

    <main>
        <section id="home" class="section active">
            <h2 data-i18n="welcomeHome">Welcome, Commander!</h2>
            <p data-i18n="welcomeText">This is your ultimate tool for mastering PUBG Mobile. Use the calculator to plan your strategy and check the guides to improve your gameplay.</p>
            
            <div style="margin-top: 2rem; display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 1rem;">
                <div style="background: rgba(255,107,53,0.1); padding: 1.5rem; border-radius: 10px; border-left: 4px solid #ff6b35;">
                    <h3 data-i18n="feature1">Smart Calculator</h3>
                    <p data-i18n="feature1Desc">Calculate rewards and plan your strategy</p>
                </div>
                <div style="background: rgba(255,107,53,0.1); padding: 1.5rem; border-radius: 10px; border-left: 4px solid #ffd700;">
                    <h3 data-i18n="feature2">Pro Strategies</h3>
                    <p data-i18n="feature2Desc">Learn from top players worldwide</p>
                </div>
                <div style="background: rgba(255,107,53,0.1); padding: 1.5rem; border-radius: 10px; border-left: 4px solid #ff6b35;">
                    <h3 data-i18n="feature3">Weapons Guide</h3>
                    <p data-i18n="feature3Desc">Master every weapon in the game</p>
                </div>
            </div>
        </section>

        <section id="calculator" class="section">
            <div class="calculator-card">
                <h2 data-i18n="calculateRewards">Calculate Rewards</h2>
                <div class="form-group">
                    <input type="number" id="kills" class="form-input" data-i18n-placeholder="killsPlaceholder" placeholder="Number of kills" min="0" max="50">
                </div>
                <div class="form-group">
                    <input type="number" id="placement" class="form-input" data-i18n-placeholder="placementPlaceholder" placeholder="Final placement (1-100)" min="1" max="100">
                </div>
                <button class="btn-primary" onclick="calculateRewards()" data-i18n="calculateButton">Calculate</button>
                <div id="result"></div>
            </div>
        </section>

        <section id="strategies" class="section">
            <h2 data-i18n="strategies">Advanced Strategies</h2>
            <div style="display: grid; gap: 1.5rem; margin-top: 2rem;">
                <div style="background: var(--color-gray); padding: 2rem; border-radius: 10px;">
                    <h3 data-i18n="strategy1">Early Game Survival</h3>
                    <p data-i18n="strategy1Desc">Choose optimal drop locations and secure early loot...</p>
                </div>
                <div style="background: var(--color-gray); padding: 2rem; border-radius: 10px;">
                    <h3 data-i18n="strategy2">Mid Game Rotation</h3>
                    <p data-i18n="strategy2Desc">Master zone rotations and positioning...</p>
                </div>
                <div style="background: var(--color-gray); padding: 2rem; border-radius: 10px;">
                    <h3 data-i18n="strategy3">End Game Dominance</h3>
                    <p data-i18n="strategy3Desc">Close games effectively and secure chicken dinner...</p>
                </div>
            </div>
        </section>

        <section id="weapons" class="section">
            <h2 data-i18n="weapons">Weapons Guide</h2>
            <p data-i18n="weaponsDesc">Coming soon - comprehensive weapon statistics and recommendations...</p>
        </section>
    </main>

    <script>
        // === SISTEMA DE INTERNACIONALIZAÇÃO ===
        const translations = {};

        async function loadLanguage(lang) {
            if (!translations[lang]) {
                try {
                    const response = await fetch(`locales/${lang}.json`);
                    translations[lang] = await response.json();
                } catch (error) {
                    console.error(`Failed to load language: ${lang}`, error);
                    return;
                }
            }
            
            document.querySelectorAll('[data-i18n]').forEach(element => {
                const key = element.getAttribute('data-i18n');
                if (translations[lang][key]) {
                    element.textContent = translations[lang][key];
                }
            });
            
            document.querySelectorAll('[data-i18n-placeholder]').forEach(element => {
                const key = element.getAttribute('data-i18n-placeholder');
                if (translations[lang][key]) {
                    element.placeholder = translations[lang][key];
                }
            });
        }

        document.getElementById('languageSelector').addEventListener('change', (e) => {
            loadLanguage(e.target.value);
        });

        loadLanguage('en');

        // === LÓGICA DA INTERFACE ===
        function showSection(sectionId) {
            document.querySelectorAll('.section').forEach(section => {
                section.classList.remove('active');
            });
            document.querySelectorAll('.nav-button').forEach(button => {
                button.classList.remove('active');
            });
            document.getElementById(sectionId).classList.add('active');
            event.currentTarget.classList.add('active');
        }

        function calculateRewards() {
            const kills = parseInt(document.getElementById('kills').value) || 0;
            const placement = parseInt(document.getElementById('placement').value) || 100;
            const currentLang = document.getElementById('languageSelector').value;
            
            let baseReward = 0;
            if (placement === 1) baseReward = 1000;
            else if (placement <= 3) baseReward = 800;
            else if (placement <= 10) baseReward = 500;
            else if (placement <= 25) baseReward = 200;
            else baseReward = 50;
            
            const killBonus = kills * 20;
            const total = baseReward + killBonus;
            
            document.getElementById('result').innerHTML = `
                <h3>${translations[currentLang]?.['resultTitle'] || 'Calculated Reward:'}</h3>
                <p>${(translations[currentLang]?.['baseReward'] || 'Placement: {{placement}}th - {{reward}} BP')
                    .replace('{{placement}}', placement)
                    .replace('{{reward}}', baseReward)}</p>
                <p>${translations[currentLang]?.['killReward'] || 'Kills Bonus:'} ${killBonus} BP</p>
                <p style="color: #ffd700; font-size: 1.2rem; font-weight: bold; margin-top: 1rem;">
                    ${(translations[currentLang]?.['totalReward'] || 'Total: {{total}} BP')
                    .replace('{{total}}', total)}
                </p>
            `;
        }
    </script>
</body>
</html>
│
├── 📁 locales/                     (Pasta de idiomas)
│   ├── 📄 en.json                  
({
  "appTitle": "PUBG Coach Pro",
  "welcomeSubtitle": "Your personal assistant for chicken dinners",
  "home": "Home",
  "calculateRewards": "Calculate Rewards",
  "strategies": "Strategies",
  "weapons": "Weapons Guide",
  "welcomeHome": "Welcome, Commander!",
  "welcomeText": "This is your ultimate tool for mastering PUBG Mobile. Use the calculator to plan your strategy and check the guides to improve your gameplay.",
  "feature1": "Smart Calculator",
  "feature1Desc": "Calculate rewards and plan your strategy",
  "feature2": "Pro Strategies",
  "feature2Desc": "Learn from top players worldwide",
  "feature3": "Weapons Guide",
  "feature3Desc": "Master every weapon in the game",
  "killsPlaceholder": "Number of kills",
  "placementPlaceholder": "Final placement (1-100)",
  "calculateButton": "Calculate",
  "resultTitle": "Calculated Reward:",
  "baseReward": "Placement: {{placement}}th - {{reward}} BP",
  "killReward": "Kills Bonus:",
  "totalReward": "Total: {{total}} BP",
  "strategy1": "Early Game Survival",
  "strategy1Desc": "Choose optimal drop locations and secure early loot...",
  "strategy2": "Mid Game Rotation",
  "strategy2Desc": "Master zone rotations and positioning...",
  "strategy3": "End Game Dominance",
  "strategy3Desc": "Close games effectively and secure chicken dinner...",
  "weaponsDesc": "Coming soon - comprehensive weapon statistics and recommendations..."
}
│   ├── 📄 pt.json                  
 {
  "appTitle": "PUBG Coach Pro",
  "welcomeSubtitle": "Seu assistente pessoal para vitórias no PUBG",
  "home": "Início",
  "calculateRewards": "Calculadora de Recompensas",
  "strategies": "Estratégias",
  "weapons": "Guia de Armas",
  "welcomeHome": "Bem-vindo, Comandante!",
  "welcomeText": "Esta é sua ferramenta definitiva para dominar o PUBG Mobile. Use a calculadora para planejar sua estratégia e verifique os guias para melhorar seu gameplay.",
  "feature1": "Calculadora Inteligente",
  "feature1Desc": "Calcule recompensas e planeje sua estratégia",
  "feature2": "Estratégias Pro",
  "feature2Desc": "Aprenda com os melhores jogadores do mundo",
  "feature3": "Guia de Armas",
  "feature3Desc": "Domine todas as armas do jogo",
  "killsPlaceholder": "Número de kills",
  "placementPlaceholder": "Posição final (1-100)",
  "calculateButton": "Calcular",
  "resultTitle": "Recompensa Calculada:",
  "baseReward": "Posição: {{placement}}º - {{reward}} BP",
  "killReward": "Bônus por Kills:",
  "totalReward": "Total: {{total}} BP",
  "strategy1": "Sobrevivência no Início",
  "strategy1Desc": "Escolha locais de drop ideais e garanta loot inicial...",
  "strategy2": "Rotação no Meio do Jogo",
  "strategy2Desc": "Domine rotações de zona e posicionamento...",
  "strategy3": "Domínio no Final",
  "strategy3Desc": "Feche partidas efetivamente e garanta a vitória...",
  "weaponsDesc": "Em breve - estatísticas completas de armas e recomendações..."
}
│   ├── 📄 ja.json                 
 {
  "appTitle": "PUBGコーチプロ",
  "welcomeSubtitle": "チキンディナーへの個人アシスタント",
  "home": "ホーム",
  "calculateRewards": "報酬計算",
  "strategies": "戦略",
  "weapons": "武器ガイド",
  "welcomeHome": "指揮官、ようこそ！",
  "welcomeText": "これはPUBGモバイルをマスターするための究極のツールです。計算機で戦略を計画し、ガイドでゲームプレイを向上させましょう。",
  "feature1": "スマート計算機",
  "feature1Desc": "報酬を計算し戦略を計画",
  "feature2": "プロ戦略",
  "feature2Desc": "世界中のトッププレイヤーから学ぶ",
  "feature3": "武器ガイド",
  "feature3Desc": "ゲーム内の全武器をマスター",
  "killsPlaceholder": "キル数",
  "placementPlaceholder": "最終順位 (1-100)",
  "calculateButton": "計算",
  "resultTitle": "計算された報酬:",
  "baseReward": "順位: {{placement}}位 - {{reward}} BP",
  "killReward": "キルボーナス:",
  "totalReward": "合計: {{total}} BP",
  "strategy1": "序盤の生存",
  "strategy1Desc": "最適なドロップ地点と初期装備の確保...",
  "strategy2": "中盤のローテーション",
  "strategy2Desc": "ゾーン移動とポジショニング...",
  "strategy3": "終盤の支配",
  "strategy3Desc": "効果的にゲームを締め、勝利を収める...",
  "weaponsDesc": "近日公開 - 包括的な武器統計と推奨..."
}
│   └── 📄 ko.json                
  {
  "appTitle": "PUBG 코치 프로",
  "welcomeSubtitle": "치킨 디너를 위한 개인 어시스턴트",
  "home": "홈",
  "calculateRewards": "보상 계산",
  "strategies": "전략",
  "weapons": "무기 가이드",
  "welcomeHome": "지휘관님, 환영합니다!",
  "welcomeText": "PUBG 모바일을 마스터하기 위한 궁극의 도구입니다. 계산기로 전략을 계획하고 가이드로 게임 플레이를 향상시키세요.",
  "feature1": "스마트 계산기",
  "feature1Desc": "보상 계산 및 전략 계획",
  "feature2": "프로 전략",
  "feature2Desc": "전 세계 탑 플레이어로부터 배우기",
  "feature3": "무기 가이드",
  "feature3Desc": "게임 내 모든 무기 마스터",
  "killsPlaceholder": "킬 수",
  "placementPlaceholder": "최종 순위 (1-100)",
  "calculateButton": "계산",
  "resultTitle": "계산된 보상:",
  "baseReward": "순위: {{placement}}위 - {{reward}} BP",
  "killReward": "킬 보너스:",
  "totalReward": "총계: {{total}} BP",
  "strategy1": "초반 생존",
  "strategy1Desc": "최적의 드롭 위치 및 초기 전리품 확보...",
  "strategy2": "중반 이동",
  "strategy2Desc": "존 이동 및 위치 선정...",
  "strategy3": "종반 지배",
  "strategy3Desc": "효과적으로 게임을 마무리하고 승리하기...",
  "weaponsDesc": "곧 제공 - 포괄적인 무기 통계 및 추천..."
}
└── 📄 zh.json
{
  "appTitle": "PUBG 教练专业版",
  "welcomeSubtitle": "您的专属吃鸡助手",
  "home": "首页",
  "calculateRewards": "奖励计算",
  "strategies": "策略",
  "weapons": "武器指南",
  "welcomeHome": "欢迎您，指挥官！",
  "welcomeText": "这是您掌握PUBG移动版的终极工具。使用计算器规划策略，查阅指南提升游戏技巧。",
  "feature1": "智能计算器",
  "feature1Desc": "计算奖励并规划策略",
  "feature2": "专业策略",
  "feature2Desc": "向全球顶尖玩家学习",
  "feature3": "武器指南",
  "feature3Desc": "精通游戏中的每种武器",
  "killsPlaceholder": "击杀数",
  "placementPlaceholder": "最终名次 (1-100)",
  "calculateButton": "计算",
  "resultTitle": "计算奖励:",
  "baseReward": "名次: {{placement}} - {{reward}} BP",
  "killReward": "击杀奖励:",
  "totalReward": "总计: {{total}} BP",
  "strategy1": "早期生存",
  "strategy1Desc": "选择最佳落点并确保早期物资...",
  "strategy2": "中期转移",
  "strategy2Desc": "掌握圈形转移和站位...",
  "strategy3": "决赛圈主宰",
  "strategy3Desc": "有效结束对局，确保胜利...",
  "weaponsDesc": "即将推出 - 全面的武器数据和推荐..."
}
│
└── 📁 assets/                     
 {
  "name": "PUBG Chicken Dinner Coach Pro",
  "short_name": "PUBG Coach",
  "description": "Professional PUBG Mobile coaching assistant",
  "start_url": "/",
  "display": "standalone",
  "background_color": "#1a1a1a",
  "theme_color": "#ff6b35",
  "orientation": "portrait",
  "icons": [
    {
      "src": "favicon-32x32.png",
      "sizes": "32x32",
      "type": "image/png"
    },
    {
      "src": "favicon-16x16.png",
      "sizes": "16x16",
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
  ]
}
    ├── 📁 icons/                  
    <link rel="apple-touch-icon" sizes="180x180" href="/apple-touch-icon.png">
<link rel="icon" type="image/png" sizes="32x32" href="/favicon-32x32.png">
<link rel="icon" type="image/png" sizes="16x16" href="/favicon-16x16.png">
<link rel="manifest" href="/site.webmanifest">
    │   ├── 📄 apple-touch-icon.png     (180x180 - ícone Apple)
    │   ├── 📄 favicon-32x32.png        (32x32 - para navegadores)
    │   ├── 📄 favicon-16x16.png        (16x16 - favicon pequeno)
    │   ├── 📄 favicon.ico              (Ícone .ico tradicional)
    │   ├── 📄 icon-512x512.png         (512x512 - grande)
    │   └── 📄 site.webmanifest         (Arquivo de configuração)
    │
    ├── 📁 css/
    │   └── 📄 style.css            
/* ===== ESTILOS GERAIS ===== */
:root {
    --color-primary: #ff6b35;
    --color-primary-dark: #e55a2b;
    --color-dark: #1a1a1a;
    --color-darker: #141414;
    --color-gray: #2d2d2d;
    --color-light: #ffffff;
    --font-main: 'Arial', 'Segoe UI', sans-serif;
}

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: var(--font-main);
    background: linear-gradient(135deg, var(--color-darker) 0%, var(--color-dark) 100%);
    color: var(--color-light);
    line-height: 1.6;
    min-height: 100vh;
}

/* ===== CABEÇALHO ===== */
.app-header {
    background: rgba(26, 26, 26, 0.95);
    backdrop-filter: blur(10px);
    padding: 2rem 1rem;
    text-align: center;
    border-bottom: 3px solid var(--color-primary);
    position: relative;
}

.app-title {
    font-size: 2.5rem;
    font-weight: 800;
    margin-bottom: 0.5rem;
    background: linear-gradient(45deg, var(--color-primary), #ffd700);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
}

.app-subtitle {
    color: #cccccc;
    font-size: 1.1rem;
    font-weight: 300;
}

.language-selector {
    position: absolute;
    top: 1rem;
    right: 1rem;
    background: var(--color-gray);
    color: white;
    border: 1px solid #444;
    padding: 0.5rem 1rem;
    border-radius: 6px;
    cursor: pointer;
}

/* ===== NAVEGAÇÃO ===== */
.nav-container {
    display: flex;
    justify-content: center;
    gap: 1rem;
    padding: 1.5rem;
    background: rgba(255, 107, 53, 0.1);
    backdrop-filter: blur(5px);
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
}

.nav-button:hover {
    background: var(--color-primary);
    transform: translateY(-2px);
    box-shadow: 0 5px 15px rgba(255, 107, 53, 0.3);
}

.nav-button.active {
    background: var(--color-primary);
    border-color: #ffd700;
    box-shadow: 0 5px 15px rgba(255, 107, 53, 0.4);
}

/* ===== SEÇÕES ===== */
.section {
    display: none;
    padding: 3rem 2rem;
    max-width: 1000px;
    margin: 0 auto;
    animation: fadeIn 0.5s ease;
}

@keyframes fadeIn {
    from { opacity: 0; transform: translateY(20px); }
    to { opacity: 1; transform: translateY(0); }
}

.section.active {
    display: block;
}

/* ===== CALCULADORA ===== */
.calculator-card {
    background: linear-gradient(135deg, var(--color-gray) 0%, #333 100%);
    padding: 2.5rem;
    border-radius: 15px;
    border-left: 5px solid var(--color-primary);
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
}

.form-group {
    margin-bottom: 2rem;
}

.form-input {
    width: 100%;
    padding: 1.2rem;
    background: #1a1a1a;
    color: white;
    border: 2px solid #444;
    border-radius: 8px;
    font-size: 1.1rem;
    transition: all 0.3s ease;
}

.form-input:focus {
    outline: none;
    border-color: var(--color-primary);
    box-shadow: 0 0 0 3px rgba(255, 107, 53, 0.2);
}

.btn-primary {
    background: linear-gradient(45deg, var(--color-primary), var(--color-primary-dark));
    color: white;
    border: none;
    padding: 1.2rem 2.5rem;
    border-radius: 8px;
    cursor: pointer;
    font-size: 1.1rem;
    font-weight: bold;
    width: 100%;
    transition: all 0.3s ease;
    text-transform: uppercase;
    letter-spacing: 1px;
}

.btn-primary:hover {
    transform: translateY(-2px);
    box-shadow: 0 8px 25px rgba(255, 107, 53, 0.4);
}

#result {
    margin-top: 2rem;
    padding: 1.5rem;
    background: rgba(255, 107, 53, 0.1);
    border-radius: 10px;
    border: 1px solid rgba(255, 107, 53, 0.3);
}

/* ===== CARDS DE RECURSOS ===== */
.feature-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 1rem;
    margin-top: 2rem;
}

.feature-card {
    background: rgba(255, 107, 53, 0.1);
    padding: 1.5rem;
    border-radius: 10px;
    border-left: 4px solid #ff6b35;
    transition: transform 0.3s ease;
}

.feature-card:hover {
    transform: translateY(-5px);
}

.feature-card:nth-child(2) {
    border-left-color: #ffd700;
}

/* ===== RESPONSIVIDADE ===== */
@media (max-width: 768px) {
    .app-title { font-size: 2rem; }
    .nav-container { flex-direction: column; gap: 0.5rem; }
    .nav-button { padding: 0.8rem 1rem; }
    .section { padding: 2rem 1rem; }
    .feature-grid { grid-template-columns: 1fr; }
}
    │
    └── 📁 js/
        └── 📄 script.js          
          // === SISTEMA DE INTERNACIONALIZAÇÃO ===
const translations = {};

/**
 * Carrega um idioma e aplica as traduções
 * @param {string} lang - Código do idioma (en, pt, ja, ko, zh)
 */
async function loadLanguage(lang) {
    if (!translations[lang]) {
        try {
            const response = await fetch(`locales/${lang}.json`);
            translations[lang] = await response.json();
        } catch (error) {
            console.error(`Falha ao carregar idioma: ${lang}`, error);
            return;
        }
    }
    
    // Aplica traduções a elementos com data-i18n
    document.querySelectorAll('[data-i18n]').forEach(element => {
        const key = element.getAttribute('data-i18n');
        if (translations[lang][key]) {
            element.textContent = translations[lang][key];
        }
    });
    
    // Aplica placeholders traduzidos
    document.querySelectorAll('[data-i18n-placeholder]').forEach(element => {
        const key = element.getAttribute('data-i18n-placeholder');
        if (translations[lang][key]) {
            element.placeholder = translations[lang][key];
        }
    });
}

// Configura o seletor de idioma
document.getElementById('languageSelector').addEventListener('change', (e) => {
    loadLanguage(e.target.value);
    // Opcional: Salvar preferência no localStorage
    localStorage.setItem('preferredLanguage', e.target.value);
});

// === CONTROLE DE SEÇÕES ===
/**
 * Mostra uma seção específica e atualiza a navegação
 * @param {string} sectionId - ID da seção a ser mostrada
 */
function showSection(sectionId) {
    // Esconde todas as seções
    document.querySelectorAll('.section').forEach(section => {
        section.classList.remove('active');
    });
    
    // Remove classe active de todos os botões
    document.querySelectorAll('.nav-button').forEach(button => {
        button.classList.remove('active');
    });
    
    // Mostra a seção selecionada
    document.getElementById(sectionId).classList.add('active');
    
    // Atualiza o botão ativo (se o evento veio de um clique)
    if (event && event.currentTarget) {
        event.currentTarget.classList.add('active');
    }
}

// === CALCULADORA DE RECOMPENSAS ===
/**
 * Calcula recompensas baseadas em kills e posição
 */
function calculateRewards() {
    const kills = parseInt(document.getElementById('kills').value) || 0;
    const placement = parseInt(document.getElementById('placement').value) || 100;
    const currentLang = document.getElementById('languageSelector').value;
    
    // Validação de entrada
    if (kills < 0) {
        alert('Por favor, insira um número válido de kills');
        return;
    }
    
    if (placement < 1 || placement > 100) {
        alert('Por favor, insira uma posição entre 1 e 100');
        return;
    }
    
    // Cálculo da recompensa base
    let baseReward = 0;
    if (placement === 1) baseReward = 1000;
    else if (placement <= 3) baseReward = 800;
    else if (placement <= 10) baseReward = 500;
    else if (placement <= 25) baseReward = 200;
    else baseReward = 50;
    
    // Cálculo do bônus
    const killBonus = kills * 20;
    const total = baseReward + killBonus;
    
    // Exibe o resultado
    const resultElement = document.getElementById('result');
    resultElement.innerHTML = `
        <h3>${translations[currentLang]?.['resultTitle'] || 'Calculated Reward:'}</h3>
        <p>${(translations[currentLang]?.['baseReward'] || 'Placement: {{placement}}th - {{reward}} BP')
            .replace('{{placement}}', placement)
            .replace('{{reward}}', baseReward)}</p>
        <p>${translations[currentLang]?.['killReward'] || 'Kills Bonus:'} ${killBonus} BP</p>
        <p style="color: #ffd700; font-size: 1.2rem; font-weight: bold; margin-top: 1rem;">
            ${(translations[currentLang]?.['totalReward'] || 'Total: {{total}} BP')
            .replace('{{total}}', total)}
        </p>
    `;
}

// === INICIALIZAÇÃO ===
/**
 * Inicializa o aplicativo quando o DOM estiver carregado
 */
document.addEventListener('DOMContentLoaded', function() {
    console.log('PUBG Coach Pro inicializado!');
    
    // Carrega idioma salvo ou padrão (inglês)
    const savedLanguage = localStorage.getItem('preferredLanguage') || 'en';
    document.getElementById('languageSelector').value = savedLanguage;
    loadLanguage(savedLanguage);
    
    // Mostra a seção inicial
    showSection('home');
    
    // Configura botões de navegação
    document.querySelectorAll('.nav-button').forEach(button => {
        button.addEventListener('click', function() {
            const targetSection = this.getAttribute('onclick').match(/'([^']+)'/)[1];
            showSection(targetSection);
        });
    });
});

// === FUNÇÕES ADICIONAIS PARA FUTURAS EXPANSÕES ===
/**
 * Salva dados do usuário (para futuras implementações)
 */
function saveUserData() {
    // Implementar para versões futuras
}

/**
 * Carrega dados do usuário (para futuras implementações)
 */
function loadUserData() {
    // Implementar para versões futuras
}
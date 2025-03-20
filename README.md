<html lang="ru">
<head>
    <meta charset="UTF-8">
    <title>Статистика клана Бездна</title>
    <style>
        body {
            background: linear-gradient(-45deg, #0a0a0a, #1a1a1a, #2a2a2a, #1a1a1a);
            background-size: 400% 400%;
            animation: gradientBG 15s ease infinite;
            color: #e0e0e0;
            font-family: 'Arial', sans-serif;
            padding: 20px;
            min-height: 100vh;
            margin: 0;
        }

        @keyframes gradientBG {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }

        .clan-header {
            overflow: hidden;
            position: relative;
            height: 60px;
            margin-bottom: 25px;
            border-left: 4px solid #ff6600;
        }

        .clan-header h1 {
            position: absolute;
            white-space: nowrap;
            animation: titleMove 15s linear infinite;
            font-size: 2.5em;
            margin: 0;
            background: linear-gradient(45deg, #ff6600, #ffaa00, #ff6600);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            text-shadow: 0 0 15px rgba(255,102,0,0.5);
            padding-left: 15px;
        }

        @keyframes titleMove {
            0% { transform: translateX(-100%); }
            100% { transform: translateX(100vw); }
        }

        .stats-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 15px;
            margin-bottom: 25px;
        }

        .stat-item {
            background: rgba(45,45,45,0.8);
            padding: 15px;
            border-radius: 8px;
            backdrop-filter: blur(5px);
            border: 1px solid #ff660055;
        }

        .buttons-container {
            display: flex;
            gap: 15px;
            margin-bottom: 20px;
        }

        .members-btn {
            background: linear-gradient(45deg, #ff6600, #ff8822);
            color: white;
            border: none;
            padding: 12px 25px;
            border-radius: 5px;
            cursor: pointer;
            font-size: 16px;
            transition: transform 0.3s;
        }

        .storage-btn {
            background: linear-gradient(45deg, #00ff66, #22ff88);
        }

        .chicken-btn {
            background: linear-gradient(45deg, #ffd700, #ffaa00);
        }

        .members-btn:hover {
            transform: scale(1.05);
        }

        .members-list, .storage-list, .chicken-section {
            display: none;
            background: rgba(38,38,38,0.9);
            padding: 20px;
            border-radius: 10px;
            backdrop-filter: blur(5px);
            margin-bottom: 20px;
        }

        .members-list {
            border: 1px solid #ff660055;
        }

        .storage-list {
            border: 1px solid #00ff6655;
        }

        .chicken-section {
            border: 1px solid #ffd70055;
            text-align: center;
            font-size: 1.5em;
        }

        .member-row {
            display: grid;
            grid-template-columns: 30px 1fr 50px 80px 80px;
            align-items: center;
            padding: 10px;
            border-bottom: 1px solid #383838;
        }

        .storage-item {
            display: grid;
            grid-template-columns: 30px 1fr 60px;
            align-items: center;
            padding: 8px;
            border-bottom: 1px solid #383838;
        }

        .rank-icon {
            font-size: 1.2em;
            color: #ff6600;
        }

        .storage-header {
            color: #00ff66;
            font-size: 1.2em;
            margin-bottom: 15px;
        }
    </style>
</head>
<body>
    <div class="clan-header">
        <h1>📯 Клан: �҉̧Б҉̧Е҉̧З҉̧Д҉̧Н҉̧А҉̧🧿</h1>
    </div>

    <div class="stats-grid">
        <div class="stat-item">
            🔸 Уровень: 7<br>
            🔹 Очки клана: 97125<br>
            ♨️ Сила клана: 2319
        </div>
        <div class="stat-item">
            💰 Казна: 12133<br>
            📦 Хранилище: (281/730)<br>
            👥 Состав: (35/35)
        </div>
    </div>

    <div class="buttons-container">
        <button class="members-btn" onclick="toggleSection('membersList')">👥 Показать состав</button>
        <button class="members-btn storage-btn" onclick="toggleSection('storageList')">📦 Хранилище</button>
        <button class="members-btn chicken-btn" onclick="toggleSection('chickenSection')">🐔 Шах 🔸0 🏵-999 🔹????</button>
    </div>

    <div class="members-list" id="membersList">
        <div class="member-header">
            <h2>👑 Лидер: 🧿 🧝♂️ AyanVRotVamDam 🔸30</h2>
            <h3>💂 Старейшины:
                🧿 👸 Mike413 🔸35,
                🧿 🧝♀️ Akila 🔸26,
                🧿 🤴️ ХреноДилдоХант 🔸32,
                🧿 🤴️ Circa 🔸34
            </h3>
        </div>
    </div>

    <div class="storage-list" id="storageList">
        <div class="storage-header">📦 Хранилище клана (281/730)</div>
        <div class="storage-item"><div>💚</div><div>Бонус регенерации 24ч</div><div>7шт.</div></div>
        <div class="storage-item"><div>🥪</div><div>Бутерброд [III] - 24ч</div><div>1шт.</div></div>
        <div class="storage-item"><div>💧</div><div>Слёзы Обезумевших [I]</div><div>25шт.</div></div>
        <div class="storage-item"><div>🍲</div><div>Чесночная похлебка [I]</div><div>2шт.</div></div>
        <div class="storage-item"><div>🔧</div><div>Ремкомплект</div><div>6шт.</div></div>
        <div class="storage-item"><div>🥮</div><div>Пастуший хлеб [I]</div><div>3шт.</div></div>
        <div class="storage-item"><div>🍲</div><div>Блюдо из рыбы [I]</div><div>8шт.</div></div>
        <div class="storage-item"><div>🧪</div><div>Богатство торговца</div><div>3шт.</div></div>
        <div class="storage-item"><div>📔</div><div>Пробивающая стрела I(🗡1⚡️1)</div><div>1шт.</div></div>
        <div class="storage-item"><div>🍛</div><div>Луковый суп [I]</div><div>7шт.</div></div>
        <div class="storage-item"><div>🥘</div><div>Блюдо из мяса [III]</div><div>8шт.</div></div>
        <div class="storage-item"><div>🥘</div><div>Острый лечо [I]</div><div>2шт.</div></div>
        <div class="storage-item"><div>📜</div><div>Пыльный фрагмент шлема</div><div>1шт.</div></div>
        <div class="storage-item"><div>📜</div><div>Пыльный фрагмент сапог</div><div>1шт.</div></div>
        <div class="storage-item"><div>🈴</div><div>Вольфрам</div><div>25шт.</div></div>
        <div class="storage-item"><div>📜</div><div>Пыльный фрагмент перчатки</div><div>3шт.</div></div>
        <div class="storage-item"><div>🈴</div><div>Биоток</div><div>22шт.</div></div>
        <div class="storage-item"><div>🍛</div><div>Аквельский обед [III]</div><div>2шт.</div></div>
        <div class="storage-item"><div>✴️</div><div>Медь</div><div>140шт.</div></div>
        <div class="storage-item"><div>🍲</div><div>Блюдо из рыбы [III]</div><div>5шт.</div></div>
        <div class="storage-item"><div>🍛</div><div>Аквельский обед [I]</div><div>9шт.</div></div>
        <div class="storage-item" style="color: #ffd700; margin-top: 15px;">
            <div>💰</div><div>Золота в казне:</div><div>12133</div>
        </div>
    </div>

    <div class="chicken-section" id="chickenSection">
        Петушок 🐔 обычный
        <div style="font-size: 0.6em; margin-top: 10px; color: #ffd700;">
            [от Str1t любимому Шаху ❤️]
        </div>
    </div>

    <script>
        const members = [
            {name: '🧿 🧟♂️ Ардагер', level: 33, points: 166, power: 12222},
            {name: '🧿 🤴 Fdooch', level: 31, points: 1481, power: 12189},
            {name: '🧿 🧝♂️ Малик666', level: 32, points: 20, power: 10719},
            {name: '🧿 🤴 Morderface', level: 34, points: 834, power: 10377},
            {name: '🧿 🤴 Barny', level: 31, points: 26524, power: 9426},
            {name: '🧿 👸 Mike413', level: 35, points: 790, power: 9081},
            {name: '🧿 🤴 Преступление', level: 32, points: 1625, power: 8835},
            {name: '🧿 🤴 FoboS', level: 31, points: 18359, power: 7526},
            {name: '🧿 🧝♂️ Kazutora', level: 32, points: 13094, power: 7524},
            {name: '🧿 🤴 Ange1Frei', level: 29, points: 2967, power: 6072},
            {name: '🧿 👸 тыковка', level: 30, points: 1165, power: 5801},
            {name: '🧿 🤴 Circa', level: 34, points: 88, power: 4600},
            {name: '🧿 🤴 Лжешах', level: 29, points: 2625, power: 4554},
            {name: '🧿 🧝♀️ Str1t', level: 33, points: 72, power: 3563},
            {name: '🧿 👸 Deffl', level: 33, points: 97, power: 3281},
            {name: '🧿 🧝♂️ ШевелисьПлотва', level: 27, points: 405, power: 2811},
            {name: '🧿 🤴 ArtsiomA', level: 25, points: 3131, power: 1243},
            {name: '🧿 🧝♂️ Imperiya', level: 26, points: 3652, power: 1200},
            {name: '🧿 🤴 корнеплод', level: 31, points: 371, power: 934},
            {name: '🧿 🧝♂️ AyanVRotVamDam', level: 30, points: 1810, power: 682},
            {name: '🧿 👸 Skolopendra', level: 26, points: 1998, power: 647},
            {name: '🧿 🤴 ЭндшпилЬ', level: 24, points: 4841, power: 642},
            {name: '🧿 🤴 ХреноДилдоХант', level: 32, points: 466, power: 379},
            {name: '🧿 🤴 ZloyViking', level: 25, points: 1966, power: 342},
            {name: '🧿 🤴 Instin4ik', level: 35, points: 65, power: 217},
            {name: '🧿 🧟♂️ zhenkazz', level: 24, points: 2751, power: 137},
            {name: '🧿 🤴 Кетцаль', level: 24, points: 4477, power: 127},
            {name: '🧿 🧟♂️ RhododendroN', level: 27, points: 273, power: 119},
            {name: '🧿 🧟♂️ sanji', level: 29, points: 8209, power: 118},
            {name: '🧿 🧝♂️ MaZaFaKa', level: 24, points: 6831, power: 39},
            {name: '🧿 🤴 Megalodon', level: 35, points: 736, power: 16},
            {name: '🧿 🤴 BuIka', level: 32, points: 1041, power: 8},
            {name: '🧿 🧝♂️ dddevic', level: 27, points: 478, power: 5},
            {name: '🧿 🧝♀️ Akila', level: 26, points: 2176, power: 0},
            {name: '🧿 🧝♂️ NeIgnurik', level: 21, points: 1866, power: 0}
        ];

        function toggleSection(sectionId) {
            const sections = document.querySelectorAll('.members-list, .storage-list, .chicken-section');
            sections.forEach(section => {
                if(section.id === sectionId) {
                    section.style.display = section.style.display === 'none' ? 'block' : 'none';
                } else {
                    section.style.display = 'none';
                }
            });
        }

        function renderMembers() {
            const container = document.querySelector('.members-list');
            members.forEach((member, index) => {
                const row = document.createElement('div');
                row.className = 'member-row';
                row.innerHTML = `
                    <div class="rank-icon">${index+1}.</div>
                    <div>${member.name}</div>
                    <div>🔸${member.level}</div>
                    <div>🏵${member.points}</div>
                    <div>🔹${member.power}</div>
                `;
                container.appendChild(row);
            });
        }

        renderMembers();
    </script>
</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Fuel Up Lumo!</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            background-color: #f0f8ff;
            color: #333;
            text-align: center;
            padding: 20px;
        }
        .container {
            max-width: 800px;
            margin: auto;
            background: #fff;
            padding: 20px;
            border-radius: 15px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }
        h1 {
            color: #2e8b57;
        }
        .start-screen {
            display: flex;
            flex-direction: column;
            align-items: center;
        }
        .game-screen {
            display: none;
        }
        .lumo-image {
            width: 250px;
            height: auto;
            margin-bottom: 20px;
        }
        .cta-button {
            padding: 10px 20px;
            font-size: 1.2em;
            cursor: pointer;
            border: none;
            border-radius: 5px;
            background-color: #4682b4;
            color: #fff;
            margin-top: 20px;
        }
        .pantry-selection {
            display: flex;
            justify-content: center;
            gap: 10px;
            margin-top: 20px;
        }
        .food-category-button {
            padding: 10px 15px;
            font-size: 1em;
            cursor: pointer;
            border: 1px solid #ccc;
            border-radius: 5px;
            background-color: #f9f9f9;
        }
        .food-list {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 10px;
            margin-top: 20px;
        }
        .food-card {
            background: #e6e6fa;
            border: 1px solid #d3d3d3;
            border-radius: 10px;
            padding: 15px;
            width: 120px;
            cursor: pointer;
            transition: transform 0.2s;
        }
        .food-card:hover {
            transform: scale(1.05);
        }
        .food-card h4 {
            margin-top: 0;
            color: #333;
        }
        .food-card p {
            font-size: 0.9em;
            margin: 5px 0;
            line-height: 1.2;
        }
        .nutrition-meters {
            margin-top: 30px;
        }
        .meter-container {
            margin-bottom: 10px;
            text-align: left;
        }
        .meter-label {
            font-weight: bold;
            margin-bottom: 5px;
        }
        .meter-bar {
            width: 100%;
            background-color: #eee;
            border-radius: 10px;
            overflow: hidden;
        }
        .meter-fill {
            height: 20px;
            background-color: #2e8b57;
            border-radius: 10px;
            transition: width 0.5s ease-in-out;
            position: relative;
        }
        .meter-fill.vibrant {
            background-color: #ffd700;
        }
        .coin-counter {
            font-size: 1.5em;
            margin-top: 20px;
            color: #daa520;
            font-weight: bold;
        }
        .feedback-message {
            margin-top: 20px;
            font-size: 1.1em;
            font-style: italic;
            color: #8b0000;
        }
    </style>
</head>
<body>

<div class="container">
    <div class="start-screen" id="start-screen">
        <h1>Fuel Up Lumo!</h1>
        <img src="Lumo--Talking-and-Pointing (2).gif" alt="Lumo the Dragon" class="lumo-image">
        <button class="cta-button" onclick="startGame()">Choose a food to help Lumo fly!</button>
    </div>

    <div class="game-screen" id="game-screen">
        <h1>Help Lumo Fly!</h1>
        <img id="lumo-game-image" src="Lumo--Talking-and-Pointing (2).gif" alt="Lumo the Dragon" class="lumo-image">
        <p>Current Coins: <span id="coin-count">0</span></p>
        <p id="feedback-message" class="feedback-message"></p>

        <div class="nutrition-meters">
            <div class="meter-container"><div class="meter-label">Vitamin A</div><div class="meter-bar"><div class="meter-fill" id="meter-a"></div></div></div>
            <div class="meter-container"><div class="meter-label">Vitamin C</div><div class="meter-bar"><div class="meter-fill" id="meter-c"></div></div></div>
            <div class="meter-container"><div class="meter-label">Fiber</div><div class="meter-bar"><div class="meter-fill" id="meter-fiber"></div></div></div>
            <div class="meter-container"><div class="meter-label">Protein</div><div class="meter-bar"><div class="meter-fill" id="meter-protein"></div></div></div>
            <div class="meter-container"><div class="meter-label">Water</div><div class="meter-bar"><div class="meter-fill" id="meter-water"></div></div></div>
        </div>

        <div class="pantry-selection">
            <button class="food-category-button" onclick="showFoods('fruit')">Fruit</button>
            <button class="food-category-button" onclick="showFoods('veggie')">Veggie</button>
            <button class="food-category-button" onclick="showFoods('protein')">Protein</button>
        </div>

        <div id="food-list" class="food-list"></div>
    </div>
</div>

<script>
    const foodData = {
        'fruit': [
            { name: 'Apple', nutrients: { a: 10, c: 50, fiber: 25, protein: 5, water: 20 } },
            { name: 'Orange', nutrients: { a: 5, c: 70, fiber: 15, protein: 2, water: 30 } },
            { name: 'Banana', nutrients: { a: 15, c: 20, fiber: 30, protein: 10, water: 15 } }
        ],
        'veggie': [
            { name: 'Carrot', nutrients: { a: 80, c: 10, fiber: 20, protein: 5, water: 10 } },
            { name: 'Spinach', nutrients: { a: 50, c: 30, fiber: 15, protein: 15, water: 25 } },
            { name: 'Broccoli', nutrients: { a: 30, c: 60, fiber: 30, protein: 20, water: 20 } }
        ],
        'protein': [
            { name: 'Chicken', nutrients: { a: 0, c: 0, fiber: 0, protein: 80, water: 10 } },
            { name: 'Beans', nutrients: { a: 5, c: 5, fiber: 40, protein: 30, water: 15 } },
            { name: 'Fish', nutrients: { a: 10, c: 0, fiber: 0, protein: 75, water: 20 } }
        ]
    };

    let nutritionLevels = {
        a: 0, c: 0, fiber: 0, protein: 0, water: 0
    };
    let coins = 0;

    const startScreen = document.getElementById('start-screen');
    const gameScreen = document.getElementById('game-screen');
    const lumoGameImage = document.getElementById('lumo-game-image');
    const coinCounter = document.getElementById('coin-count');
    const feedbackMessage = document.getElementById('feedback-message');
    const foodListContainer = document.getElementById('food-list');

    function startGame() {
        startScreen.style.display = 'none';
        gameScreen.style.display = 'block';
    }

    function showFoods(category) {
        foodListContainer.innerHTML = ''; // Clear previous foods
        foodData[category].forEach(food => {
            const foodCard = document.createElement('div');
            foodCard.className = 'food-card';
            foodCard.innerHTML = `
                <h4>${food.name}</h4>
                <p>Adds:</p>
                ${Object.entries(food.nutrients).map(([key, value]) => {
                    if (value > 0) {
                        return `<p>${key.charAt(0).toUpperCase() + key.slice(1)}: +${value}%</p>`;
                    }
                    return '';
                }).join('')}
            `;
            foodCard.onclick = () => addFood(food);
            foodListContainer.appendChild(foodCard);
        });
    }

    function addFood(food) {
        let anyNutrientIncreased = false;
        let anyNutrientReached100 = false;
        feedbackMessage.textContent = ''; // Clear previous message
        
        // Add nutrients and update meters
        for (const nutrient in nutritionLevels) {
            if (food.nutrients[nutrient] && nutritionLevels[nutrient] < 100) {
                nutritionLevels[nutrient] += food.nutrients[nutrient];
                if (nutritionLevels[nutrient] > 100) {
                    nutritionLevels[nutrient] = 100;
                }
                anyNutrientIncreased = true;
                updateMeter(nutrient);
            }
        }
        
        if (anyNutrientIncreased) {
            lumoCheer();
            
            // Check for completed goals and give coins
            for (const nutrient in nutritionLevels) {
                if (nutritionLevels[nutrient] === 100 && !document.getElementById(`meter-${nutrient}`).classList.contains('vibrant')) {
                    document.getElementById(`meter-${nutrient}`).classList.add('vibrant');
                    anyNutrientReached100 = true;
                    feedbackMessage.textContent += `Vitamin C helps Lumo sparkle! `;
                    coins += 5;
                    coinCounter.textContent = coins;
                }
            }
            if (anyNutrientReached100) {
                lumoFly();
            } else {
                lumoCheer();
            }
        } else {
            feedbackMessage.textContent = "That's not the right food right now, Lumo can't eat any more of that!";
        }
    }

    function updateMeter(nutrient) {
        const meter = document.getElementById(`meter-${nutrient}`);
        const percentage = nutritionLevels[nutrient];
        meter.style.width = `${percentage}%`;
    }

    function lumoCheer() {
        // Simple animation placeholder
        lumoGameImage.src = 'Lumo--Talking-and-Pointing (2).gif'; // Revert to talking/pointing
    }

    function lumoFly() {
        // Lumo "glows" or "cheers" by changing the image
        lumoGameImage.src = 'Dragon-Fly-Animation (2).gif';
    }

</script>

</body>
</html>

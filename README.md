
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Arrays forEach Practice</title>
    <style>
        body { font-family: sans-serif; padding: 20px; }
        .quiz-container { border: 1px solid #ccc; padding: 15px; border-radius: 8px; }
        ul { list-style-type: square; }
    </style>
</head>
<body>
    <div class="quiz-container">
        <h1>JavaScript forEach Practice</h1>
        <p>Check the console (F12) or the list below for output:</p>
        <ul id="output-list"></ul>
    </div>

    <script>
        const fruits = ['Apple', 'Banana', 'Cherry', 'Date'];
        const listElement = document.getElementById('output-list');

        // Example: Using forEach to populate a list
        fruits.forEach((fruit, index) => {
            console.log(`${index + 1}: ${fruit}`);
            let li = document.createElement('li');
            li.textContent = fruit;
            listElement.appendChild(li);
        });
    </script>
</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Code Snippet Generator</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 20px;
        }
        .input-group {
            margin-bottom: 10px;
        }
        .input-group label {
            display: block;
            margin-bottom: 5px;
        }
        #generated-code {
            white-space: pre-wrap;
            background: #f4f4f4;
            padding: 10px;
            border: 1px solid #ccc;
            margin-top: 10px;
        }
        .hidden {
            display: none;
        }
    </style>
</head>
<body>

    <h1>Code Snippet Generator</h1>

    <div id="input-fields">
        <div class="input-group">
            <label for="buttonIds">Button IDs (comma separated):</label>
            <input type="text" id="buttonIds" placeholder="Enter Button IDs">
        </div>
        <div class="input-group">
            <label for="columnIds">Column IDs (comma separated):</label>
            <input type="text" id="columnIds" placeholder="Enter Column IDs">
        </div>
    </div>

    <button id="generate-code">Generate Code</button>

    <div id="output">
        <pre id="generated-code" class="hidden"></pre>
        <button id="copy-code" class="hidden">Copy Code</button>
    </div>

    <script>
        document.getElementById('generate-code').addEventListener('click', function() {
            const buttonIds = document.getElementById('buttonIds').value.split(',').map(id => id.trim());
            const columnIds = document.getElementById('columnIds').value.split(',').map(id => id.trim());

            if (buttonIds.length === columnIds.length && buttonIds.length > 0) {
                let buttonColumnPairs = buttonIds.map((buttonId, index) => {
                    return `{ buttonId: "${buttonId}", columnId: "${columnIds[index]}" }`;
                }).join(',\n        ');

                const generatedCode = `
<script>
document.addEventListener("DOMContentLoaded", function () {
    const buttonColumnPairs = [
        ${buttonColumnPairs}
    ];

    buttonColumnPairs.forEach(function (pair) {
        const button = document.querySelector(\`#\${pair.buttonId}\`);
        const column = document.querySelector(\`#\${pair.columnId}\`);
        column.style.display = "none";

        button.addEventListener("click", function () {
            togglePopup(pair);
        });
    });

    function togglePopup(activePair) {
        buttonColumnPairs.forEach(function (pair) {
            const column = document.querySelector(\`#\${pair.columnId}\`);
            if (pair === activePair) {
                if (column.style.display === "none") {
                    column.style.display = "block";
                } else {
                    column.style.display = "none";
                }
            } else {
                column.style.display = "none";
            }
        });
    }
});
</script>`;

                document.getElementById('generated-code').textContent = generatedCode.trim();
                document.getElementById('generated-code').classList.remove('hidden');
                document.getElementById('copy-code').classList.remove('hidden');
            } else {
                alert('Please enter an equal number of Button IDs and Column IDs.');
            }
        });

        document.getElementById('copy-code').addEventListener('click', function() {
            const code = document.getElementById('generated-code');
            const range = document.createRange();
            range.selectNodeContents(code);
            const selection = window.getSelection();
            selection.removeAllRanges();
            selection.addRange(range);

            try {
                document.execCommand('copy');
                alert('Code copied to clipboard!');
            } catch (err) {
                alert('Failed to copy code.');
            }

            selection.removeAllRanges();
        });
    </script>

</body>
</html>

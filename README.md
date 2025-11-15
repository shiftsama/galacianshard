<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Online ROM Patcher</title>
    <link rel="stylesheet" href="assets/css/rompatcher.css">
    <style>
        body { font-family: Arial, sans-serif; margin: 20px; }
        h1 { color: #333; }
    </style>
</head>
<body>
    <h1>Online ROM Patcher</h1>
    <div id="rompatcher"></div>

    <!-- RomPatcher.js scripts -->
    <script src="assets/js/rompatcher.js"></script>
    <script>
        // Initialize RomPatcher in the target div
        document.addEventListener('DOMContentLoaded', function() {
            new MarcFilePatcher({
                target: document.getElementById('rompatcher'),
                workerPath: 'assets/js/rompatcher.worker.js'
            });
        });
    </script>
</body>
</html>
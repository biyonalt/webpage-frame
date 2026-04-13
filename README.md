
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>4-Section Layout Webpage</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            height: 100vh;
            display: flex;
            flex-direction: column;
        }

        .container {
            display: grid;
            grid-template-columns: 1fr 1fr;
            grid-template-rows: 1fr 1fr;
            height: 100vh;
            gap: 0;
        }

        .section {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            padding: 40px;
            text-align: center;
            transition: transform 0.3s ease;
        }

        .section:hover {
            transform: scale(1.02);
        }

        /* Top-Left Section */
        .section-1 {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
        }

        /* Top-Right Section */
        .section-2 {
            background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%);
            color: white;
        }

        /* Bottom-Left Section */
        .section-3 {
            background: linear-gradient(135deg, #4facfe 0%, #00f2fe 100%);
            color: white;
        }

        /* Bottom-Right Section */
        .section-4 {
            background: linear-gradient(135deg, #43e97b 0%, #38f9d7 100%);
            color: white;
        }

        h1 {
            font-size: 2.5rem;
            margin-bottom: 15px;
            font-weight: 700;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.3);
        }

        p {
            font-size: 1.1rem;
            line-height: 1.6;
            opacity: 0.9;
            max-width: 400px;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .container {
                grid-template-columns: 1fr;
                grid-template-rows: auto;
                height: auto;
            }

            .section {
                min-height: 50vh;
            }

            h1 {
                font-size: 2rem;
            }

            p {
                font-size: 1rem;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Top-Left Section -->
        <div class="section section-1">
            <h1>📱 Section One</h1>
            <p>Purple gradient background with modern design. Perfect for showcasing digital products.</p>
        </div>

        <!-- Top-Right Section -->
        <div class="section section-2">
            <h1>❤️ Section Two</h1>
            <p>Pink and red gradient creating a vibrant, energetic atmosphere for your content.</p>
        </div>

        <!-- Bottom-Left Section -->
        <div class="section section-3">
            <h1>💙 Section Three</h1>
            <p>Cool blue and cyan gradient ideal for tech and innovative content presentation.</p>
        </div>

        <!-- Bottom-Right Section -->
        <div class="section section-4">
            <h1>💚 Section Four</h1>
            <p>Fresh green gradient perfect for eco-friendly, growth, or positive messaging.</p>
        </div>
    </div>
</body>
</html>

# eng23ds0090
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Travel Itinerary Planner</title>
    <style>
        /* General Reset */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Arial', sans-serif;
            background-color: #f4f4f9;
            color: #333;
        }

        /* Navigation Bar */
        nav {
            background-color: #00796b;
            padding: 15px;
            text-align: center;
        }

        nav ul {
            list-style-type: none;
        }

        nav ul li {
            display: inline;
            margin: 0 20px;
        }

        nav ul li a {
            text-decoration: none;
            color: white;
            font-size: 1.2em;
        }

        nav ul li a:hover {
            color: #c1e8e3;
        }

        /* Hero Section */
        .hero {
            background-color: #004d40;
            color: white;
            padding: 100px 20px;
            text-align: center;
        }

        .hero h1 {
            font-size: 3.5em;
            margin-bottom: 20px;
        }

        .hero p {
            font-size: 1.2em;
            margin-bottom: 30px;
        }

        .hero button {
            padding: 15px 30px;
            background-color: #00796b;
            color: white;
            border: none;
            font-size: 1.1em;
            cursor: pointer;
            border-radius: 5px;
        }

        .hero button:hover {
            background-color: #004d40;
        }

        /* Itinerary Planner Section */
        .itinerary-planner {
            background-color: #ffffff;
            padding: 50px 20px;
            max-width: 1000px;
            margin: 0 auto;
        }

        .itinerary-planner h2 {
            font-size: 2.5em;
            margin-bottom: 40px;
            text-align: center;
            color: #00796b;
        }

        .itinerary-container {
            display: flex;
            flex-wrap: wrap;
            gap: 30px;
            justify-content: space-between;
        }

        .itinerary-card {
            background-color: #e0f2f1;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            width: calc(33% - 20px);
            transition: transform 0.3s ease;
        }

        .itinerary-card:hover {
            transform: scale(1.05);
        }

        .itinerary-card img {
            width: 100%;
            height: 250px;
            object-fit: cover;
            border-radius: 5px;
        }

        .itinerary-card h3 {
            font-size: 1.8em;
            color: #00796b;
            margin-top: 15px;
        }

        .itinerary-card p {
            font-size: 1.1em;
            color: #333;
            margin-top: 10px;
        }

        .social-share {
            margin-top: 15px;
        }

        .social-share a {
            margin: 0 10px;
            text-decoration: none;
            font-size: 1.2em;
            color: #00796b;
        }

        .social-share a:hover {
            color: #004d40;
        }

        /* Add New Itinerary Section */
        .add-itinerary {
            margin-top: 40px;
            text-align: center;
        }

        .add-itinerary input,
        .add-itinerary textarea,
        .add-itinerary select {
            padding: 12px;
            font-size: 1.1em;
            margin: 10px;
            width: 300px;
            border: 2px solid #00796b;
            border-radius: 5px;
        }

        .add-itinerary button {
            padding: 12px 30px;
            background-color: #00796b;
            color: white;
            border: none;
            border-radius: 5px;
            font-size: 1.2em;
            cursor: pointer;
        }

        .add-itinerary button:hover {
            background-color: #004d40;
        }

        /* Footer Section */
        footer {
            background-color: #00796b;
            color: white;
            text-align: center;
            padding: 20px;
            margin-top: 40px;
        }

    </style>
</head>
<body>

    <!-- Navigation Bar -->
    <nav>
        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#itinerary">Itinerary</a></li>
            <li><a href="#add-itinerary">Add Itinerary</a></li>
        </ul>
    </nav>

    <!-- Hero Section -->
    <section class="hero" id="home">
        <h1>Plan Your Next Adventure</h1>
        <p>Effortlessly create your travel itinerary and make your journey memorable.</p>
        <button>Start Planning</button>
    </section>

    <!-- Itinerary Section -->
    <section class="itinerary-planner" id="itinerary">
        <h2>Your Travel Itinerary</h2>
        <div class="itinerary-container">
            <div class="itinerary-card">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQPK7gzVvAp5IQtgW5OUuTUDyfVZSMU5RvxKQ&s" alt="Paris">
                <h3>Paris - The City of Love</h3>
                <p>Duration: 5 Days</p>
                <p>Visit iconic landmarks like the Eiffel Tower, the Louvre Museum, and enjoy a Seine River cruise.</p>
                <div class="social-share">
                    <a href="#">Share on Facebook</a><br>
                    <a href="#">Share on Twitter</a><br>
                    <a href="#">Share on Instagram</a><br>
                </div>
            </div>
            <div class="itinerary-card">
                <img src="https://images.unsplash.com/photo-1540959733332-eab4deabeeaf?fm=jpg&q=60&w=3000&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxzZWFyY2h8MTR8fHRva3lvfGVufDB8fDB8fHww" alt="Tokyo">
                <h3>Tokyo - Vibrant Cityscape</h3>
                <p>Duration: 4 Days</p>
                <p>Explore Tokyo Tower, Shibuya Crossing, and traditional temples like Sensoji.</p>
                <div class="social-share">
                    <a href="#">Share on Facebook</a><br>
                    <a href="#">Share on Twitter</a><br>
                    <a href="#">Share on Instagram</a><br>
                </div>
            </div>
            <div class="itinerary-card">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQJJyn_DR6mTTC09kmEBHkT7wt-e-oNzrF6gg&s" alt="New York">
                <h3>New York - The Big Apple</h3>
                <p>Duration: 7 Days</p>
                <p>Discover the Statue of Liberty, Central Park, and Broadway shows.</p>
                <div class="social-share">
                    <a href="#">Share on Facebook</a><br>
                    <a href="#">Share on Twitter</a><br>
                    <a href="#">Share on Instagram</a><br>
                </div>
            </div>
        </div>
    </section>

    <!-- Add New Itinerary Section -->
    <section class="add-itinerary" id="add-itinerary">
        <h2>Add Your Own Itinerary</h2>
        <form>
            <input type="text" placeholder="Destination Name" required><br>
            <textarea placeholder="Brief Description" required></textarea><br>
            <input type="file" name="image" accept="image/*"><br>
            <select required>
                <option value="" disabled selected>Duration (in days)</option>
                <option value="3">3 Days</option>
                <option value="5">5 Days</option>
                <option value="7">7 Days</option>
                <option value="10">10 Days</option>
            </select><br>
            <button type="submit">Add Itinerary</button>
        </form>
    </section>

    <!-- Footer -->
    <footer>
        <p>&copy; 2024 Travel Itinerary Planner. All Rights Reserved.</p>
    </footer>

</body>
</html>

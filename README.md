<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Blog Home</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <div class="container">
            <h1>My Blog</h1>
            <nav>
                <ul>
                    <li><a href="/">Home</a></li>
                    <li><a href="/new-post">New Post</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <main>
        <div class="container">
            <h2>Recent Posts</h2>
            <div id="posts">
                <!-- Posts will be dynamically added here -->
            </div>
        </div>
    </main>

    <footer>
        <div class="container">
            <p>&copy; 2024 My Blog. All rights reserved.</p>
        </div>
    </footer>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>New Post</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <div class="container">
            <h1>My Blog</h1>
            <nav>
                <ul>
                    <li><a href="/">Home</a></li>
                    <li><a href="/new-post">New Post</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <main>
        <div class="container">
            <h2>Create New Post</h2>
            <form action="/posts" method="POST">
                <div class="form-group">
                    <label for="title">Title:</label>
                    <input type="text" id="title" name="title" required>
                </div>
                <div class="form-group">
                    <label for="content">Content:</label>
                    <textarea id="content" name="content" rows="10" required></textarea>
                </div>
                <button type="submit">Submit</button>
            </form>
        </div>
    </main>

    <footer>
        <div class="container">
            <p>&copy; 2024 My Blog. All rights reserved.</p>
        </div>
    </footer>
</body>
</html>
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f4f4f4;
    color: #333;
}

header {
    background-color: #333;
    color: white;
    padding: 10px 0;
    text-align: center;
}

header h1 {
    margin: 0;
}

header nav ul {
    list-style-type: none;
    padding: 0;
}

header nav ul li {
    display: inline;
    margin: 0 15px;
}

header nav ul li a {
    color: white;
    text-decoration: none;
}

.container {
    width: 80%;
    margin: 0 auto;
    padding: 20px 0;
}

main {
    margin: 20px 0;
}

h2 {
    margin-top: 0;
}

.form-group {
    margin-bottom: 15px;
}

label {
    display: block;
    margin-bottom: 5px;
}

input, textarea {
    width: 100%;
    padding: 10px;
    border: 1px solid #ccc;
    border-radius: 5px;
}

button {
    padding: 10px 15px;
    border: none;
    background-color: #5cb85c;
    color: white;
    border-radius: 5px;
    cursor: pointer;
}

button:hover {
    background-color: #4cae4c;
}

footer {
    background-color: #333;
    color: white;
    text-align: center;
    padding: 10px 0;
    position: fixed;
    bottom: 0;
    width: 100%;
}

footer p {
    margin: 0;
}

.post {
    background-color: #fff;
 padding: 15px;
    margin: 10px 0;
    border-radius: 5px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

.post h3 {
    margin-top: 0;
}

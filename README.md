:root {
    --primary-color: #2d3436;
    --accent-color: #0984e3;
    --text-light: #636e72;
    --bg-light: #f9f9f9;
}

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

body {
    line-height: 1.6;
    color: var(--primary-color);
    background-color: #fff;
}

/* Navigation */
nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1.5rem 10%;
    background: #fff;
    box-shadow: 0 2px 5px rgba(0,0,0,0.1);
    position: fixed;
    width: 100%;
    top: 0;
    z-index: 1000;
}

nav ul { display: flex; list-style: none; }
nav ul li { margin-left: 2rem; }
nav ul li a { text-decoration: none; color: var(--primary-color); font-weight: bold; }

/* Hero Section */
#hero {
    height: 100vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    text-align: center;
    background: var(--bg-light);
    padding: 0 10%;
}

.highlight { color: var(--accent-color); }

.btn {
    margin-top: 2rem;
    padding: 0.8rem 2rem;
    background: var(--accent-color);
    color: #fff;
    text-decoration: none;
    border-radius: 5px;
    transition: 0.3s;
}

/* Projects */
#projects { padding: 5rem 10%; }
.project-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 2rem;
    margin-top: 2rem;
}

.project-card {
    padding: 2rem;
    border: 1px solid #ddd;
    border-radius: 8px;
    transition: transform 0.3s;
}

.project-card:hover { transform: translateY(-10px); }

/* Footer */
footer {
    text-align: center;
    padding: 4rem 10%;
    background: var(--primary-color);
    color: #fff;
}

.social-links a {
    color: #fff;
    font-size: 2rem;
    margin: 0 1rem;
    text-decoration: none;
}

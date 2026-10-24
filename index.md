# Assignment 5.5 — CSS Fundamentals Mini-Project

## File 1: `index.html`

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>College Club - Home</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>College Club</h1>
        <nav>
            <a href="index.html">Home</a>
            <a href="about.html">About</a>
            <a href="registration.html">Registration</a>
            <a href="contact.html">Contact</a>
        </nav>
    </header>

    <main>
        <section class="hero">
            <h2>Welcome to Our College Club</h2>
            <p>Join our club to learn new skills, share ideas, and participate in exciting activities.</p>
            <a class="button" href="registration.html">Join Us</a>
        </section>

        <section class="card">
            <h2>Our Activities</h2>
            <p>We organize workshops, group discussions, competitions, and college events.</p>
        </section>
    </main>

    <footer>
        <p>College Club Website</p>
    </footer>
</body>
</html>
```

## File 2: `about.html`

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>About Us - College Club</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>College Club</h1>
        <nav>
            <a href="index.html">Home</a>
            <a href="about.html">About</a>
            <a href="registration.html">Registration</a>
            <a href="contact.html">Contact</a>
        </nav>
    </header>

    <main>
        <section class="card">
            <h2>About Our Club</h2>
            <p>Our college club encourages students to learn, collaborate, and develop their skills.</p>
            <p>We welcome students who want to participate in activities and work together as a team.</p>
        </section>

        <section class="card">
            <h2>Club Members</h2>
            <table>
                <thead>
                    <tr>
                        <th>Role</th>
                        <th>Responsibility</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td>President</td>
                        <td>Leads club activities</td>
                    </tr>
                    <tr>
                        <td>Secretary</td>
                        <td>Manages records</td>
                    </tr>
                    <tr>
                        <td>Member</td>
                        <td>Participates in events</td>
                    </tr>
                </tbody>
            </table>
        </section>
    </main>

    <footer>
        <p>College Club Website</p>
    </footer>
</body>
</html>
```

## File 3: `registration.html`

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Registration - College Club</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>College Club</h1>
        <nav>
            <a href="index.html">Home</a>
            <a href="about.html">About</a>
            <a href="registration.html">Registration</a>
            <a href="contact.html">Contact</a>
        </nav>
    </header>

    <main>
        <section class="card">
            <h2>Club Registration</h2>
            <form>
                <label for="name">Full Name</label>
                <input type="text" id="name" name="name" required>

                <label for="email">Email</label>
                <input type="email" id="email" name="email" required>

                <label for="course">Course</label>
                <input type="text" id="course" name="course" required>

                <button type="submit">Register</button>
            </form>
        </section>
    </main>

    <footer>
        <p>College Club Website</p>
    </footer>
</body>
</html>
```

## File 4: `contact.html`

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contact - College Club</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>College Club</h1>
        <nav>
            <a href="index.html">Home</a>
            <a href="about.html">About</a>
            <a href="registration.html">Registration</a>
            <a href="contact.html">Contact</a>
        </nav>
    </header>

    <main>
        <section class="card">
            <h2>Contact Us</h2>
            <p>Email: club@example.com</p>
            <p>Location: College Campus</p>
        </section>

        <section class="card">
            <h2>Upcoming Events</h2>
            <table>
                <thead>
                    <tr>
                        <th>Event</th>
                        <th>Activity</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td>Workshop</td>
                        <td>Skill Development</td>
                    </tr>
                    <tr>
                        <td>Competition</td>
                        <td>Student Participation</td>
                    </tr>
                </tbody>
            </table>
        </section>
    </main>

    <footer>
        <p>College Club Website</p>
    </footer>
</body>
</html>
```

## File 5: `style.css`

```css
:root {
    --primary-color: #1d4ed8;
    --secondary-color: #0f172a;
    --background-color: #f1f5f9;
    --card-color: #ffffff;
    --text-color: #334155;
    --spacing-small: 8px;
    --spacing-medium: 16px;
    --spacing-large: 32px;
}

* {
    box-sizing: border-box;
}

body {
    margin: 0;
    font-family: Arial, sans-serif;
    background-color: var(--background-color);
    color: var(--text-color);
    line-height: 1.6;
}

header {
    background-color: var(--secondary-color);
    color: white;
    padding: var(--spacing-medium);
    text-align: center;
}

header h1 {
    margin: var(--spacing-small);
}

nav {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: var(--spacing-medium);
}

nav a {
    color: white;
    text-decoration: none;
    padding: var(--spacing-small);
}

nav a:hover {
    color: #93c5fd;
}

main {
    max-width: 900px;
    margin: var(--spacing-large) auto;
    padding: 0 var(--spacing-medium);
}

h2 {
    color: var(--primary-color);
}

p {
    font-size: 16px;
}

.hero {
    background-color: var(--card-color);
    padding: var(--spacing-large);
    text-align: center;
    border-radius: 10px;
    margin-bottom: var(--spacing-large);
}

.card {
    background-color: var(--card-color);
    padding: var(--spacing-large);
    margin-bottom: var(--spacing-large);
    border-radius: 10px;
    box-shadow: 0 2px 8px rgba(0, 0, 0, 0.08);
}

.button,
button {
    display: inline-block;
    background-color: var(--primary-color);
    color: white;
    padding: var(--spacing-small) var(--spacing-medium);
    border: none;
    border-radius: 5px;
    text-decoration: none;
    cursor: pointer;
}

.button:hover,
button:hover {
    background-color: #1e40af;
}

form {
    display: flex;
    flex-direction: column;
    gap: var(--spacing-small);
}

input {
    width: 100%;
    padding: var(--spacing-small);
    border: 1px solid #cbd5e1;
    border-radius: 5px;
    margin-bottom: var(--spacing-medium);
}

input:focus {
    outline: 2px solid var(--primary-color);
}

table {
    width: 100%;
    border-collapse: collapse;
    background-color: var(--card-color);
}

th,
td {
    border: 1px solid #cbd5e1;
    padding: var(--spacing-medium);
    text-align: left;
}

th {
    background-color: var(--primary-color);
    color: white;
}

tr:nth-child(even) {
    background-color: #e2e8f0;
}

footer {
    background-color: var(--secondary-color);
    color: white;
    text-align: center;
    padding: var(--spacing-medium);
}

@media (max-width: 600px) {
    nav {
        flex-direction: column;
        gap: var(--spacing-small);
    }

    main {
        margin: var(--spacing-medium) auto;
    }

    .card,
    .hero {
        padding: var(--spacing-medium);
    }
}
```

## Design Choices

1. A consistent blue, dark navy, and light grey color palette is used throughout the website.
2. Arial typography and readable line spacing improve readability.
3. CSS variables make colors and spacing easy to reuse and update.
4. Navigation, buttons, forms, and tables use consistent styling.
5. Chrome DevTools can be used to inspect elements and debug CSS issues.
6.
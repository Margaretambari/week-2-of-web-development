

Complete HTML5 form including a variety of input fields.

Correct use of form attributes such as placeholder, required, autocomplete, and readonly.

HTML5 validation features implemented correctly across all relevant fields.

A clear, accessible layout using semantic tags.




HTML

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Enhanced Form Submission</title>
</head>
<body>

    <header>
        <h1>Enhanced Form Submission</h1>
        <p>Please complete the form below to register for our upcoming workshop.</p>
    </header>

    <main>
        
        <section>
            <h2>Workshop Details</h2>
            <p>Our workshop will cover the following topics:</p>
            <ul>
                <li>Introduction to HTML5</li>
                <li>Advanced CSS Techniques</li>
                <li>JavaScript Fundamentals</li>
                <li>Responsive Web Design</li>
            </ul>

            <h3>Event Schedule</h3>
            <table>
                <thead>
                    <tr>
                        <th>Time</th>
                        <th>Topic</th>
                        <th>Presenter</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td>9:00 AM - 10:30 AM</td>
                        <td>HTML5 Forms & Validation</td>
                        <td>Jane Doe</td>
                    </tr>
                    <tr>
                        <td>10:45 AM - 12:15 PM</td>
                        <td>CSS Grid & Flexbox</td>
                        <td>John Smith</td>
                    </tr>
                    <tr>
                        <td>1:30 PM - 3:00 PM</td>
                        <td>Introduction to DOM Manipulation</td>
                        <td>Alice Johnson</td>
                    </tr>
                </tbody>
            </table>

            <h3>Workshop Highlights</h3>
            <figure>
                <img src="https://via.placeholder.com/600x300.png?text=Workshop+Image" alt="Image of a coding workshop in progress." width="600" height="300">
                <figcaption>A placeholder image representing a workshop environment.</figcaption>
            </figure>
        </section>

        <section>
            <h2>Registration Form</h2>
            <form action="#" method="post" autocomplete="on">

                <fieldset>
                    <legend>Personal Information</legend>
                    <label for="fullName">Full Name:</label>
                    <input type="text" id="fullName" name="fullName" placeholder="e.g., Jane Doe" required autocomplete="name">
                    <br><br>

                    <label for="email">Email:</label>
                    <input type="email" id="email" name="email" placeholder="e.g., jane.doe@example.com" required autocomplete="email">
                    <br><br>
                    
                    <label for="phone">Phone Number:</label>
                    <input type="tel" id="phone" name="phone" placeholder="e.g., 555-123-4567" pattern="[0-9]{3}-[0-9]{3}-[0-9]{4}" required autocomplete="tel">
                    <small>Format: 123-456-7890</small>
                    <br><br>
                </fieldset>

                <fieldset>
                    <legend>Workshop Preferences</legend>
                    <label for="workshopDate">Preferred Date:</label>
                    <input type="date" id="workshopDate" name="workshopDate" required>
                    <br><br>
                    
                    <label for="workshopTime">Preferred Time:</label>
                    <input type="time" id="workshopTime" name="workshopTime">
                    <br><br>

                    <label for="skillLevel">Skill Level:</label>
                    <select id="skillLevel" name="skillLevel" required>
                        <option value="" disabled selected>Select your skill level</option>
                        <option value="beginner">Beginner</option>
                        <option value="intermediate">Intermediate</option>
                        <option value="advanced">Advanced</option>
                    </select>
                    <br><br>

                    <label>Dietary Restrictions:</label><br>
                    <input type="checkbox" id="vegetarian" name="dietary" value="vegetarian">
                    <label for="vegetarian">Vegetarian</label><br>
                    <input type="checkbox" id="vegan" name="dietary" value="vegan">
                    <label for="vegan">Vegan</label><br>
                    <input type="checkbox" id="glutenFree" name="dietary" value="glutenFree">
                    <label for="glutenFree">Gluten-Free</label><br>
                </fieldset>

                <fieldset>
                    <legend>Additional Information</legend>
                    <label for="notes">Notes:</label>
                    <textarea id="notes" name="notes" rows="4" cols="50" placeholder="e.g., Any specific questions you have for the presenters?"></textarea>
                    <br><br>

                    <label for="username">Username:</label>
                    <input type="text" id="username" name="username" readonly value="auto-generated-user">
                    <small>This field is pre-filled and cannot be changed.</small>
                    <br><br>

                    <input type="submit" value="Register">
                    <input type="reset" value="Reset Form">
                </fieldset>
            </form>
        </section>

    </main>

    <footer>
        <p>&copy; 2025 Workshop Registration. All rights reserved.</p>
    </footer>

</body>
</html>

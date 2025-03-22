# Advanced HTML5 Elements and Forms

## Objectives
Implement HTML5 images, lists, tables, forms and input types.
Use form validation attributes.
Apply multimedia elements such as audio and video.

## Instructions

- Create an index.html file.
- Add an ordered list with roman numerals
- Add an external image from pexels.com
- Add a table of 5 contacts with; name, address, mobile and emails
- Add a registration form

>[!NOTE]
>  The registration form should have:
>- Name, email, password, and date fields.
>- A dropdown, radio buttons, and checkboxes.
>- Proper labels and placeholders.
>- Required fields and validation attributes.
>- Ensure proper indentation and commenting.
 
# Tasks
- Create a well-structured HTML5 document.
- Ensure semantic correctness.

Happy Coding! 💻✨


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Assignment Page</title>
    <style>
        table, th, td {
            border: 1px solid black;
            border-collapse: collapse;
            padding: 8px;
        }
        .form-group {
            margin-bottom: 10px;
        }
    </style>
</head>
<body>
    <!-- Ordered List with Roman Numerals -->
    <h2>Top 3 Priorities</h2>
    <ol type="I">
        <li>Complete HTML Assignment</li>
        <li>Practice CSS Styling</li>
        <li>Learn JavaScript Basics</li>
    </ol>

    <!-- External Image from Pexels -->
    <h2>Nature Image</h2>
    <img src="https://images.pexels.com/photos/268533/pexels-photo-268533.jpeg" 
         alt="Nature Photo" 
         width="400"
         height="300">

    <!-- Contacts Table -->
    <h2>Contact List</h2>
    <table>
        <thead>
            <tr>
                <th>Name</th>
                <th>Address</th>
                <th>Mobile</th>
                <th>Email</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>John Doe</td>
                <td>123 Main St</td>
                <td>555-1234</td>
                <td>john@email.com</td>
            </tr>
            <tr>
                <td>Jane Smith</td>
                <td>456 Oak Ave</td>
                <td>555-5678</td>
                <td>jane@email.com</td>
            </tr>
            <tr>
                <td>Bob Johnson</td>
                <td>789 Pine Rd</td>
                <td>555-9012</td>
                <td>bob@email.com</td>
            </tr>
            <tr>
                <td>Alice Brown</td>
                <td>321 Elm St</td>
                <td>555-3456</td>
                <td>alice@email.com</td>
            </tr>
            <tr>
                <td>Charlie Wilson</td>
                <td>654 Maple Dr</td>
                <td>555-7890</td>
                <td>charlie@email.com</td>
            </tr>
        </tbody>
    </table>

    <!-- Registration Form -->
    <h2>Registration Form</h2>
    <!-- Registration Form Section -->
<h2>Registration Form</h2>
<form>
    <!-- Personal Information -->
    <div class="form-group">
        <label for="name">Full Name: <span class="required">*</span></label>
        <input type="text" id="name" name="name" 
               placeholder="John Doe" 
               required 
               minlength="3"
               pattern="[A-Za-z ]+">
    </div>

    <!-- Contact Information -->
    <div class="form-group">
        <label for="email">Email: <span class="required">*</span></label>
        <input type="email" id="email" name="email" 
               placeholder="john.doe@example.com" 
               required>
    </div>

    <div class="form-group">
        <label for="password">Password: <span class="required">*</span></label>
        <input type="password" id="password" name="password" 
               placeholder="••••••••" 
               required 
               minlength="8">
    </div>

    <!-- Date Input -->
    <div class="form-group">
        <label for="birthdate">Date of Birth: <span class="required">*</span></label>
        <input type="date" id="birthdate" name="birthdate" 
               required 
               max="2024-01-01">
    </div>

    <!-- Dropdown Menu -->
    <div class="form-group">
        <label for="country">Country: <span class="required">*</span></label>
        <select id="country" name="country" required>
            <option value="" disabled selected>Select Country</option>
            <option value="usa">United States</option>
            <option value="canada">Canada</option>
            <option value="uk">United Kingdom</option>
            <option value="other">Other</option>
        </select>
    </div>

    <!-- Radio Buttons -->
    <div class="form-group">
        <label>Gender: <span class="required">*</span></label>
        <div class="radio-group">
            <label>
                <input type="radio" name="gender" value="male" required>
                Male
            </label>
            <label>
                <input type="radio" name="gender" value="female">
                Female
            </label>
            <label>
                <input type="radio" name="gender" value="other">
                Prefer not to say
            </label>
        </div>
    </div>

    <!-- Checkboxes -->
    <div class="form-group">
        <label>Subscription Options:</label>
        <div class="checkbox-group">
            <label>
                <input type="checkbox" name="newsletter">
                Subscribe to newsletter
            </label>
            <label>
                <input type="checkbox" name="terms" required>
                I agree to terms and conditions <span class="required">*</span>
            </label>
        </div>
    </div>

    <button type="submit">Register</button>
</form>

<style>
    .required {
        color: red;
        font-size: 0.8em;
    }
    
    .form-group {
        margin-bottom: 1rem;
    }
    
    .radio-group, .checkbox-group {
        display: flex;
        flex-direction: column;
        gap: 0.5rem;
    }
    
    select {
        padding: 0.3rem;
        width: 200px;
    }
    
    input[type="text"],
    input[type="email"],
    input[type="password"],
    input[type="date"] {
        padding: 0.5rem;
        width: 250px;
    }
</style>
<form>
</body>
</html>
   

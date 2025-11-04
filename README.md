<style>

body {
    /* Optional: Set a background color for the page */
    background-color: #457ecf; 
    font-family: Arial, sans-serif;
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    margin: 0;
}

form {
    /* Main container styling */
    background-color: #ffffff;
    padding: 40px;
    border-radius: 10px;
    box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
    width: 100%;
    max-width: 400px; /* Limit the form width */
    display: flex;
    flex-direction: column;
    gap: 15px; /* Space between form elements */
}

input[type="text"], 
input[type="email"], 
textarea {
    /* Styling for all input fields and textarea */
    width: 100%;
    padding: 12px;
    border: 1px solid #ccc;
    border-radius: 6px;
    box-sizing: border-box; /* Include padding/border in the element's total width/height */
    transition: border-color 0.3s ease, box-shadow 0.3s ease;
    font-size: 16px;
}

input[type="text"]:focus, 
input[type="email"]:focus, 
textarea:focus {
    /* Styling when an input is clicked/active */
    border-color: #007bff; /* Highlight border */
    box-shadow: 0 0 5px rgba(0, 123, 255, 0.5);
    outline: none; /* Remove default browser outline */
}

textarea {
    /* Specific styling for the message box */
    resize: vertical; /* Allow vertical resizing, but not horizontal */
    min-height: 120px;
}

button[type="submit"] {
    /* Styling for the submit button */
    background-color: #007bff; /* Primary button color */
    color: white;
    padding: 12px 20px;
    border: none;
    border-radius: 6px;
    cursor: pointer;
    font-size: 16px;
    font-weight: bold;
    letter-spacing: 1px;
    transition: background-color 0.3s ease, transform 0.1s ease;
}

button[type="submit"]:hover {
    /* Slight darkening/lift on mouse hover */
    background-color: #0056b3;
    transform: translateY(-1px);
}
</style>
<form action="http://10.53.89.148/submit.php" method="post">
    <input type="text" name="name" placeholder="Your Name" required>
    <input type="email" name="email" placeholder="Your Email" required>
    <textarea name="message" placeholder="Your message" required></textarea>
    <button type="submit">Send</button>
</form>


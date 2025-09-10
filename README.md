# -Basic-Computer-Classes-Survey-Form
<!DOCTYPE html>
<html>
<head>
  <title>Basic Computer Classes - Student Survey</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #f0f4f8;
      display: flex;
      justify-content: center;
      align-items: center;
      min-height: 100vh;
    }
    .survey-form {
      background: #fff;
      padding: 25px;
      width: 400px;
      border-radius: 12px;
      box-shadow: 0 0 10px rgba(0,0,0,0.2);
    }
    h2 {
      text-align: center;
      color: #333;
    }
    label {
      font-weight: bold;
      margin-top: 10px;
      display: block;
      color: #444;
    }
    input, select, textarea {
      width: 100%;
      padding: 10px;
      margin-top: 6px;
      margin-bottom: 15px;
      border: 1px solid #ccc;
      border-radius: 6px;
    }
    textarea {
      resize: none;
    }
    button {
      width: 100%;
      padding: 12px;
      background: #4CAF50;
      color: white;
      font-size: 16px;
      border: none;
      border-radius: 6px;
      cursor: pointer;
    }
    button:hover {
      background: #45a049;
    }
  </style>
</head>
<body>

  <form class="survey-form" action="/submit" method="post">
    <h2>Student Survey Form</h2>

    <label for="name">Full Name:</label>
    <input type="text" id="name" name="name" required>

    <label for="email">Email:</label>
    <input type="email" id="email" name="email" required>

    <label for="rating">How would you rate the classes?</label>
    <select id="rating" name="rating" required>
      <option value="">--Select--</option>
      <option value="excellent">Excellent</option>
      <option value="good">Good</option>
      <option value="average">Average</option>
      <option value="poor">Poor</option>
    </select>

    <label>Which topics did you find most useful?</label>
    <input type="checkbox" name="topics" value="ms-office"> MS Office<br>
    <input type="checkbox" name="topics" value="internet"> Internet Basics<br>
    <input type="checkbox" name="topics" value="typing"> Typing Skills<br>
    <input type="checkbox" name="topics" value="others"> Others<br><br>

    <label for="experience">Share your experience:</label>
    <textarea id="experience" name="experience" rows="4" required></textarea>

    <label for="suggestions">Any suggestions for improvement?</label>
    <textarea id="suggestions" name="suggestions" rows="3"></textarea>

    <button type="submit">Submit Survey</button>
  </form>

</body>
</html>

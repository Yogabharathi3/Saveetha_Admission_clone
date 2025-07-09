# Saveetha_Admission_clone
## Date:09.07.2025

## Objective:
To design a landing page clone of Saveetha Engineering College’s Admission Enquiry form using HTML and CSS. This activity reinforces skills in layout design, form creation, user input handling, responsive structure, and visual styling based on a real-world example.

## Tasks:
#### 1. Analyze the Landing Page Layout:
Observe the split-screen layout with a promotional section on the left and a form on the right.

Note the use of background images, text styling, and branding elements.

#### 2. Create the HTML Structure:
Use semantic tags like ```<section>, <header>, <form>, and <footer>``` to organize content.

Structure the form with input fields such as name, email, phone, password, city, state, course, specialization, captcha, and checkbox.

#### 3. Add Form Functionality:
Include appropriate input types (text, email, tel, password, select, etc.) with placeholders and labels.

Use the <button> element for the "APPLY NOW" action.

#### 4. Apply CSS Styling:
Implement a split layout using flexbox or grid.

Style the form elements with padding, shadows, background colors, and rounded borders.

Include hover effects and button transitions to match the original look.

#### 5. Incorporate Images and Branding:
Add the institution logo and use matching fonts and colors.

Place a background image or blurred overlay behind the form content if needed.

#### 6. Ensure Responsiveness:
Make sure the page adapts to different screen sizes using media queries.

Maintain readability and layout integrity on both desktop and mobile.

## HTML Code:
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Admission Enquiry - Saveetha Engineering College</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>

  <div class="form-container">
    <h2>Admissions Open 2025</h2>

    <form>
      <input type="text" placeholder="Enter Name *">
      <input type="email" placeholder="Enter Email Address *">

      <div class="phone-group">
        <select>
          <option>+91</option>
        </select>
        <input type="tel" placeholder="Enter Mobile Number *">
      </div>

      <input type="password" placeholder="Any Password *">

      <div class="two-cols">
        <input type="text" placeholder="State *">
        <input type="text" placeholder="City *">
      </div>

      <div class="two-cols">
        <input type="text" placeholder="Course *" >
        <input type="text" placeholder="Specialization *" >
      </div>

      <div class="captcha">
        <img src="captcha.png" alt="captcha">
        <input type="text" placeholder="Enter text*">
      </div>

     <div class="checkbox">
  <label>
    <input type="checkbox">
    I authorise Saveetha Engineering College & its representatives to contact me with updates and notifications via Email/SMS/WhatsApp/Call. This will override DND/NDNC *
  </label>
</div>

      <button type="submit" class="submit-btn">APPLY NOW </button>

      <p class="login-link">Already have an Account? 
        <a >Login</a><br>
        <a>Resend Verification Email</a></p>
    </form>
  </div>

</body>
</html>
```
## CSS Code:
```
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Segoe UI", sans-serif;
}

body {
  background: url('saveetha.jpg') center center/cover no-repeat;
  height: 100vh;
  display: flex;
  justify-content: flex-end;
  align-items: center;
  padding: 20px;
}

.form-container {
  width: 100%;
  max-width: 400px;
  background: rgba(17, 0, 0, 0.3);
  padding: 30px;
  border-radius: 10px;
  box-shadow: 0 0 15px rgba(0, 0, 0, 0.2);
}
.form-container h2 {
  text-align: center;
  margin-bottom: 20px;
  color:blanchedalmond;
  font-size: 22px;
}

.form-container input,
.form-container select {
  width: 100%;
  padding: 10px;
  margin: 8px 0;
  border-radius: 5px;
  border: 1px solid #ccc;
}

.phone-group {
  display: flex;
  gap: 5px;
}

.phone-group select {
  width: 30%;
}

.phone-group input {
  width: 70%;
}

.two-cols {
  display: flex;
  gap: 10px;
}

.two-cols input {
  flex: 1;
}

.captcha {
  display: flex;
  align-items: center;
  gap: 10px;
  margin: 10px 0;
}

.captcha img {
  width: 80px;
  height: 30px;
  background: #eee;
  border-radius: 4px;
}

.checkbox {
  font-size: 12px;
  margin-top: 10px;
  color: white;
}

.checkbox label {
  display: flex;          
  align-items:center; 
  line-height: 1.4;        
}

.submit-btn {
  width: 100%;
  background: #d19a2e;
  color: white;
  padding: 12px;
  border: none;
  font-weight: bold;
  border-radius: 6px;
  margin-top: 15px;
  
}
.login-link {
  margin-top: 15px;
  font-size: 13px;
  text-align: center;
  color:white;
}

@media (max-width: 768px) {
  body {
    justify-content: center;
    padding: 10px;
  }

  .form-container {
    width: 100%;
  }
}
```
## Output:
![image](https://github.com/user-attachments/assets/44f6d0ab-ecbd-4c0a-801d-281dc20cd060)

## Result:
A landing page clone of Saveetha Engineering College’s Admission Enquiry form using HTML and CSS is designed successfully.

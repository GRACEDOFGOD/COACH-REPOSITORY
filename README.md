<!DOCTYPE html>
<html lang="en"> 
  <head>
    <meta charset="utf-8">
    <link rel="stylesheet" type="text/css" href="styles.css">
  </head>
  <body>
    <h1 id="title">SURVEY FORM | NEW FOUNDATION ACADEMY</h1>
    <p id="description" class="toptop">Thank you for helping us improve</p>

    <!-- The form id was missing a closing quote -->
    <form id="survey-form"> 
     
      <label id="name-label" for="name">
        <b class="nf">Full Name</b>
        <!-- 'for' attribute value 'name' should match input's 'name' attribute -->
        <input type="text" id="name" name="name" placeholder="Enter your name" required>
      </label>

      <label class="nf" id="email-label" for="email">
        <b>Email</b>
        <!-- The 'for' attribute should be for 'email', not 'name' -->
        <input type="email" id="email" name="email" placeholder="Enter your email" required>
      </label>

      <label class="nf" id="number-label" for="number">
        <b>Age (years)</b>
        <!-- 'name' attribute added to identify this field -->
        <input type="number" id="number" name="age" min="10" max="100" placeholder="Enter your age" required>
      </label>

      <label class="nf" for="role">
        <b>Which role best describes you?</b>
        <!-- Closing the select inside the label and fixing 'disabled' typo -->
        <select id="dropdown" name="role" required>
          <option disabled selected value>Select one option</option>
          <option value="Student">Student</option>
          <option value="Employed">Employed</option>
          <option value="Self-employed">Self-employed</option>
          <option value="Prefer not to say">Prefer not to say</option>
        </select>
      </label>

      <p class="nf">How likely are you to recommend us to a friend?</p>
      <label class="b"> 
        <input type="radio" name="recommend" value="definitely" required> Definitely
      </label>
      <label class="b"> 
        <input type="radio" name="recommend" value="Not likely" required> Not likely
      </label>
      <label class="b"> 
        <input type="radio" name="recommend" value="Not at all" required> Not at all
      </label>

      <p>What do you love about our school?</p>
      <label class="b">
        <input type="checkbox" name="love" value="Teachers"> Teachers
      </label>
      <label class="b">
        <input type="checkbox" name="love" value="Facilities"> Facilities
      </label>
      <label class="b">
        <input type="checkbox" name="love" value="Curriculum"> Curriculum
      </label>
      <label class="b">
        <input type="checkbox" name="love" value="Track record"> Track record
      </label>

      <p>Anything you want us to improve on?</p>
      <textarea id="comment" name="comment" rows="5" cols="25" placeholder="I would like the school to improve on..."></textarea>

      <!-- 'type' should be lowercase -->
      <button type="submit" id="submit">Submit</button>
    </form>
  </body>
</html>

---
layout: post
title: Pairing Application
description: Sign Up Form
nav-menu: true
tags: uot
short-title: UoT
explanation: This form is for individuals who either have an idea or are looking to join a team with an existing idea. We will send a confirmation email with more details on the next steps after receiving your application. The deadline to apply is January 25th, 2025. 
---

<div class="row">
<div class="6u 12u$(small)">
<div id="signupWrapper">
<form
  action="https://formspree.io/f/mnnqdjpj"
  method="POST"
enctype="multipart/form-data"
>
    <!-- Venture Idea Selection -->
    <div class="field">
        <label>Do you have an existing venture idea, or would you prefer to work on a team’s idea?</label><br>
        <input type="radio" id="existing_idea" name="venture_preference" value="I have an existing venture idea" required>
        <label for="existing_idea">I have an existing venture idea</label><br>
        <input type="radio" id="join_team" name="venture_preference" value="I want to join a team with an idea" required>
        <label for="join_team">I want to join a team with an idea</label>
    </div>
    <!-- Venture Idea Description -->
    <div class="field">
        <label for="venture_description">If you have a venture idea, please provide a brief description of it. (100 words min)</label>
        <textarea id="venture_description" name="venture_description" minlength="100"></textarea>
    </div>
    <!-- Full Name -->
    <div class="field">
        <label for="full_name">Full Name</label>
        <input type="text" id="full_name" name="full_name" required>
    </div>
    <!-- Email -->
    <div class="field">
        <label for="email">Email</label>
        <input type="email" id="email" name="email" required>
    </div>
    <!-- Institute of Study -->
    <div class="field">
        <label for="institute">Institute of Study</label>
        <input type="text" id="institute" name="institute" placeholder="e.g. UofT" required>
    </div>
    <!-- Program and Year of Study -->
    <div class="field">
        <label for="program_year">Program and Year of Study</label>
        <input type="text" id="program_year" name="program_year" placeholder="e.g., Psychology - 2nd year PhD" required>
    </div>
    <!-- Area of Expertise -->
    <div class="field">
        <label for="expertise">Area of Expertise</label>
        <input type="text" id="expertise" placeholder="e.g., Software Development, Marketing, Engineering" name="expertise" required>
    </div>
    <!-- Venture Interest Area -->
    <div class="field">
        <label for="venture_interest">Venture Interest Area</label>
        <input type="text" id="venture_interest" placeholder="e.g., HealthTech, EdTech, Sustainability" name="venture_interest" required>
    </div>
    <!-- Preferred Team Role -->
    <div class="field">
        <label for="team_role">Preferred Team Role</label>
        <input type="text" id="team_role" name="team_role" required>
    </div>
    <!-- Experience Level in Entrepreneurship/Venture Creation -->
    <div class="field">
        <label for="experience_level">Experience Level in Entrepreneurship/Venture Creation</label>
        <input type="text" id="experience_level" name="experience_level" required>
    </div>
    <!-- Work Style -->
    <div class="field">
        <label for="work_style">How would you describe your work style?</label>
        <textarea id="work_style" name="work_style" required></textarea>
    </div>
    <!-- Pitch Competitions -->
    <div class="field">
        <label for="pitch_competitions">Have you participated in pitch competitions before? If so, please specify the name of the competition and your results.</label>
        <textarea id="pitch_competitions" name="pitch_competitions"></textarea>
    </div>
    <!-- Why Join IOB Competition -->
    <div class="field">
        <label for="join_reason">Why do you want to join the IOB Competition?</label>
        <textarea id="join_reason" name="join_reason" required></textarea>
    </div>
    <!-- Resume Attachment -->
    <div class="field">
        <label for="resume">Optional Attachment: Resume (only PDF is supported)</label>
        <input type="file" id="resume" name="resume" accept="application/pdf">
    </div>
      <div style="padding-bottom: 30px;"> Please note: Due to high website traffic, submissions may take up to 2 minutes to process. During this time, avoid refreshing or closing your browser. Once we receive your application, you will receive a confirmation email with further details on the next steps. If you do not receive our email within two days, please contact us at innovationboard.uoft@gmail.com.
          </div>
    <!-- Submit Button -->
    <div class="fit">
        <button type="submit">Submit </button>
    </div>

</form>
</div>
</div>
</div>

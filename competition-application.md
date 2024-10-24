---
layout: post
title: Competition Application
description: Sign Up Form
nav-menu: true
explanation: Take the first step toward an exciting adventure – submit your team application today to join the Innovation OnBoard competition.
---

<div class="row">
<div class="6u 12u$(small)">
<div id="signupWrapper">
<form
  action="https://formspree.io/f/xyzyzobl"
  method="POST"
>
        <div class="field">
            <label for="fullName">Full Name:</label>
            <input type="text" id="fullName" name="fullName" required>
        </div>
        <div class="field">
            <label for="email">Email:</label>
            <input type="email" id="email" name="email" required>
        </div>
        <div class="field">
            <label for="phone">Phone Number:</label>
            <input type="tel" id="phone" name="phone">
        </div>
        <div class="field">
            <label for="program">Program and Year of Study:</label>
            <input type="text" id="program" name="program">
        </div>
        <div class="field">
            <label for="expertise">Areas of Expertise:</label>
            <input type="text" id="expertise" name="expertise">
        </div>
        <div class="field">
            <label for="skills">Primary Skills:</label>
            <input type="text" id="skills" name="skills">
        </div>
        <div class="field">
            <label for="interest">Areas of Interest for the Venture:</label>
            <input type="text" id="interest" name="interest">
        </div>
        <div class="field">
            <label for="role">Preferred Role in the Team:</label>
            <input type="text" id="role" name="role">
        </div>
        <div class="field">
            <label for="experience">Experience Level in Entrepreneurship/Venture Creation:</label>
            <select id="experience" name="experience">
                <option value="beginner">Beginner</option>
                <option value="intermediate">Intermediate</option>
                <option value="advanced">Advanced</option>
            </select>
        </div>
        <div class="field">
            <label for="previousParticipation">Have You Previously Participated in Innovation Competitions?</label>
            <select id="previousParticipation" name="previousParticipation">
                <option value="yes">Yes</option>
                <option value="no">No</option>
            </select>
            <textarea id="competitionExperience" name="competitionExperience" placeholder="If yes, briefly describe." style="display:none;"></textarea>
        </div>
        <div class="field">
            <label for="motivation">What Motivates You to Join This Competition?</label>
            <textarea id="motivation" name="motivation"></textarea>
        </div>
        <div class="field">
            <label for="availability">Availability and Commitment Level:</label>
            <input type="text" id="availability" name="availability">
        </div>
        <div class="field">
            <label for="teamSize">Preferred Team Size:</label>
            <input type="text" id="teamSize" name="teamSize">
        </div>
        <div class="field">
            <label for="workStyle">How Would You Describe Your Work Style?</label>
            <input type="text" id="workStyle" name="workStyle">
        </div>
        <div class="field">
            <label for="ventureIdea">Do You Have a Pre-existing Venture Idea or Would You Like to Work on a Team's Idea?</label>
            <select id="ventureIdea" name="ventureIdea">
                <option value="existing">Existing Idea</option>
                <option value="team">Team Idea</option>
            </select>
        </div>
        <div class="field">
            <label for="pairing">Do You Want to be Paired with Other Teammates Based on Your Preferences?</label>
            <select id="pairing" name="pairingWithOtherTeammates">
                <option value="yes">Yes</option>
                <option value="no">No</option>
            </select>
        </div>
        <button type="submit">Submit Application</button>
    </form>
</div>
</div>
</div>

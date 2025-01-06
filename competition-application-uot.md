---
layout: post
title: Team Application
description: Sign Up Form
nav-menu: true
explanation: |
 Submit your team application today to join the Innovation OnBoard Competition! If your team requires additional talents, you are welcome to request extra members. Each team must include at least one current University of Toronto student or an alumnus who graduated in 2022 or later. You can update your team details, such as adding new members, anytime before the application deadline by contacting us. 
---
<div class="row">
    <div class="6u 12u$(small)">
        <div id="signupWrapper">
            <form
              action="https://formspree.io/f/mkgnrool"
              method="POST"
            >
                <div class="field">
                    <label for="teamname">Team Name</label>
                    <input type="text" id="teamname" name="teamname" required>
                </div>
                <div class="field">
                    <label for="problem">What problem are you solving?</label>
                    <textarea id="problem" name="problem" placeholder="Please describe the specific problem or challenge your startup idea aims to address." required></textarea>
                </div>
                <div class="field">
                    <label for="solution">What is your solution?</label>
                    <textarea id="solution" name="solution" placeholder="Please articulate your startup's innovative solution to the problem identified earlier." required></textarea>
                </div>
                 <!-- Venture Idea Selection -->
                <div class="field">
                    <label>Would you like additional members to join your team?</label><br>
                    <input type="radio" id="need_members" name="additional_members" value="Yes, we need additional member(s)" required>
                    <label for="need_members">Yes, we need additional member(s)</label><br>
                    <input type="radio" id="open_for_members" name="additional_members" value="Team is complete, but we are open to more members" required>
                    <label for="open_for_members">Our team is complete, but we are open to more members</label>
                    <input type="radio" id="no_members" name="additional_members" value="We do not wish to add more member" required>
                    <label for="no_members">Our team is complete, and we do not wish to add more members</label>
                </div>
                <div class="field">
                    <label for="need_member_explanation">If you would like an additional team member, please describe your ideal candidate(s). </label>
                    <textarea id="need_member_explanation" name="need_member_explanation" placeholder="Please be as specific as possible to help us find the perfect match"></textarea>
                </div>
                <div class="field">
                    <label for="additional">Anything you want to add?</label>
                    <textarea id="additional" name="additional" placeholder="You can include any other information here."></textarea>
                </div>
                <div id="teamMembersContainer">
                    <div class="field">
                        <label for="name-0">Team Member Name:</label>
                        <input type="text" id="name-0" name="teamMember-1[]" required>
                    </div>
                    <div class="field">
                        <label for="email">Team Member Email:</label>
                        <input type="email" id="email" name="teamMember-1[]" required>
                    </div>
                    <div class="field">
                        <label for="name-1">Team Member Program of Study:</label>
                        <input type="text" id="name-1" name="teamMember-1[]" placeholder="e.g. Psychology" required>
                    </div>
                    <div class="field">
                        <label for="name-1">Team Member Degree:</label>
                        <input type="text" id="name-1" name="teamMember-1[]" placeholder="e.g., PhD, MSc, BSc" required>
                    </div>
                    <div class="field">
                        <label for="name-1">Team Member Year of Study:</label>
                        <input type="text" id="name-1" name="teamMember-1[]" placeholder="e.g. 2nd year" required>
                    </div>
                    <div style="padding-bottom: 30px;"> Please note: Due to high website traffic, submissions may take up to 2 minutes to process. During this time, avoid refreshing or closing your browser. Once we receive your application, you will receive a confirmation email with further details on the next steps. If you do not receive our email within two days, please contact us at innovationboard.uoft@gmail.com.</div>
                </div>
                    <button type="button" onclick="addTeamMember()">Add Team Member</button>
                    <button type="submit">Submit Application</button>
            </form>
        </div>
    </div>
</div>

<script>
let memberCount = 2;

    function addTeamMember() {
      const container = document.getElementById("teamMembersContainer");
      // Add Member Name 
      const newMemberName = document.createElement("div");
      newMemberName.className = "field";
      newMemberName.innerHTML = `
        <label for="name-${memberCount}">Team Member ${memberCount} Name:</label>
        <input type="text" id="name-${memberCount}" name="teamMember-${memberCount}[]" required>
      `;
      container.appendChild(newMemberName);

      // Add member email
      const newMemberEmail = document.createElement("div");
      newMemberEmail.className = "field";
      newMemberEmail.innerHTML = `
        <label for="name-${memberCount}">Team Member ${memberCount} Email:</label>
        <input type="email" id="name-${memberCount}" name="teamMember-${memberCount}[]" required>
      `;
      container.appendChild(newMemberEmail);

      // Add Program 
      const newMemberProgram = document.createElement("div");
      newMemberProgram.className = "field";
      newMemberProgram.innerHTML = `
        <label for="name-${memberCount}">Team Member ${memberCount} Program of Study:</label>
        <input type="text" id="name-${memberCount}" name="teamMember-${memberCount}[]" placeholder="Math" required>
      `;
      container.appendChild(newMemberProgram);

      // Add Degree
      const newMemberDegree = document.createElement("div");
      newMemberDegree.className = "field";
      newMemberDegree.innerHTML = `
        <label for="name-${memberCount}">Team Member ${memberCount} Degree:</label>
        <input type="text" id="name-${memberCount}" name="teamMember-${memberCount}[]" placeholder="PhD" required>
      `;
      container.appendChild(newMemberDegree);

      // Add Year
      const newMemberYear = document.createElement("div");
      newMemberYear.className = "field";
      newMemberYear.innerHTML = `
        <label for="name-${memberCount}">Team Member ${memberCount} Year of Study:</label>
        <input type="text" id="name-${memberCount}" name="teamMember-${memberCount}[]" placeholder="2nd year" required>
      `;
      container.appendChild(newMemberYear);

      memberCount++;
    }
</script>

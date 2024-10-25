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
          action="https://formspree.io/f/xrbgbdrv"
          method="POST"
        >
                <div id="teamMembersContainer">
                  <div class="field">
                    <label for="name-0">Name Team Member 1:</label>
                    <input type="text" id="name-0" name="teamMemberNames[]" required>
                  </div>
                </div>
                <div class="field">
                    <label for="email">Email:</label>
                    <input type="email" id="email" name="email" required>
                </div>
                <div class="field">
                    <label for="phone">Phone Number:</label>
                    <input type="tel" id="phone" name="phone">
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
      const newMember = document.createElement("div");
      newMember.className = "field";
      newMember.innerHTML = `
        <label for="name-${memberCount}">Name Team Member ${memberCount}:</label>
        <input type="text" id="name-${memberCount}" name="teamMemberNames[]" required>
      `;
      container.appendChild(newMember);
      memberCount++;
    }
</script>

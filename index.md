---
layout: default
title: "Declaration of the Free States"
---

<link rel="stylesheet" href="{{ '/assets/style.css' | relative_url }}">

<div class="declaration-wrap">

<div class="title-block">
  <div class="document-kicker">A Statement of Causes and Resolve</div>
  <h1>Declaration of the Free States</h1>
  <div class="document-version">Version 1.0 — 12 March 2026</div>
</div>

<hr class="rule">

<p class="lead">
The Declaration of the Free States sets forth the causes which compel a Free People to name and resist the rise of tyranny, and to restore constitutional government.
</p>


<hr class="rule">

<h2>The Declaration</h2>

<p>
<a href="{{ '/declaration.html' | relative_url }}">Full Text</a><br>
<a href="{{ '/declaration.pdf' | relative_url }}">Download PDF</a>
</p>

<hr class="rule">


<h2>Signatories</h2>

<p>
Governors, Attorneys General, Secretaries of State, and other constitutional officers of the several States are invited to declare their public support for the principles set forth in this Declaration. Public declarations of support are recorded as part of the historical record of this Declaration.
</p>

<p>
<a href="{{ '/state_officers.html' | relative_url }}">State Officers</a><br>
<a href="{{ '/signatories.html' | relative_url }}">Public Signatories</a>
</p>

<hr class="rule">

<hr class="rule">

<h2>Support</h2>

<p class="lead">
If you support the principles of this Declaration, you may register that support here.
</p>

<div style="text-align:center;">
  <a
    href="#"
    id="support-button"
    class="support-button plausible-event-name=Support+Declaration"
    onclick="return false;">
    Support this Declaration
  </a>
</div>

<p id="support-message" style="text-align:center; margin-top: 0.75rem;"></p>

<script>
document.addEventListener("DOMContentLoaded", function () {
  const button = document.getElementById("support-button");
  const message = document.getElementById("support-message");
  const key = "declaration_support_registered";

  if (localStorage.getItem(key) === "yes") {
    button.textContent = "Support Registered";
    button.setAttribute("aria-disabled", "true");
    button.style.pointerEvents = "none";
    message.textContent = "Your support has been recorded on this device.";
  }

  button.addEventListener("click", function () {
    localStorage.setItem(key, "yes");
    button.textContent = "Support Registered";
    button.setAttribute("aria-disabled", "true");
    button.style.pointerEvents = "none";
    message.textContent = "Your support has been recorded on this device.";
  });
});
</script>


<div class="closing-block">
  <p>
  Published for the judgment of history.
  </p>
</div>

</div>



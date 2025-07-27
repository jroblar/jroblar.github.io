---
layout: null
permalink: /cv/
title: cv
nav: true
nav_order: 5
cv_pdf: /assets/pdf/juanrobledo_resume_v5.pdf  # Path to your CV
description: This is a description of the page.
redirect_from:
  - /cv
---

<p>Opening CV in a new tab...  
If nothing happens, <a href="{{ page.cv_pdf }}" target="_blank" rel="noopener noreferrer">click here to view it</a>.</p>

<script>
  // Try opening the CV in a new tab
  var win = window.open("{{ page.cv_pdf }}", "_blank");

  // If the popup is blocked, fallback message is visible
  if (!win || win.closed || typeof win.closed === "undefined") {
    console.warn("Popup blocked. Showing fallback link.");
  } else {
    // Redirect the current tab back to the homepage
    window.location.href = "/";
  }
</script>

---
title: "Modal form"
linkTitle: "Modal form"
date: 2017-01-05
description: >
  Just do a button.
hide_feedback: true
---


<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@sheerid/jslib@1/sheerid.css" type="text/css"/>
<script src="https://cdn.jsdelivr.net/npm/@sheerid/jslib@1/sheerid.js"></script>
<button onclick="displayVerification()">Confirm Eligibility</button>
<script>
  function displayVerification() {
    const verificationUrl = 'https://services.sheerid.com/verify/62856b5af125ee46cfd7a1b2/';
    sheerId.loadInModal(
        verificationUrl, {
        mobileRedirect: true
      });
  };
</script>
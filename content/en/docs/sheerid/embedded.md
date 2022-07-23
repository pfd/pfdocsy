---
title: "Embedded form"
linkTitle: "Embedded form"
date: 2017-01-05
description: >
  Just do a button.
hide_feedback: true
---

<script src="https://cdn.jsdelivr.net/npm/@sheerid/jslib@1.102.1/sheerid.js" integrity="sha256-4twAwy76jZ/IrDsAdvdIJL8AhLgp0ykGeT1ztEfb7Ks=" crossorigin="anonymous"></script>

<div id="my-container"></div>
<script>
  sheerId.loadInlineIframe(
    document.getElementById('my-container'),
    'https://services.sheerid.com/verify/62856b5af125ee46cfd7a1b2/',
  );
</script>

<a class="cool" onclick="displayVerification()">Get that discount</a>
<script>
  function displayVerification() {
    sheerId.loadInModal(
      'https://services.sheerid.com/verify/62856b5af125ee46cfd7a1b2/', {
        mobileRedirect: false,
      });
  }
</script>
---
layout: default
title: Donate
permalink: /donate/
---
<h1>{{ page.title }}</h1>


<div style="padding-top:30px; width: 100%; text-align:center">

<form action="https://www.paypal.com/cgi-bin/webscr" method="post" target="_blank">
  <input type="hidden" name="cmd" value="_donations">
  <input type="hidden" name="business" value="payments@hobartmakers.com">
  <input type="hidden" name="lc" value="AU">
  <input type="hidden" name="item_name" value="Hobart Makers Inc.">
  <input type="hidden" name="currency_code" value="AUD">
  <input type="hidden" name="bn" value="PP-DonationsBF:btn_donateCC_LG.gif:NonHosted">
  <input type="submit" class="btn btn-primary btn-lg" value="Make a Donation"/>
</form>

</div>

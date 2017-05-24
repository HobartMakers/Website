---
title: "Subscribe to Hobart Hackerspace"
layout: "page"
permalink: "/subscribe/"
---

We'd love to have you join us :-) Subscribing to the Hobart Hackerspace is great value, and you get many benefits, such as:

* 24/7 Access to the hackerspace
* Discounted $1 sausages (non-member price $2.50)
* Discount at Jaycar

If you are a new member, you will be contacted via. email and receive a new RFID tag for free when we next see you at the space. You'll be able to swipe this tag on the access controller at the rear of the building and you will be let in, as long as your subscription is current!

If you are an existing or previous member, you may enter your RFID tag number below, and it will be re-enabled. It is engraved on the back of your tag. If you don't know what your tag number is, please <a href="{{ "/contact/" | relative_url }}">contact us</a> and we can look it up for you.

<div class="row">
    <div class="col-xs-4">

        <form action="https://www.paypal.com/cgi-bin/webscr" method="post" target="_top">

        <input type="hidden" name="cmd" value="_s-xclick" />
        <input type="hidden" name="hosted_button_id" value="N2TU8HM7CQ4AA" />


        <div class="form-group">
            <input type="hidden" name="on1" value="Your Tag Number" />
            <label for="os1">RFID Tag Number</label>
            <input type="text" class="form-control" name="os1" id="os1" maxlength="20" />
        </div>

        <p>
        <input type="hidden" name="on0" value="" />
        <input type="radio" name="os0" value="Full" checked="checked" /> Full $32.50/month<br />
        <input type="radio" name="os0" value="Concession" /> Concession $22.50/month 
        </p>


        <input type="hidden" name="currency_code" value="AUD" />

        <input class="btn btn-primary" type="submit" value="Subscribe via. PayPal Subscription" />

        </form>
    </div>
</div>

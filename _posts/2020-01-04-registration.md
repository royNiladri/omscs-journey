---
title: "Registration"
layout: post
permalink: "registration"
---
Boy was that stressful! As most of you would be aware that we new students have only the second phase to register. We got the time tickets on January 2nd and had a registration start time of 11 am ET on January 3rd. I was aware of the rush and had been checking up the available slots on oscar and Reddit. I wanted to get into GIOS and had as backup HCI and HPCA.

When the final moment of truth arrived, years of clicking and tabbing came to the rescue. Just before the registration started, GIOS had ~65 available spots. Click, click, click and my heart skipped a beat when I saw the table row, `**Registered (Web) on Jan 03, 2020`. I probably did my registration in under 30 seconds. I went back to check the status after 5 minutes, and waitlist number had crossed 75! Quite literally, "Every second counts".

As for payments, there are multiple options. I used Credit Card (because it's the simplest and happens immediately). Another popular option is the Flywire. On the official site I read, it might take up to 7 days for the payment to get processed and so did not seem like a feasible option for most people in their first term. Here is the breakdown of what I paid using Credit Card for one paper:

Transaction Component | USD (&#36;) | INR (&#8377;)
:--|--:|--:
Tuition Fees | 841.00| 59,978.44
PayPath Service Fees (2.85%) | 23.97 | 1,709.49
Currency Markup Fee | NA | 1,243.15
**TOTAL** | **864.97** | **62,931.08**

Classes are supposed to start from **January 6th (Monday)**. Eagerly waiting for the next updates.

# Fees by Semester
Please note Flywire usually takes 7-8 working days to complete the transaction from the day payment is initiated by the student.

<table>
    <tr>
        <th>Semester</th>
        <th>Courses taken</th>
        <th>Payment Mode</th>
        <th>Fees (&#36;)</th>
        <th>Fees (&#8377;)</th>
    </tr>
    {% for payment in site.data.payments %}
    <tr>
        <td>{{payment.term}}</td>
        <td>{{payment.subjects}}</td>
        <td>{{payment.mode}}</td>
        <td>{{payment.amount_usd}}</td>
        <td>{{payment.amount_inr}}</td>
    </tr>
    {% endfor %}  
</table>
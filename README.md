# Task2_cyberSecurity_internship
# Phishing Email Analysis Task – Cybersecurity Internship
<!--
Hi everyone,  
This is my submission for the phishing email analysis task given as part of the cybersecurity internship. I completed the task step by step and explained here in a simple way what I did, how I did it, and what I found during the investigation. I have also shared supporting screenshots and the sample phishing email I used.

---

What was the task about?

The goal of the task was to analyse a real phishing email. I had to check the email header, verify the sender, look for spoofing or fake links, detect emotional or urgent language in the content, and finally summarise the phishing indicators. I have try explained everything

---

Step 1 – Choosing the phishing email

I selected a phishing email from a public GitHub repository. It looked like a solar panel offer email in Dutch, but the sender domain and content seemed suspicious. This email was used as my main sample for the analysis. I have shared the original email file as part of this repository.

What grabbed my attention in this email was how professionally it was designed — it looked like a real solar energy company offering discounts. But once I checked the sender's domain (serenitepure.fr) and saw that the reply-to was a completely unrelated domain (aichakandisha.com), it felt fishy. The message kept repeating things like “Don’t wait” and “Click here for free offers”, which triggered a red flag for emotional manipulation. Also, when I read the technical headers, none of the security checks like SPF, DKIM, or DMARC were passed. This mismatch between visual trust and technical failure helped me understand how phishing works — it’s not just about how an email looks, but also what's hiding behind it.

---

Step 2 – Email header analysis

To analyse the email header, I copied the raw email content and used Google Admin Toolbox (message header analyser tool).  
Using this tool, I found that:

- The sender was using an unknown domain which doesn’t match the identity they claimed.
- There was no SPF, DKIM, or DMARC verification in place.
- The email passed through multiple servers, which adds to the suspicion.

I have shared a screenshot of this analysis from the toolbox, where these results are clearly visible.

---

Step 3 – Analysing the email content

After checking the header, I manually reviewed the email content. It contained an urgent message saying things like "Don’t wait", "Click here", and highlighted rising energy bills and inflation. These are emotional triggers used in social engineering. The button in the email leads to an unknown link, and the domain doesn't match the organisation the sender claims to represent. There were no contact details or official company signatures either.

I have shared a screenshot of the email content that clearly shows these patterns.

I also hovered my mouse over the link in the email to check if the destination was matching. I captured a screenshot while hovering, where the suspicious link can be seen clearly.

To go one step further, I scanned the link or domain using VirusTotal and shared the screenshot showing whether it was flagged as suspicious or safe so its a sample so obiously its safe but gain info on relationship an other details.

---

What I learned from this task

- I learned how phishing emails try to manipulate users emotionally by showing fake urgency or attractive offers.
- I understood how to read and analyse email headers to check sender authenticity.
- I saw how attackers use spoofed domains and unverified headers to bypass email filters.
- I practiced real phishing detection methods that can help in cyber awareness and security operations.

---

Tools I used

- GitHub (for phishing sample)
- Google Admin Toolbox (for header analysis)
- VirusTotal (for link scanning)
- Screenshot tool and basic browser tools
- My own observations and understanding



That’s all from my side for this task. I really enjoyed doing this and learned practical things that will help me in the cybersecurity field. Thank you so much for reviewing my work.



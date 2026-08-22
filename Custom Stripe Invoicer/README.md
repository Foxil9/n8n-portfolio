# Project Summary — Stripe

**The problem:** Stripe payments aren’t automatically accessible to every staff member and customer support, and that can be problematic when someone needs to check a payment for further evaluation or to check any data.

**The solution I provide:** This workflow allows the staff and anyone given access to the Google Spreadsheet to get access to specific customers when needed. That info includes name, email, order id, total amount paid and more. It notifies staff on error and sends a confirmation email

**The Logic Behind:** I use a stripe trigger to execute the workflow for each payment and then check for fail/success (A Notifier is provided in case of Unexpected Outcome; No necessarily failure). Then I grab the order details using an HTTP request and add the information to a google spreadsheet and send a confirmation email using the company’s official transactions email 

**What I learned from this project:** I learned that notifying on error is necessary for things like transaction management. I also learned that using the solution that works even if it’s simple and easy to apply. 

Try it Yourself! All workflows can be accessed in my github page.

You'll need to set up any missing credentials for this to work. If self-hosting, the instance needs a public IP/URL. n8n Cloud works out of the box with no hosting required.”

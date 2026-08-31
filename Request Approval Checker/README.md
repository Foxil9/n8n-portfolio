# Project Summary — Request Checker

!Screenshot From 2026-08-31 09-43-17-modified.png

**The problem:** Requests that need approval from more than one person often get lost in email threads, forgotten, or approved out of order with no clear record of who signed off and when.

**The solution I provide:** An automated two-level approval system that checks for approval from two people and routes the request accordingly. It notifies on error, and it checks the first person's approval before the second, disapproving immediately if the first rejects it, to save resources.

**The Logic Behind:** The workflow triggers on a new request and sends it to the first approver. If they reject it, the workflow stops immediately and the request is marked disapproved, no need to bother the second approver. If they approve, the request moves to the second approver, and the final outcome is recorded based on their decision. A cleanup step runs after each response to prevent stale or duplicate entries from corrupting the request's status.

**What I learned from this project:** I learned how to design workflows around early-exit logic instead of checking every condition regardless of outcome. I also learned how important cleanup steps are for data integrity when a workflow can be triggered multiple times for the same request.

Try it Yourself! All workflows can be accessed in my GitHub page.

You'll need to set up any missing credentials for this to work. If self-hosting, the instance needs a public IP/URL. n8n Cloud works out of the box with no hosting required.

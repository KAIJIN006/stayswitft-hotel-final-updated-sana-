StaySwift Hotel Reservation System

Run locally:
  py -m venv .venv
  .venv\\Scripts\\activate
  pip install -r requirements.txt
  python app.py

For Render:
  Build command: pip install -r requirements.txt
  Start command: gunicorn app:app
  Root Directory: set to the folder containing app.py and requirements.txt.

Email notifications:
Set SMTP_HOST, SMTP_PORT (usually 587), SMTP_USER, SMTP_PASSWORD, SMTP_FROM,
and SECRET_KEY in your hosting environment. For Gmail, use a Google App Password,
not your normal Gmail password.

When a room opens, matching waiting-list guests receive an email with a
Review & Confirm Booking button. Opening the link only displays the offer.
The booking is created under the waiting-list user's account only after they
press Confirm Booking. The first successful confirmation wins. Existing
waiting-list dates (check-in/check-out) are used for the reservation.

This is a school-project prototype, not production-ready software.

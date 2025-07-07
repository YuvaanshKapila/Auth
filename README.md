This is a Python project that uses your face to log you in. It checks your face using the webcam and compares it to saved photos of people who are allowed.

No passwords. Just your face.

What It Does
Uses your webcam to scan your face

Compares it to saved face photos

If it matches, it lets you in

If not, it says authentication failed

What You Need
Python 3.7 or higher

A webcam

These Python libraries:

bash
Copy
Edit
pip install face_recognition opencv-python
Folder Setup
Copy
Edit
biometric_auth/
├── auth.py
├── user_photos/
│   └── your_name.jpg
Put your face photo (like john.jpg) inside the user_photos/ folder. The file name (without .jpg) becomes the person's name.

How to Run
Open terminal or command prompt in the project folder

Run the script:

bash
Copy
Edit
python auth.py
Look into the webcam

If your face matches a photo inside user_photos/, it will say:

csharp
Copy
Edit
[SUCCESS] Welcome, your_name!
Press q to quit any time

How to Add a User
Take a clear photo of the person’s face

Save it in the user_photos/ folder

Make sure the face is facing forward and not blurry

Run the program. Now they are part of the system

How It Works
It loads face data from saved images

Then captures your live face from the webcam

Compares both using facial measurements

If the faces are similar, you are authenticated

Future Ideas
Add fingerprint or voice login

Add a log file to record login attempts

Make a GUI (window-based app)

Add a "register user" option using the webcam

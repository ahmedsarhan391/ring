Simple To-Do App (iPhone)
=========================

A small Arabic to-do list that runs in Safari on iPhone. It is a single
`index.html` file with no dependencies. Tasks are saved on the phone
(localStorage), so they stay after you close the app.

Features
--------

- Add a task
- Tap the circle to mark a task done (tap again to undo)
- Tap `×` to delete a task
- Delete all completed tasks at once
- Dark mode follows the iPhone setting

Run it on your iPhone
---------------------

iPhone apps normally need a Mac and Xcode. This app avoids that: it is a
web page you add to your Home Screen.

1. Put the folder on a web server. Two easy options:
   - **On the same Wi-Fi as your iPhone:** from this folder on a computer run
     `python3 -m http.server 8000`, then find the computer's local IP
     (for example `192.168.1.20`).
   - **Online:** upload `index.html` to any static host (GitHub Pages, Netlify, ...).
2. On the iPhone, open Safari and go to `http://<computer-ip>:8000/` (or the online address).
3. Tap the Share button, then **Add to Home Screen**.
4. Open **مهامي** from the Home Screen. It opens full screen without the Safari bar.

Test
----

The app was tested in Chromium with an iPhone 14 screen size (390 x 844, touch enabled):
adding, completing, deleting, clearing completed tasks, saving across reloads,
safe HTML in task text, and the absence of horizontal scrolling.

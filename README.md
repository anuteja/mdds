# MDDS
# Musical Dart Defense System
### USB dart launcher with face recognition targeting. Also Spotify

# First Component
Facial Detection and Recognition Features: Spotify integration for recognized users, and dart barrage for strangers The software was first trained to detect the faces of team members by capturing a series of photos at varying angles and distance. The algorithm used to detect faces was Haar Wavelet Classifier, and the algorithm for recognizing faces in the database was EigenFaces.

# Second Component 
Launcher Targeting System Features: Targeting by absolute angle, Interruptable actions The launcher we used had no official drivers for Linux, but we were able to find a low-level library that someone made.. Unfortunately, it only allowed relative targeting; there is no way for the hardware to detect which way it is aiming. Part of our project was engineering a wrapper library to keep track of the launcher's angles. The launcher rotates at a constant speed, so it was easy to calculate how far it moved as long as we always kept track of how long it was moving. This library may be potentially useful for anyone who wants to script a Dream Cheeky USB Missile Launcher.

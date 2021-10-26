## Steps to reproduce the error

1. Open the project in Android Studio using the command `npx cap open android`.
2. Run it on an Android device using a USB cable. The device needs to have the Developer Options menu enabled: https://www.samsung.com/uk/support/mobile-devices/how-do-i-turn-on-the-developer-options-menu-on-my-samsung-galaxy-device/. From the Developer Options menu USB-Debugging should also be enabled.
3. When the app is opened it might need you to allow it to use the device's camera.
4. Go to `chrome://inspect/#devices` in Google Chrome. You should be able to see your connected device there. Click on `inspect` in order to be able to debug the app with Google DevTools. Open up the console.
5. In the Capacitor App click the button `Take Photo` and from the below options choose `Take Picture`. Don't actually take a picture.
6. Observe what is going on in the console after pressing the `back` button of the device.
7. There is an error message `User cancelled photos app`.

# parkrun Barcode for Mi Band

You can now have your **parkrun barcode** right on your watch!

There are **2 ways** to do this:  
- **Watchface Style** – the barcode is on your watch face  
- **App Style** – the barcode is an app you open on your watch  

## Requirements

- Windows PC  
- Android device (Temporary for installation. iOS users can use iPhone again afterwards.)

***Be sure to [download all files in releases](https://github.com/marcusoffline/parkrun-Mi-Band-10/releases/download/parkrun-for-Mi-Band-1.0.3/parkrun-for-Mi-Band-1.0.3.zip), and let's get started!***

---

## Step 1 - Making Your Barcode Image

1. Open `Barcode Image Creator.html`  
2. Enter your parkrun ID  
3. Click **Generate**, then **Save** → you now have `image.png`  

---

## Step 2 - Watchface Style
*Skip to next section if you are creating App Style*

1. Copy `image.png` to `Watchface/images/`  
   - Replace the old file  
   - Make sure the file name is `image.png`  
2. Install Mi Create: [https://github.com/ooflet/Mi-Create](https://github.com/ooflet/Mi-Create)  
3. Open Mi Create → **Open Project** → select `Watchface/parkrun.fprj`  
4. Click **Build**  
5. Go to the output folder  
6. Rename:  
   - `parkrun.face` → `parkrun.bin`  
   - Delete `parkrun.info`  

*You now have your Watchface file!*

---

## Step 2 - App Style

1. Copy `image.png` to `App/src/images/`  
   - Replace the old file  
   - Make sure the file name is `image.png`  
2. Install Node.js (Windows Installer `.msi`): [https://nodejs.org](https://nodejs.org)  
3. Open Command Prompt and type: `npm install -g aiot-toolkit`
4. In the App folder, run **Build App**  
5. Open the `dist` folder  

*If you see a `.rpk` file → you now have your App file!*

---

## Step 3 - Install on Your Watch

1. Copy the Watchface (`.bin`) or App (`.rpk`) to your Android device (USB, cloud, or whatever works)  
2. Pair your Mi Band 10 if not already paired  
   - On your Mi Band: **Settings → System → Connect new phone**  
3. Install **Notify for Xiaomi** from Google Play Store (or `.apk` file from [https://mibandnotify.com/downloads/](https://mibandnotify.com/downloads/))  
4. Open Notify for Xiaomi → **Sign in**  
5. In Notify for Xiaomi, select: **Device → Update Firmware → Third-party App or Watchface**  
6. Select your parkrun file  

**Your parkrun barcode is now on your watch!**  

*Make sure to sync it back through the Mi Fitness app.*

***iOS users:** You can re-pair the device to your iPhone.*

<h1>Step 1: </h1> </br>
Download and Install Termux<br>
Apk from f-droid </br>
https://f-droid.org/it/packages/com.termux/ </br>
or Official PlayStore</br>
https://play.google.com/store/apps/details?id=com.termux

<h1>Step 2: Install required packages </h1> </br>
pkg upgrade -y </br>
curl -LO https://its-pointless.github.io/setup-pointless-repo.sh </br>
bash setup-pointless-repo.sh </br>
pkg install android-tools python build-essential cmake libjpeg-turbo libpng libxml2 libxslt freetype git -y </br>
pip install wheel </br>
<h1>Step 3: Install instagramBot</h1> </br>
<h3></h3>This procedure is slow, use -vvv in pip if you want to see if everything installing alright</h3></br>

git clone https://github.com/Danny-1201/instagramBot.git</br>
cd instagramBot </br>
pip install -r requirements.txt </br>

<h1>Step 4: Run </h1> </br>
python -m uiautomator2 init </br>
python run.py </br>

<h1>-How can I access termux files?</h1> </br>
Read that article https://wiki.termux.com/wiki/Internal_and_external_storage </br>

-The easiest solution is to download an storage access framework compatible file manager like FX File Explorer Then you can follow that instructions https://wiki.termux.com/images/e/e5/FX_Termux_Home.jpg Then you can edit and view GramAddict files.
</br>
<h1>Troubleshooting</h1></br>
if you type on termux adb devices and you get a blank list try the following:</br>
connect the phone to a PC and get sure you get your device ID in adb devices (from pc console) </br>
adb tcpip 5555 </br>
adb kill-server and disconnect the cable </br>
get back on termux and write: adb connect localhost:5555 </br>
now you should be able to see your device ID in adb devices </br>
when I start the bot it looks like it freezes after opening IG and termux shell has been closed </br>
edit your accounts/yourusername/config.yml file and set close-apps: false </br>
All credits to patbengr </br>

<h1 style="color:Tomato;">It looks as much human as possible</h1>
<h1>Hi Carlos</h1></br>
  <h3>please follow these 4 steps to run instagram bot!</h3>
</h1>
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

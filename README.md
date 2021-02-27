ZE Delivery - API automation with Ruby/Airborne and Mobile(Android) Automation with Appium and Cucumber


Use virtual device if possible at Android Studio 
If not please use a android device without the app installed

Run automated API tests with report
Go to project folder ./ze_delivery and run :
  .rspec --pattern api/*_spec.rb --format html --out api.html



        Installing Enviroment Mac OS

1. Install Homebrew:
   /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

2. Install JDK for Mac:
   http://www.oracle.com/technetwork/java/javase/downloads/index.html

3. Instaling and seting rbenv:
   brew install rbenv
   echo 'eval "$(rbenv init -)"' >> ~/.bash_profile
   rbenv install -l
   rbenv install 2.3.1 #Ou versão superior estável
   rbenv local 2.3.1

4. Install Android Studio - It will install all other necessary dependencies like Sdk,Platform Tools,ADB
   https://developer.android.com/studio/index.html?hl=pt-br

5. Install Appium Client
   http://appium.io/ => Clique em download e baixe a versão mais recente para o seu SO

         JAVA Enviroment Variables

open your ~/.bash_profile or ~/.zshrc_profile

         Set and Save :

export JAVA_HOME=$(/usr/libexec/java_home)
export PATH=$JAVA_HOME/bin:$PA


        ANDROID Enviroment Variables

open your ~/.bash_profile or ~/.zshrc_profile

        Set and Save:

export ANDROID_HOME=/Users/<user>/Library/Android/sdk
export PATH=$ANDROID_HOME/tools/bin:$PATH
export PATH=$ANDROID_HOME/tools:$PATH
export PATH=$ANDROID_HOME/platform-tools:$PATH
export PATH=$ANDROID_HOME/platform-tools/adb:$PATH
export PATH=$ANDROID_HOME/emulator/:$PATH

        # <user> change to your user


        Installing Gems from Ruby on your terminal:
gem install bundle


        Project Exec:

a)Git clone: https://github.com/morlfm/ze_Delivery
b)Go to the ???? folder on yout terminal and do :
    bundle
c)Use virtual device if possible at Android Studio to not break automation with you already had it installed may crash the test , If not please use a android device without the app installed
d)Open Appium server and start server
e)On terminal to start test with report do :

    cucumber -p report


Run automated API tests with report
  Go to project folder ./ze_delivery and run :
      .rspec --pattern api/*_spec.rb --format html --out api.html

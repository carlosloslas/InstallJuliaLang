#InstallJuliaLang#
Install guide for JuliaLang

##Intro##
I had some truble trying to install Julia from the pulled stuff from the GitHub repository. So Once I have managed to build the language succeed in building it, I thought the best thing would be to share it with everybody so that the info can help others.
######Note######
I share this info with the best of intentions in order to help other people, but I am no expert, so use the guide to your own risk. Any issues or suggestions are welcome and I will do my best to  answer and acomodate them, but I my knowledge is limited.
##Steps##
1. Clone the Julia repository to your home directory.

 Open a terminal in your home directory and type:
 ```
 git clone git://github.com/JuliaLang/julia.git
 ```
2. Install Homebrew. 
 On the same terminal in your home directory type:
  ```
 ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
  ```
  In order to check the installation of homebrew:
	```
	brew doctor
 ```
 For more info on Homebrew their website is full of info: www.brew.sh
 
 And their documentation is very good: https://git.io/brew-docs

3. Install Julia with homebrew.

 In the terminal on your home directory:
 ```
 cd julia
 ```
 Checkout the latest stable version, currently v0.3.6:
 ```
 git checkout v0.3.8
 ```
 And to finally build Julia:
 ```
 brew update
 brew tap staticfloat/julia
 brew install julia
 ```
 
4. Check the homebrew build:
 ```
 /usr/local/Cellar/julia/0.3.6_1/bin/julia -e "Base.runtests()"
 ```
5. Run Julia !!!

 On a terminal window in your home directory:
 ```
 julia
 ```
 If evrything works you should get:
 ```
                _
   _       _ _(_)_     |  A fresh approach to technical computing
  (_)     | (_) (_)    |  Documentation: http://docs.julialang.org
   _ _   _| |_  __ _   |  Type "help()" for help.
  | | | | | | |/ _` |  |
  | | |_| | | | (_| |  |  Version 0.3.6 (2015-02-17 22:12 UTC)
 _/ |\__'_|_|_|\__'_|  |  
|__/                   |  x86_64-apple-darwin14.0.0
```
(but nicelly written, I can't seem to make it work...)

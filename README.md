# Lazyshot
Simplest way to take automated screenshot of given URLs. Easy installation!

![LAZYSHOT](https://image.ibb.co/iMLdFc/Group_2.png)



### Requirements:
* Python >= 2.7
* Selenium, urlparse and termcolor Python library. Please install latest by running these commands.
```
pip install selenium
pip install urlparse
pip install termcolor
```

### Installation:
Follow these steps to install the Lazyshot.
* Clone the project using command an any directory you want
```
git clone https://github.com/mdhama/lazyshot.git
```
* Go to /lazyshot
```
cd lazyshot
```
* Download chromedriver from [here](https://chromedriver.storage.googleapis.com/index.html?path=2.9/)
* Extract zip file. Copy and paste `chromedriver` to `/path/to/lazyshot/` directory
* Give the execute permission to chormedriver
```
chmod 755 chromedriver
```
* Add alias `chromedriver` into .bash_profile
```
nano ~/.bash_profile

or

vi ~/.bash_profile
```
* Append below line into .bash_profile
```
alias chromedriver="~/path/to/lazyshot/chromedriver"
```
* Save and exit. Now refresh .bash_profile 
```
source ~/.bash_profile
```

Done!


### How to use:

To take screenshots simply run this command 
```
python lazyshot.py wordlist
```

Screenshots will be save into Default `outputs` folder. You can pass the custom folder name using 
```
python lazyshot.py wordlist --out folder_name
```

### Wordlist:
Wordlist is just a simple data file where each line contains one URL.

File name `wordlst` or `wordlist.txt`

```
www.example.com
https://foo.example.com
http://bar.expample.com
foo-bar.exmaple.com
```

### Example:
```
python lazyshot.py wordlist.txt --out exmaple

output:

 _                     __ __ _           _
| |                   /  ___| |         | |   
| |     __ _ _____   _\ `--.| |__   ___ | |_  
| |    / _` |_  / | | |`--. \ '_ \ / _ \| __| 
| |___| (_| |/ /| |_| /\__/ / | | | (_) | |_  
\_____/\__,_/___|\__, \____/|_| |_|\___/ \__| 
                  __/ |                     
                 |___/       By: Mukesh Dhama
---------------------------------------------                           


www.example.com is ready.
foo.example.com is ready.
bar.expample.com is ready.
foo-bar.exmaple.com is ready.
```
Screenshots will be saved into `example` directory in .png format

### License:
MIT License





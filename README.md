# nic_domain_check
check nic domain availability by python

powerd by AraKam Group
https://arakam.ir


for this we used www.nic.ir :

#Python

domain_name = 'test.ir'
link = 'http://whois.nic.ir/WHOIS?name=' + domain_nam
response = requests.get(link)

if int(response.text.find('ERROR:101:')) == -1 :

  	print(domain_nam)
  	print("not availible")
	
else:

  	print(domain_nam)
  	print("availible")
i

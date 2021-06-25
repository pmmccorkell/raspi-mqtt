#USAGE:
# from mqttClass import mqttClass
#
# server = 'the broker's IP'
# mqtt = mqttClass(host_IP=server,subscriptions=YOUR_DICTIONARY_OF_SUBSCRIPTIONS)
#	  if connecting to Adafruit IO or 3rd party with username and pass:
#		   mqtt = mqttClass(host_IP=server, username='YOUR IO USER', key='YOUR IO KEY',subscriptions=YOUR_DICTIONARY_OF_SUBSCRIPTIONS)
# mqtt.connect()
# 
#
# To Subscribe:
#
# 1. Write a function with the code you want to execute when the subscription is received.
# def function_name(topic,message):
#	 ......
#	 your code for subscription
#	 ......
#
# 2. Create a dictionary['topic_name':function_name]
# Pass this dictionary at instantiation, subscriptions=YOUR_DICTIONARY_OF_SUBSCRIPTIONS)
#
#
#
# To Publish:
# mqtt.pub('topic','message')
#
#

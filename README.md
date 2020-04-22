# Documentation of George Messaging prototype

## Goal


## Links

[Web for testing](https://webchat-dev.azurewebsites.net/#874ef829-a81e-40c8-bde1-9abcacb590e1) Note: client has to start conversation


## Goal of project

- ease of integration with the local BE
- integration efforts to local BE not needing extensive customisation
- integration efforts to local BE not encountering significant problems
- base scope of functionality implemented in/towards local bank
- no foreseable blockers found
- possibility to conduct a end-to-end message round trip
- maintenance of the chat component as one core solution (compared csas vs. ebh implementation)

## Use case of PoC

- user can communicate with a webchat chatbot
- user is able to do a handover from a chatbot to a human agent, to live chat


- vydefinovat striktneji, aby se nemohli vymlouvat
- jasný scenar co probehne
- end to end testovani - dohoda a harmonogram
- 


- 



## API Documentation
### Technology handover
TBD

### API URL HU

https://uat01.botoffice.net/erstegeorgeuat/rest/webhook/george

Example Request: 

```javascript
{
	"auth_token":"Kyiv7Po1v2",
	"event":"message",
	"timestamp":1457764197627,
	"message_token":"1234567_3",
	"sender":{ 
		"id":"ABC1"
	},
	"message":{ 
		"type":"text", 
		"text":"asd" 
	}
}
```

### Protocol diagram
![API diagram](media/API-diagram.png)




### Meeting minutes

#### 1.April
- Česka spořitelna will have access into test account of Mirra [on monday]
- We can test your API for sending and receiving messages [on monday]
- our platform for communication is this Viber group
- our user story we want to achieve with this first API integration:
sending and receiving messages between our router and your system
together we will design rest of APIs which is needed for communication
1/ starting a conversation
2/ ending a conversation
- next meeting is 7.4. 11am


#### 7. April
- we need service call to start conversation with human
- we need testing capacity for "human hondover" - tomorrow we know timing from HU
- @Jakub - next call - next tuesday
- @Jakub send usecases


#### 14. April
- HU implement webhook
- 	during today HU send time estimation
- CS implement webhook and send URL 
- 3pm kolik časů potřebují na implementaci
- next call on thursday 1pm
- access


#### 21. April
- this day HU will implement connector for ČS
- next status Thu 23. April 13h
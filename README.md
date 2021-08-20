EX4: Networking between two modems

NAME: Abdallah Natsheh 

Project Management:

`	`Server written by abdallah Natsheh.

`	`Client written by ameer haddad.

Notes:

1. On tera term in Terminal setup change new line both receive and transmit to LF.
1. After writing any command on tera term press enter.

- Server side:
1. we have 10 seconds to write wifi name using tera term (usart2).
1. we have 10 seconds to write wifi password using tera term (usart2).
1. Server start automatically initializing esp8266 to connect to the provided network until its printing server Ip and ready to serve.
1. Waiting for a button pressing event to send On, Off or Blink.
1. Waiting for a command receiving event from client through usart1 (commands: off, on, blink)
1. For checking the watchdog timer, you can send command “buddy” if it works it will be stuck until the watchdog reset the stm32.

- Client side:
1. we have 10 seconds to write wifi name using tera term (usart2).
1. we have 10 seconds to write wifi password using tera term (usart2).
1. we have 10 seconds to write server Ip address using tera term (usart2).
1. Server start automatically initializing esp8266 to connect to the provided network until its printing server Ip and ready to serve.
1. Waiting for a button pressing event to send On, Off or Blink.
1. Waiting for a command receiving event from server through usart1 (commands: off, on, blink).
1. For checking the watchdog timer, you can send command “buddy” if it works it will be stuck until the watchdog reset the stm32.

![Capture](https://user-images.githubusercontent.com/29822416/130243595-a1c3441a-c7b9-47be-9353-84986b048e01.PNG)

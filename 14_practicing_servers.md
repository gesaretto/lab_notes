#Week 14: Practicing Servers

- Log onto your consoles.

- Access your __instance__. What is an instance again?

    - Let us picture the incredibly sophisticated facility that might be the Amazon server: a huge network of machines that create a redundant system of storage and processing; let us literally picture it as a gigantic room full of machines.

	- The server is a _box_ - like the case of a personal computer - which is itself connected to other boxes: it is the allocation of a portion of this huge network of machines and interactions.

- Try typing ``ping google.com`` into my terminal; it will produce an explicit, non human-readable address to access the website; then it will start trying to understand how long it takes my machine to access the server and come back. This is called __latency time__.

- Try typing ``traceroute google.com`` now: it will trace the steps that allow my machine to access the server that hosts a website.

- In order to access my server, I will use a command called ``ssh``; this means __secure server shell__. This creates a private way of interaction between my terminal and the server. This way of access - a sort of secure tunnel - is encrypted and protected; nobody will be able to know what is in it or to tamper with it. It is a method that allows users to access website that could be otherwise inaccessible.
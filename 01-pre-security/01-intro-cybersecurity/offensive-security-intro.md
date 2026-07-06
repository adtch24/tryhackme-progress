\# Offensive Security Intro

\### Module: Introduction to Cyber Security | TryHackMe (Pre Security Path)



\## Room link

https://tryhackme.com/room/offensivesecurityintro



\## Task 1: Think Like a Hacker



Offensive security means attacking a system on purpose, before someone 

with bad intentions does — you act like the threat so you can find gaps 

before they get exploited for real. It's the flip side of defensive 

security, which focuses on blocking and monitoring instead of attacking.



\## Task 2: Starting the Lab



The lab gives you a fake banking site and the classic mistake to spot: 

a hidden admin page that isn't linked anywhere, on the assumption no one 

will find it. Used `dirb` to brute-force common directory names until it 

found one that existed:



```bash

dirb http://fakebank.thm

```



It found the hidden admin page in seconds — no real hacking skill 

needed, just a tool that guesses faster than a person would.



\*\*Takeaway:\*\* Hiding a page isn't security. If it exists on the server, 

it's reachable — real protection means authenticating the page itself, 

not just hoping no one finds the URL.



\## Reflection



Security by obscurity doesn't work — that's the one thing this room 

nails home. Relying on "no one will guess this URL" as your only defense 

means you've already lost.


<p align="center">
<img src="https://dots.neit.edu/cybercenter/wp-content/uploads/sites/42/2021/11/Capto_Capture-2021-11-19_01-41-20_PM.png"/>
</p>

# NCAE Cyber Games Handbook: Tips from a Former Competitor

Hey there! So, you’re gearing up for the **NCAE Cyber Games**, huh? As someone who’s been in your shoes, I’m here to share some tips, tricks, and tools that helped me navigate the competition. This isn’t an official guide—just some friendly advice from someone who’s been through it. Whether you’re a first-timer or looking to sharpen your skills, this handbook will help you tackle the challenges with confidence.

---

## What Are the NCAE Cyber Games?

The **NCAE Cyber Games** is a collegiate cybersecurity competition designed to be beginner-friendly while still challenging enough to help you grow. It’s all about **teamwork**, **confidence-building**, and **skill development**. If you’ve ever wondered how hackathons and cyber competitions work, this is the perfect place to start.

### Why Participate?
- **Learn by Doing**: Get hands-on experience with real-world cybersecurity challenges.
- **Build Your Resume**: Competitions like this are a great addition to your resume and can set you apart in the job market.
- **Teamwork Makes the Dream Work**: Collaborate with teammates to solve problems and achieve goals.
- **Have Fun**: Cybersecurity is exciting, and this competition is designed to be enjoyable while pushing you to grow.

---

## Tools and Techniques for Success

### Cryptography (Ciphers)
Ciphers are a staple in CTF competitions. Here are some tools to help you decode them:

- **CyberChef**: A versatile tool for decoding binary, Base64, ROT13, and more.  
  [https://gchq.github.io/CyberChef](https://gchq.github.io/CyberChef)

- **Quipqiup**: A cryptogram frequency analyzer for substitution ciphers.  
  [https://quipqiup.com](https://quipqiup.com)

- **Rumkin Cipher Tools**: A collection of ciphers with explanations.  
  [https://rumkin.com/tools/cipher](https://rumkin.com/tools/cipher)

- **Cipher Identifier**: Identify unknown ciphers with this handy tool.  
  [https://www.dcode.fr/cipher-identifier](https://www.dcode.fr/cipher-identifier)

---

### Cryptography (Steganography)
Steganography involves hiding data within files like images or audio. Use these tools to uncover hidden secrets:

- **0xRick’s Steganography Tools**: A comprehensive list of steg tools.  
  [https://0xrick.github.io/lists/stego](https://0xrick.github.io/lists/stego)

- **AperiSolve**: A one-click solution for analyzing steganography challenges.  
  [https://www.aperisolve.com](https://www.aperisolve.com)

---

### Packet Analysis
Packet analysis is crucial for understanding network traffic. These tools will help you dissect PCAP files:

- **A-Packets**: Analyzes PCAP files and provides visualizations.  
  [https://apackets.com](https://apackets.com)

- **CryptoKait’s Wireless Exploitation Guide**: A great resource for wireless challenges.  
  [https://cryptokait.com](https://cryptokait.com)

---

### Web Exploitation
Web challenges are all about finding vulnerabilities in websites. Here’s how to approach them:

- **HackTricks**: Your go-to reference for web vulnerabilities.  
  [https://book.hacktricks.xyz](https://book.hacktricks.xyz)

- **BurpSuite**: Intercept and analyze web requests to understand the app’s behavior.

**Things to check:**
- `robots.txt`
- Cookies
- Insecure Direct Object References (IDOR)
- SQL Injection
- Server-Side Template Injection (SSTI)
- Directory Bruteforcing

---

### OSINT/Trivia
Open-source intelligence (OSINT) and trivia challenges require quick thinking and research. When in doubt, Google it!

---

### Password Cracking
Password cracking involves identifying hash types and using the right attack method. Here’s how:

#### Steps:
1. **Identify the hash type** (e.g., MD5, SHA1).
2. **Choose the attack type**: Dictionary, brute-force/mask, or hybrid.
3. **Select or create a wordlist** (e.g., `rockyou.txt`).

#### Examples:
- **Dictionary Attack** (MD5 hash):  
  ```bash
  hashcat -m 0 -a 0 hashes.txt /usr/share/wordlists/rockyou.txt
  ```

- **Mask Attack** (Password starts with "Orca" and ends with 3 numbers):  
  ```bash
  hashcat -m 0 -a 3 hashes.txt Orca?d?d?d
  ```

#### Cracking Files:
1. **Convert files to hashes** using John:  
   ```bash
   pdf2john something.pdf
   office2john something.docx
   zip2john something.zip
   ```

2. **Crack the hash** using John or Hashcat:  
   ```bash
   john something -w=/usr/share/wordlists/rockyou.txt
   ```

---

## General Tips for NCAE Cyber Games

### Practice Makes Perfect
- **HackTheBox**: Practice exploitation challenges on platforms like HackTheBox to build your skills.
- **Start Strong**: Begin the competition by hardening your systems and setting up firewalls. A secure foundation is key to defending against attacks.

### Have Fun!
- **Troll the Red Team**: While staying professional, don’t forget to have fun and enjoy the competition. A little friendly trolling can keep things lively!

---

## Strategy: Secure First, CTF Later
Once you know the fundamentals, collaborate with your team to assign roles. For example:
- **CTF Solvers**: Focus on solving challenges and earning points.
- **Security Analysts**: Harden systems, set up firewalls, and prevent Red Team attacks.

Here’s why this strategy works:
1. **Secure Early**: Lock down your systems as soon as the competition starts. This ensures you’re not losing points to Red Team exploits.
2. **Farm Points**: Once your systems are secure, shift focus to CTF challenges. Every minute counts, so start earning points early.
3. **Endgame Focus**: In the final stages, CTF skills can make or break your ranking. Have at least one team member who’s a CTF expert to tackle those last-minute challenges.

Remember, the easiest and most efficient way to do well is to secure your machines early. While CTF tasks can be unpredictable, machine hardening is within your control (at least until Red Team gets in, lol). That said, don’t neglect CTF skills—they’re crucial for the endgame.

---

## Nationals-Specific Tips (University of South Florida)
The NCAE Nationals competition is next-level and takes place at the University of South Florida (USF). Here’s what to expect:

- **Expect the Unexpected**: Nationals often throws curveballs, like solving a Rubik’s Cube or picking a lock. Be ready for anything!
- **Step Out of Your Comfort Zone**: This is your chance to try new things and grow. Embrace the challenges, even if they seem weird at first.
- **Collaborate and Communicate**: Work closely with your team. Share ideas, divide tasks, and support each other.
- **Enjoy the Experience**: Nationals is a blast. Make new friends, learn new skills, and take pride in how far you’ve come.

---

## Learn and Grow
The NCAE Cyber Games website has some fantastic video tutorials to help you get started. Check them out here:  
[https://www.ncaecybergames.org/tutorials](https://www.ncaecybergames.org/tutorials)

At the end of the day, treat the competition as a learning experience. Whether you win or lose, you’ll walk away with new skills, new friends, and a deeper understanding of cybersecurity.

---

## Practice with the NCAE Sandbox
One of the best ways to prepare for the competition is by using the **NCAE Cyber Games Sandbox**. This sandbox environment allows you to practice your skills in different information security categories, and it’s very similar to the actual competition setup. It’s hands-on, practical, and the closest thing to the real deal. Check it out here:  
[https://ui.sandbox.ncaecybergames.org/](https://ui.sandbox.ncaecybergames.org/)

---

## Final Thoughts
The NCAE Cyber Games is more than just a competition—it’s an opportunity to grow, learn, and have fun in the world of cybersecurity. Use this handbook as your guide, and remember: every challenge is a chance to improve. Good luck, and may the flags be ever in your favor!

# My TryHackMe Notes

## Room 1: Introduction to Cyber Security
* **Offensive Security:** Thinking like an attacker to find system vulnerabilities.
* **Defensive Security:** Protecting systems and fixing weaknesses.

**Day one notes:**  Today I set up my notebook and answered my first TryHackMe question correctly!

**Day two notes:**  Today I learned all the roles in cybe security and I found what role i think suits me best!!
I also learned all the parts of a computer motherboard, for example; the *cpu* is the brains for the computer and the *HDD* or *SDD* are both the long term memory, and etc! I am excited for tomorrow 

**Day I don't know notes**  Offensive Security is about thinking like an attacker to find weaknesses before real hackers do.

In this room, you'll hack your first website in a safe and legal environment to see how ethical hackers operate. 

Answer the questions below
Which term describes simulating a hacker's actions to find system vulnerabilities?

Offensive Security

Defensive Security

Answer is *Offensive security*


## Now we will find a weakness in the FakeBank website. Click the button below to get started with this portion of the room.


One common mistake websites make is leaving hidden pages accessible. We'll use the terminal to run a command that can look for these.

Inside the terminal, copy and paste the dirb command below and wait for it to finish. Any lines from the output that start with + are pages that have been found.

dirb http://fakebank.thm
Dirb will find two URLs. Use this information to answer the question below.

Answer the questions below
Dirb found one URL, http://fakebank.thm/images.
What is the other hidden URL?


## Think like a Defender 
depicting a person sitting at a desk, with multiple monitors stacked on one another showing various cybersecurity and data iconograhpy such as a map, bar charts, etc.
Defensive security is the process of defending and securing devices and systems.

Before you can defend a system, you need to understand what defenders are responsible for. Defensive security focuses on detecting and investigating attacks, and responding before damage occurs.

Unlike offensive security, you do not attack systems, instead, you monitor and protect them.

Answer the questions below
What is the main goal of defensive security?

Detect and respond to attacks
Attack systems to find flaws
Answer is *Detect and respond to attacks*

Joe is an apprentice SOC analyst on his first solo shift. A moment ago, his monitoring dashboard lit up - something doesn't look right. Real SOC analysts rely on tools like this every day to separate normal activity from suspicious behaviour, and right now Joe needs your help to investigate before it becomes a serious incident.


    
**You'll need to...**
1. Open the monitoring dashboard
2. Review recent alerts
3. Identify the suspicious source IP.
Why you're doing this: Monitoring tools such as the one you'll be using provide insights as to what activity is taking place on computing devices. Defenders use tools like this dashboard to make sure that all activity taking place on these systems is legitimate, and investigate activity that is suspicious.

**Web Discovery Attack**
Automated directory enumeration detected on admin endpoints
Source IP : 32.122.195.63

**Suspicious Port Scanning**
Sequential port scan detected from external IP
ASSIGNED
HIGH
Source: 203.0.113.5
5 minutes ago
Assigned to: John Smith
Open

**Unusual Database Query Pattern**
Enumeration attempt on customer database
INVESTIGATING
MEDIUM
Source: Internal-DB-01
12 minutes ago
Assigned to: Sarah Johnson
Open

**SQL Injection Attack**
Automated SQL injection detected on payment form
UNASSIGNED
CRITICAL
Source: 198.51.100.45
25 minutes ago

Answer the questions below
Which source IP address is generating the suspicious traffic?

## Boot Sequence Diagram

**Step 1:** Press the Power Button
When we press the power button on our computer system, a signal is sent to the PSU to allow power to flow. Imagine our body being powered off when we sleep. Once we wake up and receive oxygen, our body starts pumping blood and boots up.

**Step 2:** Firmware starts
Continuing our analogy from step 1, once the body has started up, our core components are up and running, but our brain is not yet conscious. Like our bodies, a computer system contains firmware that allows all its components to start up. The central system that manages this is called the Unified Extensible Firmware Interface (UEFI). Note: We will often see the term BIOS mentioned instead of UEFI. BIOS does the same as UEFI, but has mainly been replaced by UEFI

**Step 3:** Power-On Self Test
Now that our body is up and running, it is time to test if everything is functioning as it should. If something isn't, there will be some alarm signals. One of the routines that the UEFI loads is the Power-On Self Test, which tests if every required component is present, configured correctly, and functioning.

**Step 4:** Select Boot Device
Once our body is up and running, configured correctly and fully functional, our system searches for the location of our bootup routine to start our consciousness. In our computer system the UEFI holds an ordered list which prioritizes on which device to look first for the boot up routine for the Operating System.

**Step 5:** Initiate Bootloader
Now that our system knows the part of our brain where our consciousness is located, it initiates the "load routine" to start it. Our computer systems follow a similar process: On the selected boot device, the bootloader is initiated. This bootloader transfers the Operating System from the selected boot device to the Random Access Memory. Once the OS is transferred, the UEFI gives control over the different components to the OS.
We have covered the core components of a computer system and how it boots up. At the moment, you won't realize this, but further on, when learning cyber security concepts, you will often need to recall the function of each of these core components and how they interact with each other. The boot process is a very important concept later on, as it is sometimes targeted by hackers.

Now that we know the insides of a computer, the next step is to see how the different combinations and specializations of these components lead to diverse types of computer systems. Continue to the next room **Computer Types** (coming soon) to find out.
 
 Now that the core components are installed in the computer system, it is time to boot up the system. We can compare this to how we wake up in the morning and do a quick check to see if everything is working. Only when everything is OK, do we get up and start our day. The image below shows the steps a computer system goes through before it shows you a working interface (in the form of an Operating System).

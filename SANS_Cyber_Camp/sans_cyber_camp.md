# **Day 1**

	https://go.cyberstart.com/
	
	Super Fun Optional CTF
		Tomahawque.com
		Code: new-fork
		Until aug13


## **Cyber Security for Good:**
		
        Wannacry ransoware solver - marques hudgen
		
		Diverse Background -- anyone cam become a cybersecurity professional
		
**What to do now:**
			
            Learn, understand the strengths and weakness
			Learn about ethics
			Subscribe to newsletters, insta and twitters
			Do bug bounties
			Online courses, Coursera, edxx
			Connect with people in the fields
			Attend conference when you can
			Educate others
			
			https://www.linkedin.com/in/mariluduque
			@STEMLatina
	
# **My Path into Cyber**
> *Lodrina Cherne* - Forensic Examiner

    Was introduced to people doing forensics
    
    DFIR
        Digital forensics Incident Response

    mobile predictive text
        saves what we are typing
        even if we use services that deletes sent messages, keyboard stores it.
    
    If phone is in airplane mode, and then restarted, mobile phone still shows what is buffered in mobile device
    some special tools can allow to see this information

    everytime a  pendrive is plugged in , soe hidden files are created in macos.

**Observe**

    When we open a protected document, how does the pc know that this file was.
    
**Test**

    Open an incognito tab, one incognito session based. Not window based

    computer history stores the recent websites, back button works even if internet is off. It has cached the sites to improve performance

    cyberseek.org/pathway.html




## **Cracking Hashes to pwn passwords**

> *Jason Nickola*

    Start diggin into things, If you don't understand, then you are in the right path

    The hashes itself are not secure, some salt(a random text) is added with the password 

    etc/shadow file and windows registory stores hashed passwords

    Cracking via Wordlist
        Coolwordlstgenerator - cmd tool to generate custom wordlist
        Crunch - tool to generate passwords
    
    Space Engineers - game(mincraft but space edition)

    Mask Attack
        Instead of bruteforcing everything, try inly possible combinations or wordlists..

    Hashcat command line options (explore more)



> ## Heather Mahalik
@heathermahalik, hmahalik@sans.org, smarterforensics.com

    Had no experience in computer science before

    Smartphone addiction

    what would happen to you if your phone is in wrong hands

    Mobile Forensics
        phone/tab as crime scene and decipher the truth
    
    https://www.sans.org/course/advanced-smartphone-mobile-device-forensics

    iTunes
        local backup
        backupnow

        ibackupbot
        for585.com/books
    
    Homework
        for585.com/phonelab

    how to unlock a locked phone
        iphone can be backed up through macs
        android unlocking requires expensive devices

    Coolest thing worked no:
        Bin Laden's devices
    
    autopsy - tool to recover

    elcomsoft phone breaker - tool


> ## Jason Jordan
@DFS_JasonJ
    
    Police -> Detective
    everyone is a photographer
        we all take photos of everything
    
    Metadata
        is kind of adjective that describes a thing
        everyfile has metadata, name, location, size etc..
        
        EXIF Metadata
            data embedded inside a photo
            when the picture was take, camera used etc..
            most files will have geo tags, gps co-ordinates of pictures
        
        Fighting Rhino Poaching with Digital forensics
            A criminal was arrested with rhino studds, in the pictures from his phone, using co ordinates from photos they found the riho that was killed.
        
**Analyze image metadata**
    
> exiftool path/to/image.jpg
    
    displays all metadata 
    the gps lat lon are not searchable in gmaps
    exiftool also allows to edit metadata

> exiftool path/to/img -c "gps format"

    displays gps in gmap searchable format

    Do people hide data in meta data
        some people do, embedding data using some tools by criminals
        

## Introduction to Network Analysis
> @greg_scheidel

bit.ly/31xiYnc

**Packet Capture and Analysis**

    Wireless monitoring
        good antenna used to capture packets
    Network tabs
        A to tap to B
    
    Tools
        tcpdump
            packet analysis
        Wireshark
            protocol analyzer
            understands the ip/tcp/udp/http protocols
            presents the ssl certificate, no need to find manually
        TShark
            command-line version of Wireshark
            can be used for scripting and data analysis
        libpcap/winpcap
            for live capture. these tools present to the above tools. they take advantage of these

> ctrl + shift + r - bypass cache,feteches from the server not from the cache

# Commands
>ip address
    
    lo - loopback
    eth0 - ethernet card

>ifconfig

    same output as above

>ip route
    
    what my gateways are, next device that I route though 
    every data I send out goes out through this route

>sudo traceroute -d 8.8.8.8 
    
    8.8.8.8 google server
    sudo- super user do
    path is not entirely diplayed because other devices doesnt respond to traceroute

>id

    displays user information

>ping -c1 8.8.8.8

    ping once c1 flag is ued

>sudo tcpdump -n "icmp"/"port 53"

    requires sudo access to access eth0
    filters only ICMP messages
    -n no name resolution
    "port 53" to filter only data through port

>nslookup google.com
    
    provides dns information 
    server and address information
     
>*command* --help/-h (or) man *commadn*

    to learn about what command does
    man displays more descriptive info


Q&A

    where do you pull up these commands
        man -k (search-term)
            man command list all the commands for related term
            eg: man -k browser
    
    wireless packet capturing
        wireshar
    why tcpdump over wireshar
        uses less resource, can be command lined and stored in a file for later usage
        port 80 doesnt always mean http

    

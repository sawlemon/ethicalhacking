
**Bug Hunter's Methodology v4.02**
by *Jason Haddix*

Recon part

## [Mindmap.png](https://github.com/imran-parray/Mind-Maps/blob/master/Bug%20Hunters%20Methodology%20v4/MindMap.png)

**Project Tracking**

	Xmind	
	Does the site have Multiple user roles
	How does it reference users
	How it handles special character
	What are dynamic parameters
	Does it have an API component
	What kind of errors am I seeing
	Does it have file uploads
	Have I done JS analysis for paths
	Have I done content discovery
	Color Coding the Output

**Mission**
	Wide Recon
		Identify all websites they own
	Recon
		Finding in scope domains
		Finding acquisitions
		ASN Enumeration
		Reverse Whois 
		Subdomain enumeration
		Port Analysis

**Scope Domain**

**Acquisitions**
	Crunchbase 
		 A Business intelligence portal
		
**ASN - Autonomous System Number**	
    Collection of known IP range owned by a company
	
	bgp.he.net (serch engine for ASN numbers)
	
	Tools 
		Metabigor 
		ASNLooup
			Both tools are based on keywords, co you can end up with some other organizations ANS which has similar name.
			
	ASN Enumeration with AMASS
		Frame work for domain intelligence


**reverse whois**

	Whoxy.com
		Given a domain, it ret  urns the registrar data
		
	DOMLink tool to achieve the same above
	
	AD/ Analytics Relationship
		Builtwith.com
		Also available as an extension for browser
		
		Everypage has some analytics code
			It returns the pages/sub pages which has the same code
		
		Getrelationship.py (github file) to achieve in command line
	
	Google FU
		Search for
			Copyright text
			Terms of service
			Privacy policy
	Shodan
		A tool that continuously spiders infrastructure on the internet


**Finding Subdomains**

	Linked and JS Discovery
		With BurpSuite Pro
			Burp 1.7 version 
			Use spider option to find more links
		Linked Discovering
			Gospider or hakrawler (cmdline )
		Subdomain enumeration
			Subdomainizer - tool
			Finds subdomain in js files
			Cloud services referenced in js files
	Subdomain Scrapping 
		Refer to slide
		(will be attached later)

		Tools
			Amass
			Subfinder v2
			
		Github-subdomains.py
		Shosubgo
			A Go script that runs faster
		CloudRanges
		
	Subdomain Bruteforce
		Amass does this using -rf flag
			Usually takes lnoger time
			
		Shuffledns
		
		Subdomain bruting lists
			All.txt - 7 years of dns bruteforces
			Commonspeak2
			Alteration scanning
				Dev.something.com
				But there may be
				Dev1.something.com, dev2.something … etc
				Also built into amass
				

**Favicon Analysis**
	Favicons are little images on the browser tab
	Generate a hash of the image and search it in shodan
	Favfreak - tool

**Port Scanning**
	Run port scanning on the subdomaions obtained from above methods
	
	Masscan - like nmap but faster 
		Doesn't do service scan
		Takes only ipaddresses
	Dnmasscan - converet domains to ip adddresses
	
	Feed the above output to nmap and do a service scan
	
	Brutespray - Default credential spray on open ports
	
	
**Github dorking**
	Search for a domain in github for accidentally password in github
	
**Screenshotting**
	Eyewitness,acquatone, httpscreenshot
	Feed in a list of domains, visits them with a headless browser and takes a screenshot of the page

**Subdomain takeover**

	Canitakeover xyz repo
	    Gives a list of services and fingerprints that might indicate that you can take over that subdomain
	
	Nucliei (most subdomian take over checks) and subOver - tools


**Frameworks**
	    
    Refer slide
	A-tier 
	    Findomain
			Uses most of the tools

    Re-Engine/reconengine (mmust checkout)
    Takes all the methodology and presents it as a tool. 
	
	Nuclei (must be using this tool)


***Note: This was a live note so there might be some typos, will fix them later***
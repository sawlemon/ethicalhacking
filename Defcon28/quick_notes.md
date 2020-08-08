**Red Teaming: Born from the Hacker Community**
https://www.youtube.com/watch?v=hbG2I8Vz49w

**Bug Hunter's Methodology v4.02**
by *Jason Haddix*

Recon part

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
		Given a domain, it returns the registrar data
		
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

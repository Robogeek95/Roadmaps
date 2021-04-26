# The internet and the web

As a web developer, learning the internals of the internet operations helps you make better decisions and know the justifications behind development best practices. While this is a rather lengthy document, I recommend you spend some time digging in

There are billions of web developers out there and the numbers are quickly rising everyday. But not many of these developers really understand what the internet is and how it works, but this knowledge helps us as developers appreciate web development even better.

This article will take the reader through what the internet is, it's history, why it matters we would also be digging into some of the several components that has made the internet better like the domain name service and the web hosting.

This is a breakdown of the contents we would be covering in this article

## The Internet

### The big picture

The Internet which stands for interconnected network is a global network of interconnected computer networks. It is a massive network of networks that consisting of several organizations ranging from local to global scope, the Internet carries a vast range of information resources and services using the Internet protocol suite (TCP/IP) to communicate between networks and devices.

The Internet is not the World Wide Web but the backbone of the Web. The internet is an infrastructure where any computer can communicate with any other computer globally as long as they are both connected to the Internet whereas the World Wide Web, or simply Web, is a way of accessing information over the medium of the Internet. It is an information-sharing model that is built on top of the Internet.

The most fascinating part about the internet is its decentralized structure. It is not governed in any form either technologically or legally for access and usage. Every network decides its policy and implements it within its jurisdiction. Sweet!!!

### History

The Internet dates back to the 1960s with research into what was then known as packet switching. Packet switching was conceptualized as a better and faster method to transfer data than the hardware solution to the problem.

The packet switching technology was essential to the development of ARPANET by the United States Military. ARPANET is considered the first known group of interconnected computers which is also known as the internet. This system was used to transfer confidential data between the Military. 

This data sharing technology was then opened to educational institutes in the United States to allow them to access the government’s supercomputer. Commercial Internet service providers began to arise in the late 1980s and the internet was fully commercialized in the US by 1995.

### How internet works

The computer can be connected via wired connections or via wireless connections. There are two main types of networks; The Local Area Network (WAN) and the Wide Area Network (WAN):

- **Local Area Network (LAN):** A LAN is two or more connected laptops or computers or phones sharing information with each other in a small geographic location. Examples, a network of computers at your home or work.
- **Wide Area Network (WAN):** A WAN is basically two or more interconnected LANs. These networks are farther apart than the systems in LAN. They can communicate via telephone lines or [radio waves](https://byjus.com/physics/radio-waves/).

The internet connection involves connecting billions of devices  all round the globe, using LAN connection is just not sufficient for this purpose.

The internet falls under the wide area network (WAN). The telephone infrastructure plays an important role in connecting to the internet as it already connects your house with anyone in the world. 

A modem is a piece of equipment that connects our network to the telephone infrastructure, this modem turns the information from our network into information manageable by the telephone infrastructure and vice versa.

After connecting to the telephone infrastructure through the modem, the next step is to send the messages from our network to the network we want to reach. But before we can do that, we will connect our network to an Internet Service Provider (ISP). An ISP is a company that manages some special routers that are all linked together and can also access other ISPs' routers. So the message from our network is carried through the network of ISP networks to the destination network. 

### What is HTTP

HTTP is an acronym for HyperText Transfer Protocol; HTTP is a protocol that enables resources such as HTML(HyperText Markup Language), CSS (Cascading Style Sheet), Javascript and Web APIs.

HTTP allows for data exchange on the internet, messages are requested or sent by the client such as the browser, these kinds of messages known as the requests, and served by the server known as the responses; thus implementing a client-server protocol.

There are two types of HTTP messages, requests and responses, and each type with its own format.

### what about HTTPS

Data transported with HTTP on it's own is not encrypted and is not secure, making it vulnerable and can be intercepted by third parties to gather data being passed between the two systems.

This can be addressed by using a secure version called HTTPS which stands for [h](https://www.pickaweb.co.uk/kb/what-is-http/)yper Text Transfer Protocol Secure.

HTTPS involves the use of an [SSL certificate](https://www.pickaweb.co.uk/kb/what-is-an-ssl-certificate/) -- "SSL" stands for secure sockets layer -- which creates a secure encrypted connection between the web server and the web browser.

Without HTTPS, any data passed is insecure. This is especially important for sites where sensitive data is passed across the connection, such as eCommerce sites that accept online card payments, or login areas that require users to enter their credentials.

### SMTP protocol

SMTP is an [Internet standard](https://en.wikipedia.org/wiki/Internet_Standard) for sending emails on the internet, it stands for Simple Mail Transfer Protocol. 

SMTP is a protocol that defines both MTA (Mail Transfer Agent) client to send mail and MTA server to receive the mail. SMTP simply defines how data or commands transfer from client to server and vice versa.

To transfer mails, SMTP uses three phases, i.e. connection establishment, mail transfer and connection termination and also (Mail Transfer Agent)commands, which are used to send data from client to server and responses, which is used to send data from server to client.

**Types of SMTP Protocol**

The SMTP model can be of the following two types:

- End-to-end model
- Store-and-forward model

The end to end model communicates between different organizations while communicating within the organization is the warehouse and forward model. To submit an email, the customer contacts the destination”s SMTP immediately. The SMTP server keeps the email until the receiver’s SMTP effectively receives it. The SMTP customer initiates the meeting, and the SMTP receiver reacts to the petition for the meet

**Components of SMTP**

1. Mail user agent (MUA) - SMTP begins a session between the MUA, A Mail User Agent is a program that is developed for the purpose of sending and receiving mail.
2. Mail submission agent (MSA)
3. Mail transfer agent (MTA)
4. Mail delivery agent (MDA)

SMTP begins a session between the MUA, the user and the MSA, the server. MTA and MDA are used for searching the domain for addresses and for local delivery services.

**Process of the SMTP**

1. **Composition of Mail:** The whole process begins in a Mail User Agent(MUA), a user composes an electronic mail using a Mail User Agent. The message contains two parts: body and header. The body is the main part of the message while the header includes information such as the sender and recipient address. The header also includes descriptive information such as the subject of the message. In this case, the message body is like a letter and the header is like an envelope that contains the recipient's address.
2. **Submission of Mail:** After composing an email, the mail client then submits the electronic mail to the SMTP server by using SMTP on TCP port 25.
3. **Delivery of Mail:** E-mail addresses contain two parts: the username of the recipient and the domain name. For example, azeezlukman95@gmail.com, where "azeezlukman95" is the username of the recipient and "gmail.com" is the domain name. If the domain name of the recipient's email address is different from the sender's domain name, then the Mail Submission Agent(MSA) will send the mail to the Mail Transfer Agent (MTA). To relay the email, the MTA will find the target domain. It checks the MX record from the Domain Name System to obtain the target domain. The MX record contains the domain name and IP address of the recipient's domain. Once the record is located, MTA connects to the exchange server to relay the message.
4. **Receipt and Processing of Mail:** Once the incoming message is received, the exchange server delivers it to the incoming server (Mail Delivery Agent) which stores the e-mail where it waits for the user to retrieve it.
5. **Access and Retrieval of Mail:** The stored email in MDA can be retrieved by using MUA (Mail User Agent). MUA can be accessed by using a login and password.

With these five(5) simple steps the SMTP delivers your electronic mails from your computer to the recipients computer, sending mail on the SMTP is used to ensure and set up communication rules between servers. The servers have a way of identifying themselves and announcing what kind of communication they are trying to perform. They also have a way of handling the errors such as incorrect email address. For example, if the recipient address is wrong, then receiving server reply with an error message of some kind.

## Domain Name Service

### Introduction to Domain Names

If you want to send a message to a computer, you have to specify which one. Thus any computer linked to a network has a unique address that identifies it, called an "IP address" (where IP stands for *Internet Protocol*). It's an address made of a series of four numbers separated by dots, for example: `192.168.2.10`.

That's perfectly fine for computers, but we human beings have a hard time remembering that sort of address. To make things easier, we can alias an IP address with a human-readable name called a domain name.

You can think of the DNS as a **phone book, s**o what the browser does is that it contacts the DNS (domain name service) and looks up the IP address for that URL. Once the IP address is retrieved, your browser attempts to connect to the webserver with the IP address obtained and retrieve the response sent by the server

### Domain Name Registrars

You might be wondering how you obtain a domain name, that's where the domain name registrars come into the picture

A domain name registrar is a service that lets you register and purchase domain names. Domain name registrars have been accredited by ICANN (Internet Corporation for Assigned Names and Numbers), which is a non-profit who has been delegated the responsibility to manage the Domain Name System.

Domain registrars essentially give consumers the tools to purchase and manage domain names. These changes can be made easily and through their easy to use dashboard.

All domain names records sit in a centralized database called a registry. For a domain name to be valid and recognized, it has to be added into that database with all information related to that domain name. The domain registrar is given permissions by ICANN to edit and make changes to your domain name’s data and information on the centralized database registry.

### Domain Registration

The process of acquiring a domain from a domain registrar is known as domain registration, Domain registration information is maintained by the domain name registries, which contract with domain registrars to provide registration services to the public. 

For an end-user or business to register a domain name, he has to go through a domain name registrar. The end-user or organization selects a registrar to provide the domain registration service, after the purchase is successful the registrar becomes the designated registrar for the domain chosen by the user and is registered in the central registry service, so the registered domain is no longer available for purchase. 

Only the designated registrar may modify or delete information about domain names in a central registry database.

Although the dedicated registrar is the only entity that can modify or delete information regarding domain names in the central registry, there are many [domain resellers](https://www.icann.org/resources/pages/reseller-2013-05-03-en) that allow you to sell domains. You do not have to become a designated registrar in order to sell and register domains.

### Domain Forwarding

Domain forwarding, also called URL forwarding, is a technique for making a web page available at several domains. 

When a web browser attempts to open a URL that has been redirected, a page with a different URL is opened. Similarly, domain redirection or domain forwarding is when all pages in a URL domain are redirected to a different domain

### Nameservers

Nameserver is a server on the internet specialized in handling queries regarding the location of a domain name's various services. Nameservers are a fundamental part of the Domain Name System (DNS). They allow using domains instead of IP addresses.

Matches the domain names to the ip address

In the real world, you’ll use nameservers and DNS records primarily to point your domain name towards your hosting.

**What Is a Nameserver? Explained in More Detail**

When a user enters a URL in their browser, like “kinsta.com, there needs to be some way to connect that URL with the underlying web server that powers the website at that [domain name](https://kinsta.com/blog/choose-domain-name/).

Think how difficult it would be if you had to enter the actual IP address of a web server every time you wanted to visit a website. You wouldn’t be able to remember whether it was 159.89.229.118 or 159.89.229.119 — it would be a mess!

Nameservers look like any other domain name. When you look at a website’s nameservers, you’ll typically see a minimum of two nameservers (though you can use more). Here’s an example of what they look like:

Nameservers play an important role in connecting a URL with a server [IP address](https://kinsta.com/knowledgebase/ipv4-address/) in a much more human-friendly way.

- `ns-380.awsdns-47.com`
- `Ns-1076.awsdns-06.org`

Only instead of serving up a website, those nameservers help direct traffic.

To illustrate the role that nameservers play in directing traffic on the Internet, let’s look at a real example.

Let’s say you want to visit the [Kinsta homepage](https://kinsta.com/). On the surface, this action is simple: you type “kinsta.com” into your browser’s address bar and you see the Kinsta homepage. Easy, right?

But behind-the-scenes, the high-level process actually goes something like this:

- You type “kinsta.com” into the address bar and hit enter
- Your browser sends a request to that domain’s nameservers
- The nameservers respond back with the IP address of the website’s server
- Your browser requests the website content from that IP address
- Your browser retrieves the content and renders it in your browser

### **Nameservers vs DNS Records**

In the example above, we left out one point for simplicity:

[DNS records](https://kinsta.com/knowledgebase/what-is-dns/).

DNS records are what contain the actual information that other browsers or services need to interact with, like your server’s IP address.

Nameservers, on the other hand, help store and organize those individual DNS records.

Earlier, we referred to DNS as the phone book of the Internet. But a more specific analogy would be that:

- Nameservers are the physical phone book itself.
- DNS records are the individual entries in the phone book.

If you wanted to find someone’s phone number (*back when phone books existed!*), you’d first grab the phone book itself. Then, you’d open the phone book and go through the entries to find the specific information that you need.

Armed with that knowledge, let’s look at a fuller sequence of what happens when you visit a website:

- You type “kinsta.com” into the address bar and hit enter
- Your browser uses DNS to retrieve the domain’s nameservers
- Your browser asks for the A record that contains the IP address of the web server (a specific DNS record)
- The nameservers provide the IP address from the A record
- Your browser requests the website content from that IP address
- Your browser retrieves the content and renders it in your browser

## web Hosting

A web hosting service is an Internet hosting service that allows individuals and organizations to make their website accessible via the World Wide Web. Web hosts are companies that provide space on a server owned or leased for use by clients, as well as providing Internet connectivity, typically in a data center. 

Web hosting came into play since not all companies and even individuals had the budget, the expertise or the infrastructure to do run a web server, web hosting services began to offer to host users websites on their own servers, without the client needing to own the necessary infrastructure required to operate the website.

### Web Hosting Packages Overview

There are two major classifications your website would fall under, it's either in the smaller hosting category or the larger hosting service category, these categories determine the package for the hosting service.

### **Smaller hosting services**

The most basic is [web page](https://en.wikipedia.org/wiki/Web_page) and small-scale file hosting, where files can be [uploaded](https://en.wikipedia.org/wiki/Upload) via [File Transfer Protocol](https://en.wikipedia.org/wiki/File_Transfer_Protocol) (FTP) or a Web interface. The files are usually delivered to the Web "as is" or with minimal processing. Many [Internet service providers](https://en.wikipedia.org/wiki/Internet_service_provider) (ISPs) offer this service free to subscribers. Individuals and organizations may also obtain Web page hosting from alternative service providers.

Free web hosting service is offered by different companies with limited services, sometimes supported by advertisements, and often limited when compared to paid hosting.

Single page hosting is generally sufficient for [personal web pages](https://en.wikipedia.org/wiki/Personal_web_page). Personal web site hosting is typically free, advertisement-sponsored, or inexpensive. Business web site hosting often has a higher expense depending upon the size and type of the site.

### **Larger hosting services**

Many large companies that are not Internet service providers need to be permanently connected to the web to send email, files, etc. to other sites. The company may use the computer as a website host to provide details of their goods and services and facilities for online orders.

A complex site calls for a more comprehensive package that provides [database](https://en.wikipedia.org/wiki/Database) [support](https://en.wikipedia.org/wiki/Data_center_management#Tech_Support) and application development platforms (e.g. [ASP.NET](https://en.wikipedia.org/wiki/ASP.NET), [ColdFusion](https://en.wikipedia.org/wiki/ColdFusion), [Java EE](https://en.wikipedia.org/wiki/Java_Platform,_Enterprise_Edition), [Perl/Plack](https://en.wikipedia.org/wiki/Plack_(software)), [PHP](https://en.wikipedia.org/wiki/PHP) or [Ruby on Rails](https://en.wikipedia.org/wiki/Ruby_on_Rails)). These facilities allow customers to write or install scripts for applications like [forums](https://en.wikipedia.org/wiki/Internet_forum) and [content management](https://en.wikipedia.org/wiki/Content_management). Also, [Secure Sockets Layer](https://en.wikipedia.org/wiki/Secure_Sockets_Layer) (SSL) is typically used for websites that wish to keep the data transmitted more secure.
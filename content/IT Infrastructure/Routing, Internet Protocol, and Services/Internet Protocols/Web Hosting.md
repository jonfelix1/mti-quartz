---
tags: 
- inti
- note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Routing, Internet Protocol and Services]]"
---

# Web Hosting

To successfully run a website via a web server, it's essential to place your website files (such as .html or other formats) on the server's hard disk. This enables the web server software to send these files in response to web-browsing requests. Below are the steps and key concepts involved in web hosting.

## Uploading Website Files

To upload your web files to a web server's hard drive, you have two primary options:

1. **Server-Side Application**:
   - You can use a server-side application (like a text editor such as Nano) to create content directly on the server. This approach allows you to manage files and make edits on the server itself.

2. **File Transfer Protocol (FTP)**:
   - Alternatively, you can copy content from your local hard drive to the server's hard drive using FTP. This method typically requires an FTP client (like FileZilla) to facilitate the file transfer.
   - Regardless of the approach, you must have an account on the web server to perform these actions.

## Web Server Operating Systems

The two most popular operating systems for web servers are:

- **Unix**: Most commonly used for web hosting due to its stability and security.
- **Windows**: Also used but less popular compared to Unix.

## Web Hosting Services

Several web hosting companies offer accounts on their servers, including:

- **BlueHost**
- **DreamHost**
- **Arvixe**
- **TMDHosting**

Typical costs for hosting services start at around **$10/month**, with prices increasing based on additional bandwidth or processing power. 

Free hosting services are available, such as DuckID for the University of Oregon, although these may not provide warranties or service plans.

### Account Setup

When setting up a web hosting account, you will need to provide several key pieces of information:

- **Username**: Often based on a unique identifier (e.g., DuckID).
- **Password**: You choose this password and can change it later.
- **Domain Name**: Includes the domain extension (e.g., .com).
- **Email Address**: Used for account confirmation.

Your username and password will be utilized to create two accounts on the same remote server:

- **Web Server Account**: For managing web content.
- **FTP Server Account**: For file transfers.

## Accessing Your Web Hosting Account

Once your account is set up, you can log in via different methods:

- **FTP Access**: Use an FTP client like FileZilla to connect.
  - Example: `ftp://myclass.mysitehosted.com`
  
- **HTTP Access**: Access your web server control panel via a web browser.
  - Example: `http://cpanel.myclass.mysitehosted.com`

### Account Quotas

Your web hosting account will typically come with certain limitations, such as:

- **File Storage**: e.g., 250 MB
- **Bandwidth**: e.g., 2.5 GB/month

Given these quotas, large files like audio/video and substantial photo files should be stored elsewhere, such as on platforms like Flickr for images or Vimeo for videos. The allocated limits are often sufficient for learning about server administration and setting up basic applications like a WordPress blog.

## Domain Name Configuration

To connect your domain name to your web server, follow these steps:

1. **Access Your Control Panel**:
   - Log in to your control panel using the URL (e.g., `http://cpanel.myclass.mysitehosted.com`) to manage your web server account.

2. **Point Domain Name to Web Server**:
   - Use a domain registrar (e.g., GoDaddy) to configure your new domain name with the appropriate Domain Name Server (DNS) settings.
   - The DNS servers associated with your web hosting account will typically have names like:
     - **Primary**: `NS1.MYCLASS.MYSITEHOSTED.COM`
     - **Backup**: `NS2.MYCLASS.MYSITEHOSTED.COM`

3. **Configuring DNS in GoDaddy**:
   - Log into your GoDaddy account.
   - Navigate to: **All Products → Domains → Domain Management**.
   - Select your domain name and click on “Set Nameservers” located near the lower left.
   - Enter the two DNS server names provided by your web hosting company.

### Finalizing Domain Configuration

After setting the DNS servers, it may take some time for changes to propagate across the Internet. Once propagated, users will be able to access your website via the domain name you registered, linking to the files hosted on your web server.

## Conclusion

Web hosting is a vital component of making a website accessible on the Internet. By understanding the processes of uploading files, selecting hosting services, managing accounts, and configuring domain names, you can effectively establish and manage your online presence. Proper setup and management will ensure that your website is accessible, functional, and ready to meet user demands.

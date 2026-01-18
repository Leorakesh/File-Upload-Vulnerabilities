# File-Upload-Vulnerabilities
Day 24 of 100 days challenge

Day 24 – File Upload Vulnerabilities
 Overview

On Day 24, I focused on understanding and testing file upload vulnerabilities, one of the most dangerous issues in web applications. When file uploads are not properly validated, attackers can upload malicious files and execute code on the server.

 What Are File Upload Vulnerabilities?

File upload vulnerabilities occur when an application allows users to upload files without strong security checks. Attackers can abuse this to upload:

Web shells

Malware scripts

Backdoors

Modified file types

If the server executes these files, it can lead to remote code execution (RCE) and full system compromise.

Common Causes

Missing file type validation

Trusting client-side checks only

No MIME type verification

Allowing executable extensions (.php, .jsp, .aspx)

Upload directory with execute permissions

Weak file renaming logic

Testing Approach

During testing, I looked for:

Upload bypass techniques

Double extensions (shell.php.jpg)

Content-Type manipulation

Magic byte modification

Executable path access

Server-side validation weaknesses

Impact

Remote code execution

Data breaches

Website defacement

Full server takeover

Prevention

Validate file extensions and MIME types

Use server-side checks

Rename uploaded files securely

Store uploads outside the web root

Disable execution in upload directories

Scan files with antivirus

 Learning Outcome

Day 24 improved my understanding of how insecure upload features can become critical attack vectors and how proper validation and storage controls prevent exploitation.

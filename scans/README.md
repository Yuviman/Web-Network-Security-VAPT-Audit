# gobuster
Gobuster is a directory/file brute-forcing for web paths or DNS subdomains using wordlists.

When to use: find hidden directories, admin panels, upload folders.

Example: gobuster dir -u http://10.0.2.15 -w /usr/share/wordlists/dirb/common.txt

# dirb
This is another web directory brute-forcer (simple and installed by default on many pentest distros).

When to use: alternative to gobuster when you prefer its wordlists or output style.

Example: dirb http://10.0.2.15 /usr/share/wordlists/dirb/common.txt

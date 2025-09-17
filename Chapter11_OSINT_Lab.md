# OSINT Lab Setup Instructions

This guide provides practical, step-by-step exercises to practice Open-Source Intelligence (OSINT) using free online tools.

---

## Step 1: Prepare Your Environment

- Use a modern web browser (Chrome, Firefox, Brave).
- Consider running in a **virtual machine** or **incognito mode** for safety.
- Ensure you have internet access.

---

## Step 2: Practice Google Dorking (Advanced Google Searches)

Try the following queries in Google:

- Find PDFs on a site:  
  ```
  site:example.com filetype:pdf
  ```

- Find login portals:  
  ```
  inurl:login site:example.com
  ```

- Find open directories:  
  ```
  intitle:"index of" site:example.com
  ```

- Find subdomains:  
  ```
  site:*.example.com -www
  ```

- Search for resumes or sensitive terms:  
  ```
  intitle:"curriculum vitae" site:example.com
  ```

👉 Explore more examples in the [Google Hacking Database](https://www.exploit-db.com/google-hacking-database).

---

## Step 3: Investigate Domains with WHOIS

1. Visit [https://who.is](https://who.is) or [https://lookup.icann.org](https://lookup.icann.org).
2. Enter a domain (e.g., `packtpub.com`).
3. Review the details:
   - Creation/expiration dates
   - Registrar info
   - DNS servers
   - Contact details (may be masked)

Look for red flags:
- Recently registered domains
- Suspicious or masked ownership
- Foreign registrars
- Disposable emails

---

## Step 4: Run Reverse Image Searches

### Using Google Images
1. Go to [https://images.google.com](https://images.google.com).
2. Click the camera icon.
3. Paste an image URL or upload a file.

### Using TinEye
1. Go to [https://tineye.com](https://tineye.com).
2. Upload or paste an image URL.
3. Review where else the image appears.

👉 Try with a suspicious LinkedIn profile picture or a generated image from [This Person Does Not Exist](https://thispersondoesnotexist.com).

---

## Step 5: Extract Metadata from Files

1. Go to [https://exif.tools](https://exif.tools) or [https://www.metadata2go.com](https://www.metadata2go.com).
2. Upload an image or document.
3. Review metadata such as:
   - Timestamps
   - GPS coordinates
   - Device type
   - Author or software info

---

## Step 6: Check for Breach Data

1. Go to [https://haveibeenpwned.com](https://haveibeenpwned.com).
2. Enter an email address you control.
3. Review results:
   - Which sites were breached
   - What data was exposed (email, passwords, etc.)

👉 To test passwords (safely), use [HIBP Passwords](https://haveibeenpwned.com/Passwords).  
⚠️ Never enter your real password.

---

## Step 7: Practice Responsibly

- Stick to **public and safe data**.
- Do not exploit, download, or redistribute sensitive content.
- Always consider **intent and ethics** when using OSINT tools.

---

✅ You now have a toolkit of OSINT skills: Google dorking, WHOIS lookups, reverse image search, metadata analysis, and breach awareness.

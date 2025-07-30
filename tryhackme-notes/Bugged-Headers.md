# 🧠 Room: Bugged Headers (TryHackMe)
📅 Date: July 29, 2025

---

## 🔍 Recon with `curl`

```bash
curl -I https://target.thm                # Get only headers  
curl -v https://target.thm                # Verbose request and response  
curl -s -D - https://target.thm | less    # Silent, show headers, pipe to pager  
curl https://target.thm/THM               # Try possible flag path  
curl https://target.thm/flag              # Try known flag path  
curl https://target.thm/robots.txt        # Check for disallowed paths  
curl https://target.thm/.hidden           # Look for hidden content  

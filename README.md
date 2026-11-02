# Art by Priti — Full Website & Separate `/admin` CMS Package

## Architecture Overview
1. **`index.html` (Public Frontend + Collector Account Portal)**
   - **Zero Admin Links on Homepage:** The public website is 100% dedicated to visitors and collectors. There are no admin buttons on the homepage.
   - **Featured Top Styles:** Displays the signature styles selected inside your CMS.
   - **Pre-Made Collector Vault (Make an Offer):** Visitors can browse ready-to-ship original artworks and submit a custom price offer.
   - **Studio Announcements:** Lists announcements by Subject and a brief teaser summary. Clicking an announcement opens a full reader modal.
   - **User Login & Collector Account:** Visitors can sign up / log in to:
     1. Place Custom Orders & submit detailed custom requirements with reference photo validation.
     2. View their orders, offers, and read direct replies sent by Priti from the CMS.
     3. Update their Profile Settings (name, phone, default shipping address, password).
   - **Contact Us Form:** Sends visitor inquiries straight into the CMS Contact Inbox.

2. **`admin.html` + `vercel.json` (`site.com/admin` CMS)**
   - Accessible exclusively via **`your-site.vercel.app/admin`** (or opening `admin.html` locally).
   - **Default Login:** ID: `priti` | Password: `priti@2026` (changeable inside the CMS).
   - **CMS Modules:**
     1. **All Received Orders & Offers:** View every custom order and pre-made art offer in one place. Send a reply that simultaneously posts to the user's account dashboard AND dispatches an email to their inbox.
     2. **Homepage Top Styles Curation:** Upload portfolio artworks and check/uncheck which ones appear in the "Featured Top Styles" section on the homepage.
     3. **Pre-Made Art Vault Manager:** Add ready-to-ship originals, set prices, and mark pieces as Available or Sold.
     4. **Announcements Publisher:** Create announcements with a Subject, short teaser description, and full story.
     5. **Contact Us Inbox:** Read and reply to all Contact Us form submissions.
     6. **Security & Banner Settings:** Update top bar text and Admin credentials.
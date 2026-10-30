=============================================================
LITTLESTORY STUDIO - DEPLOYMENT GUIDE (VERCEL + CASHFREE)
=============================================================

Included Files in this ZIP:
1. index.html       -> Your conversion-optimized landing page (No test-drive, streamlined)
2. thank-you.html   -> The post-payment instant download delivery page
3. README.txt       -> This guide

-------------------------------------------------------------
STEP 1: UPLOAD YOUR STORY BUNDLE ZIP TO GOOGLE DRIVE
-------------------------------------------------------------
1. Upload your master ZIP file (Kids_Story_Landing_Page_Package.zip) to your Google Drive.
2. Right-click the file in Google Drive -> Click "Share" -> Change General Access to "Anyone with the link can view".
3. Copy the link.
4. Open 'thank-you.html' in Notepad or VS Code:
   - Search for: YOUR_GOOGLE_DRIVE_OR_CLOUD_DOWNLOAD_LINK
   - Replace it with your Google Drive link.
   - Save the file.

-------------------------------------------------------------
STEP 2: CREATE YOUR CASHFREE PAYMENT LINK
-------------------------------------------------------------
1. Log in to your Cashfree Dashboard: https://merchant.cashfree.com/
2. Go to "Payment Gateway" -> "Payment Links" -> "Create Payment Link".
3. Enter Details:
   - Purpose: 120 Kids Story Creator Kits
   - Amount: 129 (INR)
   - Link Type: Reusable / Multi-use
   - Collect Customer Details: Enable Phone Number and Email
4. Under "Advanced Options / Redirect Settings":
   - Set Return URL / Redirect URL to your thank-you page:
     https://your-site-name.vercel.app/thank-you.html
     (Note: You can update this after getting your live Vercel URL in Step 3)
5. Copy your generated Cashfree payment link (e.g. https://payments.cashfree.com/links/xxxx).
6. Open 'index.html' in Notepad or VS Code:
   - Search for: YOUR_CASHFREE_PAYMENT_LINK (there are 3 occurrences)
   - Replace all 3 with your Cashfree payment link.
   - Save the file.

-------------------------------------------------------------
STEP 3: DEPLOY TO VERCEL (100% FREE)
-------------------------------------------------------------
Option A: Drag & Drop Deploy (Easiest & Fastest - No Git Needed)
1. Go to https://vercel.com and log in or create a free account.
2. In your dashboard, click "Add New..." -> "Project".
3. Look for the "Deploy a local folder" or Drag-and-Drop section, OR install the Vercel CLI.
   Alternatively, you can use:
   - Netlify: https://app.netlify.com/drop (Literally drag the folder containing index.html and thank-you.html, and it is live in 5 seconds).

Option B: Deploy via GitHub (Best for ongoing updates)
1. Create a free repository on GitHub (e.g., 'story-bundle-landing').
2. Upload 'index.html' and 'thank-you.html'.
3. Go to https://vercel.com -> Click "Add New Project" -> "Import Git Repository".
4. Select your repository and click "Deploy".
5. In 10 seconds, Vercel gives you an active HTTPS URL like:
   https://story-bundle-landing.vercel.app

-------------------------------------------------------------
STEP 4: FINAL CHECK
-------------------------------------------------------------
1. Update your Cashfree Redirect URL with:
   https://your-vercel-domain.vercel.app/thank-you.html
2. Test by opening the landing page in Incognito mode, clicking the purchase button, and making sure the checkout page loads smoothly.
=============================================================

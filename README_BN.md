# Comedor Pepinos — আপডেটেড দ্বিভাষিক ওয়েবসাইট

## ফাইল ও সম্পদ
- `index.html` — সম্পূর্ণ single-page site; HTML, CSS ও JavaScript একই ফাইলে।
- `assets/pepinos-logo-original.jpg` — ব্যবহারকারীর সরবরাহ করা মূল লোগো ইমেজ।
- `assets/pepinos-logo-header.jpg` — একই সরবরাহ করা লোগোর header-friendly crop।
- `assets/maps-gallery/maps-photo-000.jpg` থেকে `maps-photo-062.jpg` — ব্যবহারকারীর সরবরাহ করা ৬৩-পৃষ্ঠার PDF থেকে বের করা ৬৩টি ইমেজ।
- `SOURCES_AND_VERIFICATION.md` — উৎস, সীমাবদ্ধতা ও যাচাইয়ের নোট।

## সংশোধন ও ফিচার
- Header ও footer-এ সরবরাহ করা Pepinos লোগো।
- ৬৩টি PDF-এ থাকা ইমেজের গ্যালারি, ক্যাটাগরি ফিল্টার এবং click-to-open lightbox; previous/next বাটন, Escape, এবং keyboard arrow support।
- মেনুর কার্ডে বাহ্যিক stock-photo লিংকের বদলে সরবরাহ করা PDF-এ থাকা স্থানীয় ইমেজ।
- Spanish / English auto-localization; ব্রাউজার ভাষা থেকে প্রাথমিক ভাষা বাছাই এবং ম্যানুয়াল পছন্দ সংরক্ষণ।
- মোবাইল নেভিগেশন ও মেনু ফিল্টার।
- Android ফোন, ট্যাবলেট ও কম্পিউটারে responsive layout।
- Reduced Motion সেটিং অনুসরণ করে অ্যানিমেশন।
- Click-to-call, WhatsApp, email, Facebook, Instagram, Google Maps directions ও map embed।
- “Use my location” কেবল ব্যবহারকারী চাপলে অবস্থানের অনুমতি চায়; GPS ব্যবহারের জন্য ব্রাউজার অনুমতি এবং সাধারণত HTTPS hosting দরকার।
- Mexico City-এর স্থানীয় সময় অনুযায়ী Open/Closed ব্যাজ; সময়সূচি এখনও মালিকের কাছে নিশ্চিত করতে হবে।

## ছবি ও Google Maps আর্কাইভ সম্পর্কে জরুরি সীমাবদ্ধতা
গ্যালারির ৬৩টি ইমেজ **আপনার এই চ্যাটে দেওয়া PDF থেকেই** বের করা হয়েছে। PDF-তে খাবার, লোকেশনের ছবি, মেনু/চকবোর্ড, প্রচারণার গ্রাফিক ও লোগো আছে; কিছু ইমেজ পুনরাবৃত্তও হতে পারে। তাই সাইটে ওই ৬৩টি সংযুক্ত ইমেজ পাওয়া যায়, কিন্তু এটিকে Google Maps-এর সঙ্গে live sync অথবা শুরু থেকে এখন পর্যন্ত Google Maps-এ থাকা প্রতিটি ছবি/ভিডিও/রিভিউ/আপডেটের পূর্ণ আর্কাইভ বলা যাবে না। নতুন কনটেন্টের জন্য অফিসিয়াল Google Maps লিংক ব্যবহার করুন।

Google Places API দিয়ে অনুমোদিত নির্দিষ্ট ছবি দেখানোর জন্য Place ID, API key, photo resources ও প্রযোজ্য attribution দরকার; API response-এ সর্বোচ্চ ১০টি photo reference আসতে পারে। এটা সম্পূর্ণ historical archive নয়। API key এখানে এমবেড করা হয়নি।

## Publish করার আগে
1. ব্যবসার মালিকের অনুমতি নিন এবং ফোন, WhatsApp, ইমেইল, ঠিকানা, Instagram লিংক নিশ্চিত করুন।
2. সব খাবারের নাম, মূল্য, খোলার সময়, holiday schedule এবং live rating মালিক/Google Maps-এর বর্তমান তথ্যের সঙ্গে মিলিয়ে নিন। অজানা দাম বানিয়ে যোগ করা হয়নি।
3. `index.html`-এর পাশাপাশি `assets` ফোল্ডারটিও hosting-এ আপলোড করুন; শুধু HTML আপলোড করলে ছবি লোড হবে না।
4. GPS feature-এর জন্য HTTPS hosting ব্যবহার করুন। `file://` preview বা কিছু hosting preview-তে geolocation সীমিত হতে পারে।

## খুলে দেখুন
`index.html` Chrome-এ খুলে ডেমো দেখা যায়। অনলাইনে প্রকাশ করতে পুরো folder static hosting-এ আপলোড করুন (যেমন GitHub Pages, Netlify বা Hostinger)।

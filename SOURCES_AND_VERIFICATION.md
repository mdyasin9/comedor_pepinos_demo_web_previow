# Comedor Pepinos — উৎস ও যাচাই রিপোর্ট

**আপডেট:** ২২ অক্টোবর ২০২৬

## এই সংস্করণে ব্যবহার করা সম্পদ

- ব্যবহারকারীর সরবরাহ করা Pepinos লোগো ইমেজ থেকে header crop তৈরি করা হয়েছে; আসল full image-টিও `assets/pepinos-logo-original.jpg`-এ রাখা হয়েছে।
- ব্যবহারকারীর সরবরাহ করা `IMG_20261022_100857.pdf` ৬৩ পৃষ্ঠার একটি ছবি-ভিত্তিক PDF হিসেবে render/inspect করা হয়েছে। `pdfimages` দিয়ে PDF থেকে ৬৩টি JPEG image resource বের করে `assets/maps-gallery/maps-photo-000.jpg` ... `maps-photo-062.jpg` হিসেবে সংরক্ষণ করা হয়েছে।
- সাইটে ওই ৬৩টি ইমেজের গ্যালারি, চারটি ক্যাটাগরি filter, lightbox, previous/next, Escape ও arrow-key controls যুক্ত হয়েছে।
- আগের Unsplash stock-image references সরিয়ে PDF-এ থাকা লোকাল ইমেজ ব্যবহার করা হয়েছে।

## ব্যবসা সংক্রান্ত ইনপুট/লিংক

- নাম: Comedor Pepinos
- Google Maps short link (ব্যবহারকারীর দেওয়া): https://maps.app.goo.gl/f51fSC7jspcKztcM6
- Facebook (ব্যবহারকারীর দেওয়া): https://www.facebook.com/comedorpepinos?mibextid=ZbWKwL
- Instagram profile reference: https://www.instagram.com/comedor_pepinos/ — প্রকাশের আগে সঠিক official handle নিশ্চিত করুন।
- ফোন/WhatsApp ও ইমেইল আগের সাইটে ব্যবহারকারীর দেওয়া বিবরণের ভিত্তিতে আছে: +52 56 3077 1111; comedorpepinos@gmail.com। লাইভ করার আগে মালিকের কাছে যাচাই করুন।
- আগের public listing reference-এ Magnolia 64, Ciudad de México এবং সাধারণ সাপ্তাহিক সময়সূচির উল্লেখ ছিল; এটি বর্তমান Google Maps listing-এ পুনরায় নিশ্চিত করা হয়নি। তাই প্রকাশের আগে যাচাই করা আবশ্যক।

## ছবির শ্রেণিবিন্যাস সম্পর্কে নোট
গ্যালারির ক্যাটাগরিগুলো PDF পৃষ্ঠার দৃশ্যমান বিষয়বস্তু দেখে আনুমানিকভাবে সাজানো—যেমন খাবার, লোকেশনের ছবি/পরিবেশ, এবং মেনু/প্রচারণা। এগুলো কোনো live Google metadata নয়। PDF-তে থাকা সব ৬৩টি image resource সাইটে অন্তর্ভুক্ত হয়েছে, তবে repeated photos থাকতে পারে এবং সব পৃষ্ঠা অনন্য আলাদা ছবি নাও হতে পারে।

## Google Maps-এর অতীত/লাইভ কনটেন্ট সম্পর্কে সীমা
এই সাইট Google Maps-এর সঙ্গে live sync করে না। user-provided PDF-এ থাকা ৬৩টি image resource অন্তর্ভুক্ত করা হয়েছে, কিন্তু এটি শুরু থেকে এখন পর্যন্ত Google Maps-এর সব ছবি, ভিডিও, Street View/360°, Popular Times, updates, reviews বা সম্পূর্ণ menu item-এর নিশ্চয়তা নয়। সাইটের media hub-এ দেওয়া Google Maps/Facebook/Instagram লিংক ব্যবহারকারীদের সংশ্লিষ্ট উৎসে পাঠায়।

Google Place Photos API তথ্য: https://developers.google.com/maps/documentation/places/web-service/place-photos
Google Maps URLs: https://developers.google.com/maps/documentation/urls/get-started
Google Maps user-contributed content policy: https://support.google.com/contributionpolicy/answer/7412443?hl=en

## ফিচার ও functional checks

- HTML-এ IDs unique কি না, local image paths উপস্থিত কি না, external anchors-এ href আছে কি না, এবং JavaScript syntax যাচাই করুন/করা হয়েছে প্যাকেজ তৈরির সময়।
- Gallery category filters ও lightbox JS controls যুক্ত রয়েছে। Browser automation/live click-test এই runtime-এ করা হয়নি; প্রকাশের পর Android Chrome এবং desktop browser-এ প্রতিটি CTA, social link, GPS prompt ও modal পরীক্ষা করুন।
- `index.html`-কে একা সরালে local image paths ভাঙবে; `assets/` directory একই folder structure-এ রাখতে হবে।

## প্রকাশের আগে আবশ্যিক যাচাই
- মালিকের অনুমতি, logo/photo rights ও customer photo permissions।
- WhatsApp/phone/email, official social URLs, exact menu/prices, hours/holiday times, rating/review count এবং map address।
- GPS feature-এর জন্য HTTPS ও browser permission।

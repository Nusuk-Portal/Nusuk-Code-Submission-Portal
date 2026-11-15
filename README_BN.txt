NUSUK CODE SUBMISSION PORTAL — বাংলা নির্দেশনা

১) Supabase-এ Project তৈরি করুন।
২) SQL Editor-এ supabase_setup.sql-এর সম্পূর্ণ কোড Paste করে Run করুন।
৩) Authentication > Users থেকে Admin user তৈরি করুন।
৪) Admin User ID কপি করে SQL Editor-এ চালান:
   insert into public.portal_admins(user_id) values ('YOUR_ADMIN_USER_UUID');
৫) Project Settings > API Keys থেকে Project URL ও Publishable key (sb_publishable_...) কপি করুন।
৬) app.js-এর প্রথম দুইটি constant-এ URL ও Publishable key বসিয়ে Save করুন। Secret/service_role key কখনো browser code-এ দেবেন না।
৭) GitHub repository-র root-এ index.html, style.css, app.js ও supabase_setup.sql আপলোড করুন।
৮) Repository Settings > Pages > Deploy from a branch > main > /(root) > Save নির্বাচন করুন।
৯) GitHub Pages-এর দেখানো URL খুলে পরীক্ষা করুন।

Features: প্রতি non-empty line আলাদা record; duplicate অনুমোদিত; public read/submit; individual copy; copy all; Excel-এ date; website-এ date hidden; admin edit/delete; responsive layout।

Security note: Public insert চালু থাকায় spam হতে পারে। প্রয়োজনে পরে CAPTCHA/rate limit যোগ করুন। Supabase service_role/secret key কখনো app.js-এ রাখবেন না।
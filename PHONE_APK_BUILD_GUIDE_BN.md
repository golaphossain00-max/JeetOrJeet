# ফোন থেকে APK তৈরি করার নির্দেশিকা

এই ZIP-এ GitHub Actions cloud-build workflow যোগ করা হয়েছে। এতে আপনার নিজের কম্পিউটার লাগবে না, তবে GitHub অ্যাকাউন্ট ও ফোনের ব্রাউজার লাগবে।

1. ZIP ফাইলটি ফোনে ডাউনলোড করে Extract করুন।
2. GitHub-এ সাইন ইন করে নতুন Public বা Private repository তৈরি করুন।
3. Extract করা ফোল্ডারের সব ফাইল GitHub repository-তে আপলোড করুন। `.github/workflows/android-apk.yml` ফাইলটিও আপলোড হয়েছে কি না দেখুন।
4. Repository-এর Actions ট্যাবে যান।
5. “Build JEET OR JEET Android APK” workflow খুলে “Run workflow” চাপুন।
6. Build সফল হলে workflow run-এর নিচে Artifacts থেকে `jeet-or-jeet-debug-apk` ডাউনলোড করুন।
7. ZIP খুলে `app-debug.apk` ফাইলটি Android ফোনে ইনস্টল করুন। ফোনে “Install unknown apps” অনুমতি চাইতে পারে।

সতর্কতা:
- এটি debug APK; Play Store release-এর জন্য signed release build, privacy policy, security review এবং Play policy compliance দরকার।
- বর্তমান অ্যাপটি local demo prototype। Login/Register ডেটা ওই ডিভাইসেই থাকে; OTP, cloud database, server-side admin authorization বা payment backend নেই।
- Firebase বা অন্য backend যোগ করতে হলে মালিকের নিজস্ব project credentials ও configuration লাগবে। কোনো secret/password এখানে দেবেন না।
- Real-money betting, deposits, withdrawals বা cash-prize wagering এই প্রকল্পে নেই এবং যোগ করা হবে না।

 
## Links

- github-link: https://nodejs.org/en
- vercel-link: https://vitejs.dev/ 

✓ আপনাদের News Feed এপ্লিকেশন এর টেমপ্লেট দিয়ে দেয়া হয়েছে এটিকে রিয়্যাক্টে কনভার্ট করে API থেকে নিউজ নিয়ে এসে দেখাতে হবে । এক্ষেত্রে আপনাদের এই API ব্যবহার করতে হবে - News Api । এবং আপনারা Fetch এর পরিবর্তে Axios বা অন্য কিছু ব্যবহার করতে পারবেন না ।

[এই এসাইনমেন্ট এ আপনাকে .env ফাইলে API Key রাখতে হতে পারে । কিন্তু খেয়াল রাখবেন, .gitignore এ যেন .env ফাইল ignore করা না থাকে । অর্থাৎ, আপনি যখন github এ কোড পুশ দিবেন, তখন যেন আপনার কোডের সাথে .env ফাইল ও আপলোড হয়। যদি কোনো কারণে আপনার .env আমরা এসাইনমেন্ট চেক করার সময় না পাই, সেক্ষেত্রে আপনার এসাইনমেন্ট মার্কিং করা হবে না । এবং পরবর্তিতে আপনার ভুল সংশোধন এর ও কোনো প্রকার সুযোগ দেয়া হবে না ।]

✓ নেভিগেশনবার এ বিভিন্ন ক্যাটেগরির নাম থাকবে, সেই নাম গুলোতে ক্লিক করলে Filter করে শুধু সেই ক্যাটেগরি এর নিউজ দেখাতে হবে । অর্থাৎ এখানে আপনাকে Filter Feature ইমপ্লিমেন্ট করতে হবে । উল্লেখ্য, আপনি চাইলে টেমপ্লেটে দেয়া ক্যাটেগরির নাম গুলো পরিবর্তন করতে পারেন । এই ক্যাটেগরির নাম আপনি Hard Code করে লিখতে পারেন । তবে সর্বনিম্নে পাঁচটি ক্যাটেগরি আপনাকে দেখাতেই হবে ।

✓ আপনাকে সার্চ ফিচার ইমপ্লিমেন্ট করতে হবে । এক্ষেত্রে API থেকে 'title' এবং 'description' এর মধ্যে থেকে সার্চ করে নিয়ে এসে রেজাল্ট দেখাতে হবে । সার্চ এর ক্ষেত্রে Debounce ব্যবহার করতে হবে । যদি Debounce সম্পর্কে না জেনে থাকেন তবে এই ভিডিও দেখে নিতে পারেন - Debounce Function in Javascript

✓ UI তে আপনারা সার্চ আইকন পাচ্ছেন শুধু। কিন্তু সার্চ ইমপ্লিমেন্ট করতে হলে আপনাকে mark-up এ একটি ইনপুট বক্স নিয়ে আসতে হতে পারে। এটি আপনি আপনার সাধারণ জ্ঞান থেকে করে নিতে পারবেন। ভাল ইউজার এক্সপিরিয়েন্সের জন্য যদি mark-up এ কিছু যুক্ত করতে হয়, তাহলে সেটি আপনি করতে পারেন।

✓ আপনাকে একটি Custom Hook হুক বানাতে হবে । সেটির নাম হতে হবে useNewsQuery এবং সেটির কাজ হবে Fetch দিয়ে API রিকুয়েস্ট করা । আপনাদের যেই News Api টি দেয়া হয়েছে, সেটিতে আপনারা চাইলে Category সিলেক্ট করেও রিকুয়েস্ট করতে পারেন আবার সিলেক্ট না করেও রিকুয়েস্ট করতে পারেন । সিলেক্ট করে রিকুয়েস্ট করলে, শুধু ঐ ক্যাটেগরির নিউজ আসবে, আর সিলেক্ট না রিকুয়েস্ট করলে সব নিউজ আসবে । এখন আপনাকে হুক এমন ভাবে বানাতে হবে যেন, একটি হুক দিয়েই আপনি Categorized এবং Uncategoriezed দুই ধরণের নিউজই নিয়ে আসতে পারেন ।

সামগ্রিক বিধিনিষেধঃ
API এর জন্যে আপনি Fetch এর পরিবর্তে Axios ব্যবহার করতে পারবেন না ।
যেহেতু Routing এখন পর্যন্ত দেখানো হয়নি, যেহেতু সেটি আপনি ব্যবহার করতে পারবেন না ।
এই এসাইনমেন্ট এর জন্যে শুধু মাত্র পাঁচটি রিকুয়ারমেন্ট লিখে দেয়া হয়েছে, এগুলোর বাহিরেও আপনার কোডের হাইজিন ফ্যাক্টর এবং বেশ কিছু জায়গায় আমরা কিছু সমস্যা বা ইউজার এক্সপেরিয়ান্স আর ভালো করার scope রেখে দিয়েছি । সেগুলো আপনাকে implement করতে হবে এবং সেগুলো Implement এর ক্ষেত্রে আপনার কমন্সেস আমরা খেয়াল করবো । এ বিষয়ে Discord এ কোন ধরণের আলোচনা করা যাবে না ।
আপনি চাইলে useReducer বা useContext ব্যবহার করতে পারেন ।
কোডের স্ট্রাকচার এবং প্রয়োজন ব্যাতিত কোন ধরনের লিখা, ছবি, রঙ, আইকন, সাইজ বা অন্য কোন কিছুর পরিবর্তন করতে পারবেন না ।
রিকুয়ারমেন্ট সেকশনে বলা বিষয় গুলো ব্যাতিত, "সামগ্রিক বিধিনিষেধ" সেকশনে বলা কোন বিষয় নিয়ে Discord এ প্রশ্ন করা যাবে না । বিশেষভাবে হাইজিন ফ্যাক্টর এবং আমরা যেই সমস্যা গুলো রেখেছি সে বিষয়ে জানতে চেয়ে কোন প্রশ্ন করা যাবে না ।

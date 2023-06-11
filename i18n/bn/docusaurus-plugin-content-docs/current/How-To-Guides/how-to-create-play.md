---
sidebar_position: 1
---

# কিভাবে একটি play তৈরি করবেন

স্বাগতম, ডেভেলপাররা! আমরা এটা জেনে খুবই উৎসাহিত যে আপনি একটি নতুন play তৈরি করতে যাচ্ছেন। এটা শুরু করা খুবই সহজ।

> **দ্রষ্টব্য:** নীচের ধাপগুলি বিবেচনা করে যে, আপনি আগেই [react-play](https://github.com/reactplay/react-play) রিপোজিটরিটি ফর্ক করে ক্লোন করেছেন এবং `npm install` অথবা `yarn install` কমান্ড ব্যবহার করে ডিপেন্ডেন্সিগুলি ইনস্টল করেছেন। ফর্কিং সম্পর্কে আপনি যদি নতুন হন, তবে শুরু করার জন্য এই [YouTube গাইড](https://www.youtube.com/watch?v=h8suY-Osn8Q) দেখুন।

- অ্যাপ্লিকেশনটি রান করার জন্য নিম্নলিখিত কমান্ড ব্যবহার করুন

  ```bash
  yarn start

  or

  npm run start
  ```

  যদি আপনি ডিপেন্ডেন্সি সম্পর্কিত কোনো সমস্যার সম্মুখীন হন, তবে নিম্নোক্ত কমান্ডটি ব্যবহার করতে পারেন:

  ```bash
  npm install --legacy-peer-deps
  ```

  বিস্তারিত জানতে [README](https://github.com/reactplay/react-play#readme) ফাইলটি চেক করতে পারেন।

- আপনি অ্যাপ্লিকেশনটি http://localhost:3000 এ অ্যাক্সেস করতে পারবেন।
- `Create` বাটনে ক্লিক করুন।

<p align="center">
  <img src="https://res.cloudinary.com/atapas/image/upload/v1675171492/ReactPlay/Screenshot_2023-01-31_at_6.43.49_PM_bkcvkv.png" alt="create-play" />
</p>

- অ্যাপ্লিকেশনটি আপনাকে অনুমোদন করতে চেষ্টা করবে
- আপনি যদি ইতিমধ্যে [`NHost`](https://nhost.io) এ লগ ইন না থাকেন, তবে আপনাকে অনুমতি দিতে বলা হবে
  - আপনার গিটহাব অ্যাকাউন্ট দিয়ে লগ ইন করুন
- তথ্য পূরণ করুন এবং জমা দিন।

<p align="center">
  <img src="https://res.cloudinary.com/atapas/image/upload/v1675171492/ReactPlay/Screenshot_2023-01-31_at_6.51.24_PM_ljc1hz.png" alt="create-play-fill-form"/>
</p>

প্যারামিটার

| ফিল্ড                   | বাধ্যতামূলক? | বিবরণ                                                                                                                                                                                                                                                                                                                                                                                                                           |
| ----------------------- | ------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| নাম                     | হ্যাঁ        | প্রতিটি play এর একটি নাম থাকা উচিত যা play এর ধারণার সাথে সম্পর্কিত।                                                                                                                                                                                                                                                                                                                                                            |
| ডেস্ক্রিপশন             | হ্যাঁ        | এটি প্লেয়ের বর্ণনা যাতে ব্যবহারকারীরা তা সহজে বোঝতে পারেন। অনুমোদিত অক্ষরের সর্বাধিক সংখ্যা হল 1024।                                                                                                                                                                                                                                                                                                                           |
| ইস্যু                   | হ্যাঁ        | প্লেটির সাথে একটি ইস্যু ম্যাপ করতে হবে। এখানে তা নির্বাচন করুন।                                                                                                                                                                                                                                                                                                                                                                 |
| ভাষা                    | হ্যাঁ        | অ্যাপ্লিকেশনটিকে জানান যে আপনার স্ক্রিপ্টের পছন্দ কি। এটি একটি **JavaScript** বা **TypeScript** সমর্থন করে। আপনি যেকোনটি চয়ন করতে পারেন।                                                                                                                                                                                                                                                                                       |
| স্টাইল                  | না           | অ্যাপ্লিকেশনটিকে জানান যে আপনার স্টাইলের পছন্দ কি। এটি একটি **css** বা **scss** সমর্থন করে। আপনি যেকোনটি চয়ন করতে পারেন।                                                                                                                                                                                                                                                                                                       |
| স্তর                    | না           | আপনার প্লেয়ের জন্য তিনটি স্তর মধ্যে একটি নির্বাচন করতে হবে, শুরুশব্দবিহীন, মধ্যম বা উন্নত। প্লেয়ের ডেভেলপমেন্টের সম্ভাব্য জটিলতার উপরে একটি স্তর নির্দেশ করে।                                                                                                                                                                                                                                                                 |
| Github ব্যবহারকারীর নাম | হ্যাঁ        | প্লেয় তৈরি করতে আপনার গিটহাব ব্যবহারকারীর নাম দিন যাতে আপনাকে প্লেয়ের সৃষ্টিকারী হিসাবে চিহ্নিত করা যায়।                                                                                                                                                                                                                                                                                                                     |
| ট্যাগ                   | না           | দয়া করে ট্যাগের কমা-বিভাজিত তালিকা প্রদান করুন। উদাহরণঃ JSX, Hooks                                                                                                                                                                                                                                                                                                                                                             |
| কভার ইমেজ URL           | না           | একটি কভার ইমেজ ব্যবহার করা হয় যাতে প্লেটি থাম্বনেল হিসাবে প্রদর্শিত হয়। দয়া করে পাবলিকভাবে অ্যাক্সেস যোগ্য একটি URL এর সাথে একটি লিঙ্ক সরবরাহ করুন, উদাহরণঃ https://res.cloudinary.com/reactplay/image/upload/v1649060528/demos/id-card_pdvyvz.png। আছেলে আপনার প্লেটির মূল ফোল্ডারে cover.png নামে একটি কভার ইমেজ থাকলে অ্যাপ্লিকেশনটি সেটি ব্যবহার করবে। কভার ইমেজ না থাকলে, অ্যাপ্লিকেশনটি ডিফল্ট কভার ইমেজ ব্যবহার করবে। |
| ব্লগ URL                | না           | যদি আপনি এই প্লেয়ের জন্য একটি লেখা লিখেছেন, তাহলে দয়া করে আপনার ব্লগ লেখার পৃষ্ঠার লিঙ্ক সরবরাহ করুন।                                                                                                                                                                                                                                                                                                                         |
| ভিডিও                   | না           | যদি আপনি এই প্লেয়ের জন্য একটি ভিডিও টিউটোরিয়াল তৈরি করেছেন, তাহলে দয়া করে আপনার YouTube ভিডিওর লিঙ্ক সরবরাহ করুন।                                                                                                                                                                                                                                                                                                            |
|                         |

- On successfull submission, you will be redirected to a page where it will prompt you with the `play_id`

<p align="center">
  <img src="https://res.cloudinary.com/atapas/image/upload/v1675172353/ReactPlay/Screenshot_2023-01-31_at_7.02.55_PM_k1tphu.png" alt="command" />
</p>

- Stop your application
- Navigate to the root of the reactplay
- Run following command

  ```bash
  npx create-react-play -c <the_play_id>
  ```

  **Note:** If the play folder `<reactplay_directory>/src/plays/<your_play_name>` remain empty after running above command that means you might be in some older version of the package. Use `@latest` in that case
  `bash
npx create-react-play@latest -c <the_play_id>
`
  <p align="center">
  <img src="https://res.cloudinary.com/atapas/image/upload/v1675172352/ReactPlay/Screenshot_2023-01-31_at_7.06.07_PM_jhbcbl.png" alt="copy-command" />
  </p>

- Start the application

  ```bash
  yarn start

  or

  npm run start
  ```

- You should now see your play added to the [play list](http://localhost:3000/plays) page.
<p align="center">
  <img src="https://res.cloudinary.com/atapas/image/upload/v1675172352/ReactPlay/Screenshot_2023-01-31_at_7.06.55_PM_gyck2r.png" alt="play" />
</p>

- You can click on the play thumbnail to see the details of the play.
<p align="center">
  <img src="https://res.cloudinary.com/atapas/image/upload/v1675172353/ReactPlay/Screenshot_2023-01-31_at_7.07.19_PM_dnmcuu.png" alt="play-details"/>
</p>

- And you will notice a directory created for your play under `./src/plays/<your_play_name>`
<p align="center">
  <img src="https://res.cloudinary.com/atapas/image/upload/v1675172514/ReactPlay/Screenshot_2023-01-31_at_7.10.36_PM_uxjomi.png" alt="code"/>
</p>

- Continue developing your play. Happy coding.

## 👀 Submitting a Play for Review

After you done with coding for your `Play`, you can submit it for review. Submitting a `Play` for review is a two step process.

- Create a Pull Request on the [react-play](https://github.com/reactplay/react-play) repository with your changes.
- Dedicate some time in a week to take care of the review comments.

Once the Pull Request is approved and merged, we will notify you and add you as a `Contributor` to the [react-play](https://github.com/reactplay/react-play) project.

## ✋ Need Help?

You can reach out to us at [ReactPlay Twitter Handle | @ReactPlayIO](https://twitter.com/ReactPlayIO) with a DM. Additionally, feel free to join our [Discord community](https://discord.gg/vrTxWUP8Am) for discussions.

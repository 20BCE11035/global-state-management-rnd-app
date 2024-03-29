# global-state-management-rnd-app
 [R&amp;D] Global State Management @bothrs  [[Chapter R&amp;D] Notion Docs](https://www.notion.so/bothrs/Global-State-Recoil-vs-Context-edeb6b7be3de49899b09a211efb673e9)  ### Table of contents.


# [R&D] Global State Management @bothrs

[[Chapter R&D] Notion Docs](https://www.notion.so/bothrs/Global-State-Recoil-vs-Context-edeb6b7be3de49899b09a211efb673e9)

### Table of contents

- [Global state management with **React Context**](#react-context) See [**[PR #1]**](https://github.com/bothrs/global-state-management-rnd/pull/1)
- [Global state management with **Recoil**](#recoil) See [**[PR #2]**](https://github.com/bothrs/global-state-management-rnd/pull/2)

### **What problem are we solving and why?**

we don't know which one brings the best developer experience, with the must pragmatic approach (giving us flexibility in different code bases)

### **What happens if we don't solve this problem**

We don't have a default when starting projects, leaving it up to the moment, and risking the stack diverging

## Global state with React Context <a name="react-context"></a>

[Official Docs -- React Context](https://reactjs.org/docs/context.html#when-to-use-context)  
[**[PR #1] React Context experiment**](https://github.com/bothrs/global-state-management-rnd/pull/1) -- [Vercel Preview](https://global-state-management-rnd-git-feat-ef14a2-aetherspace-digital.vercel.app/)  
- ✅ Official React API, not going anywhere in the future
- ✅ No extra concepts to learn if already familiar with React
- ✅ Actively maintained as part of React by Meta
- ✅ Often used under the hood by other state management libraries (optimised by them though)
- ✅ Automatically picked up out of the box by React Devtools
- 🤔 Still needs to be paired with other official React hooks to turn it into a state manager
- 🤔 Bare bones / “build your own solution” still leaves room for different interpretations
- 🤔 Can cause issues during SSR where server & browser state get out of sync
- 🤔 Context API can be slow at times, often requires memoization in large apps [Docs]
- 👍 Performance issues might get solved with React's new `useSelectedContext` hook

## Global state with Recoil <a name="recoil"></a>

[Official Docs -- Recoiljs.org](https://recoiljs.org/)  
[**[PR #2] React Context experiment**](https://github.com/bothrs/global-state-management-rnd/pull/2) -- [Vercel Preview](https://global-state-management-rnd-git-feat-1291dd-aetherspace-digital.vercel.app/)

- ✅ Straightforward DX, feels like using regular React state
- ✅ Separating read-only & read-write APIs
- ✅ Minimal overhead on top of normal hooks
- ✅ Isolates global state into atoms to avoid unnecessary / unrelated re-renders
- ✅ Promoted / maintained by (devs working for) Meta
- ✅ 269,471 weekly downloads [NPM]
- ✅ Actively maintained 👉 (bi-)weekly updates & releases [GitHub]
- 🤔 Not an official API though, might fall out of flavour / tank in popularity eventually

<br/>

---

<p>
  <a href="https://aetherspace-green-stack-starter.vercel.app/">
    <img alt="Supports Next.js" longdesc="Supports Next.js" src="https://img.shields.io/badge/Next-black?style=for-the-badge&logo=next.js&logoColor=white" />
  </a>
  <a href="https://aetherspace-green-stack-starter.vercel.app/">
    <img alt="Supports Vercel Deployments" longdesc="Supports Vercel Deployments" src="https://img.shields.io/badge/vercel-%23000000.svg?style=for-the-badge&logo=vercel&logoColor=white" />
  </a>
  <a href="https://aetherspace-green-stack-starter.netlify.app/">
    <img alt="Supports Netlify Deployments" longdesc="Supports Netlify Deployments" src="https://img.shields.io/badge/netlify-%23000000.svg?style=for-the-badge&logo=netlify&logoColor=#00C7B7" />
  </a>
  <a href="https://itunes.apple.com/app/apple-store/id982107779">
    <img alt="Test in Expo GO" longdesc="Test in Expo GO" src="https://img.shields.io/badge/expo-1C1E24?style=for-the-badge&logo=expo&logoColor=#D04A37" />
  </a>
  <a href="https://itunes.apple.com/app/apple-store/id982107779">
    <img alt="Supports Expo iOS" longdesc="Supports Expo iOS" src="https://img.shields.io/badge/iOS-4630EB.svg?style=for-the-badge&logo=APPLE&labelColor=999999&logoColor=fff" />
  </a>
  <a href="https://play.google.com/store/apps/details?id=host.exp.exponent&referrer=blankexample">
    <img alt="Supports Expo Android" longdesc="Supports Expo Android" src="https://img.shields.io/badge/Android-4630EB.svg?style=for-the-badge&logo=ANDROID&labelColor=A4C639&logoColor=fff" />
  </a>
  <a href="https://main--629ce63e5ac0810042889fc6.chromatic.com/?path=/story/readme-md--page">
    <img alt="Docs with Storybook" longdesc="Documentated with Storybook" src="https://img.shields.io/badge/-Storybook-FF4785?style=for-the-badge&logo=storybook&logoColor=fff" />
  </a>
</p>

> This project was bootstrapped with [Aetherspace](https://github.com/codinsonn/aetherspace-green-stack-starter), the Evergreen repo setup for all your full-stack cross platform app development needs \{...💚\} Enabling the project to be built for Web, iOS, Android, PWA, Static, SSR, REST and GraphQL all at once 👇

### Getting Started ⚡️

Install packages: `yarn install`

Run with docs: `yarn dev`

Run on web & mobile: `yarn dev-mobile`

---

<details>
  <summary><b>✅ Aetherspace, GREEN stack & Template Benefits? 🚀</b></summary>

---

# Aetherspace - GREEN stack starter template for cross platform React app development

### Table of contents

💚 - [What is the GREEN stack?](#what-is-the-green-stack)  
🚀 - [What is Aetherspace?](#what-is-aetherspace)  
🤖 - [Why start with a turbo/monorepo?](#why-turborepo)  
📁 - [File structure and installing new packages.](#package-management)  
👾 - [Benefits and next steps.](#benefits-next-steps)  
🤷‍♂️ - [When _not_ to use the GREEN stack.](#when-not-to-use-green-stack)  
📚 - [Relevant Docs.](#relevant-docs)

## What the hell is the GREEN stack? 💚 <a name="what-is-the-green-stack"></a>

In short GREEN stands for these 5 core technologies:

- **G**raphQL for typed and self documenting APIs
- **R**eact-Native and React-Native-Web for write-once UI
- **E**vergreen components that run anywhere (as well as Electron)
- **E**xpo for easy web + mobile dev, deploys and testing
- **N**ext.js for SEO, Static Exports, API, SSR & Web-Vitals

The core idea this tech stack enables you to achieve boils down to writing your app code or features once with Javascript and React, yet make it available on any platform or device without double implementations or the need for different development teams.

### It allows you to move fast, save time and deliver more 🎉

> Think of it as Unity for React Apps. Just like Unity aims to make cross console game development a lot easier for (indie) game devs, the GREEN stack aims to do the same for cross-platform app development.

## How does 'Aetherspace' help, exactly? 🚀 <a name="what-is-aetherspace"></a>

Aetherspace is an opinionated framework I've made that fills in the gaps of working and building with the GREEN stack:

- How should I handle responsive design?
- How do I avoid SSR layout shift when react-native styling does not support media queries or classnames?
- How can I expose / read public env vars across multiple platforms?
- Wait, how do I take advantage of next/image on the web when that's not available in React-Native?
- What's the best way to style and animate my UI elements for both web and mobile?

Just to name a few.

While the stack itself is very powerful, figuring out how to get set up and do certain things in a write-once way can be frustrating and time consuming. To save you time figuring it all out on your own, _Aetherspace_ contains a bunch of packages, utils and best-practices to set you up for a free and easy ride to cross-platform success.

> Aetherspace is also fully optional. Usage of the UI primitives, React hooks and JS utils provided by `packages/aetherspace` is recommended but not required.

> Provided you throw out the examples and edit some helper scripts in the `package.json` files, you could even delete the package entirely and still be left with a great GREEN stack starter.

More on Aetherspace in the **[👾 Benefits and Next steps](#benefits-next-steps)** section or `AETHERSPACE.md` and `CODEGEN.md`.

## But why start with a turbo/monorepo? 🤖 <a name="why-turborepo"></a>

One very annoying thing about figuring stuff out on your own is when packages you're using require custom configuration for webpack, babel or otherwise. It often happens that updating e.g. a single `babel.config.js` used for both React-Native and Next.js will fix usage on either, but then break the other.

Using a monorepo with different entry points for Next.js and Expo allows us to keep configs more seperate, and therefore allow more confident updating of packages and configs without accidentally breaking other platforms.

In this starter template, we've opted to use turborepo with yarn workspaces. We'll list some basics in the next section, but for a deeper understanding please refer to their documentation for more info.

## 📁 File structure and package management 📦 <a name="package-management"></a>

This starter monorepo has two types of workspaces:

- `/apps/*` for all expo & next.js versions of your apps
- `/packages/*` for all shared dependencies / library code used in multiple apps

```
├── apps/
│   └── {app-name}/ 👉 Where all cross-platform code for {app-name} lives
│       └── components/ ➡️ Molecules / Atoms / Common UI used in 'screens/'
│       └── graphql/ ➡️ Shared code for the GraphQL API client (optional)
│       └── resolvers/ ➡️ Shared resolvers used in both REST or GraphQL API
│       └── screens/ ➡️ Page templates used in App.tsx and next.js's 'pages/' directory
│       └── package.json ➡️ config required by yarn-workspaces, no dependencies
│
│   └── {app-name}-expo/ 👉 Where all Expo & mobile specific config for {app-name} lives
│       └── app.json ➡️ Expo app config (e.g. landscape / tablet support)
│       └── App.tsx ➡️ Mobile Entrypoint & Navigation Setup (using '{app-name}/screens/')
│       └── babel.config.js ➡️ Babel transpilation config for Expo
│       └── index.js ➡️ Mobile entrypoint loader for App.tsx
│       └── metro.config.js ➡️ Metro bundler config for react-native
│       └── package.json ➡️ yarn-workspace config, lists expo & non-next.js dependencies
│       └── tsconfig.json ➡️ Typescript config for Expo
│       └── webpack.config.js ➡️ Enables PWA browser testing with Expo (no SSR)
│
│   └── {app-name}-next/ 👉 Where all Next.js, Server & API config for {app-name} lives
│       └── public/ ➡️ favicon, app icons & other static assets (e.g. images & fonts)
│       └── src/
│           └── pages/ ➡️ directory based routes (using '{app-name}/screens/')
│               └── api/ ➡️ directory based api routes (using '{app-name}/resolvers/')
│                   └── graphql.ts ➡️ GraphQL client from '{app-name}/graphql/'
│               └── _app.tsx ➡️ App Layout Wrapper (e.g. headers / footers / navigation)
│               └── _document.tsx ➡️ HTML wrapper for head, body & meta tags (+ SSR styles)
│               └── index.tsx ➡️ Homepage (e.g. using '{app-name}/screens/HomeScreen.tsx')
│       └── babel.config.js ➡️ Babel transpilation config for Next.js
│       └── next.config.js ➡️ Next.js config, modules to transpile & plugins to support
│       └── package.json ➡️ yarn-workspaces config, lists ONLY next.js dependencies
│       └── tsconfig.json ➡️ Typescript config for Next.js
│
├── packages/
│   └── @aetherspace/ ➡️ Primitives, utils & helpers for working with the GREEN stack
│   └── @config/ ➡️ list of ts & other configs to use / extend from in next or expo apps
│   └── @scripts/ ➡️ scripts that help streamline things like codegen & managing assets
│   └── {comp-lib}/ 👉 Code shared across apps, ideally same structure as 'apps/{app-name}'
│       └── package.json ➡️ yarn-workspace config, doesn't need deps unless published
│
├── node_modules/ ➡️ Contains all modules for this monorepo
└── package.json  ➡️ Root yarn-workspaces configuration + helper scripts, no deps
```

```
💡 `{app-name}` & `{comp-lib}` are just placeholders and you **can** have multiple of these
```

#### 📦 Keep your apps seperate with `/apps/*` workspaces:

For every app you're building in this monorepo, you'll need a few folders:

- `/apps/app` - Where most of your app's UI, logic and Screens will live.
  Shouldn't have any dependencies.
- `/apps/app-next` - Entry for web where only next.js related config/setup for an app should live.
  Should list only next.js related dependencies & polyfills.
- `/apps/app-expo` - Entry for mobile where only expo related config/setup for an app should live.
  Should list all react(-native) and non next.js related dependencies.

In each of these folders own `package.json` file, a `name` property should be specified to identify that workspace. This name can then be referenced during installs via e.g.

```bash
yarn workspace app-next add next-images
```

```bash
yarn workspace app-expo add moti
```

> It's also advised to see app workspaces as fully seperate from other apps:

> For example, `/apps/app` should not import or reference anything from `/apps/some-other-app`. If you do need to embed a certain screen or component from one app in another, it's best to extract it to its own shared library workspace instead (toggle below for info 👇)

<details>
<summary>💡 `/packages/*` workspaces for e.g. component libraries</summary>

#### Write shared library code in `/packages/*` workspaces:

Packages aim to provide common building blocks or logic for both apps _and_ other packages. They do not need to differentiate between entry points with `/packages/...-next` and `/packages/...-expo`.

Like `/apps/` workspaces, they do also require their own `package.json` and `name`, and installing dependencies can work exactly the same:

```bash
yarn workspace component-library add -D @types/react
```

However, unless you will be publishing the package to NPM, it may be best to just install any dependencies in the consuming apps' `/apps/{app-name}-next` or `/apps/{app-name}-expo` workspace instead.

> A good example of a library package usable by multiple app workspaces in this monorepo is the
> `/packages/aetherspace` workspace. It contains UI primitives like `AetherView`, `AetherImage` & `AetherLink` that are small wrappers for & recommended over react-native's own `View`, `Text` & `Image` components.

</details>

## 👾 Stack and Template benefits + Next steps 👾 <a name="benefits-next-steps"></a>

If you've read the sections above, It's likely the **ease** of use, **time saving** capabilities and **scalability** of this stack & template are clear.

The starter repo comes with some opinionated extra packages and abilities.  
Here's a list of what you can start doing out of the box:

- Link pages and screens cross platform with `expo-next-react-navigation` or `<AetherLink>`
- Use tailwind to style UI responsively on web / mobile with `<AetherView tw="sm:px-2">` / `tailwind-rn`
- Animate UI elements with `<AetherView.Animated>` / `react-native-reanimated` / `moti`
- Add illustrations or icons with `react-native-svg`
- Bring the power of GraphQL to JSON or REST apis with `aetherResolver()` and Schemas.
- Add auth with [AuthSession](https://docs.expo.dev/versions/latest/sdk/auth-session/) ([Expo Examples](https://docs.expo.dev/guides/authentication/))
- Document your components and APIs with Storybook.
- Deploy to vercel with `yarn deploy` or `vercel --prod --no-clipboard` ([view live](https://aetherspace-green-stack-starter.vercel.app/))
- Deploy to netlify [via this guide](https://www.netlify.com/blog/2020/11/30/how-to-deploy-next.js-sites-to-netlify/) ([view live](https://aetherspace-green-stack-starter.netlify.app/))

If you'd like to continue learning about Aetherspace and the GREEN stack, there are more detailed guides, tips and best-practices in:

- `AETHERSPACE.md`, `CODEGEN.md`, `NAVIGATION.md` & `API.md` (Aetherspace & Codegen)
- `STYLING.md`, `ANIMATING.md` & `DOCUMENTING.md` (GREEN stack How-tos)

## 💼 Why this makes sense from a business perspective 💸 <a name="why-this-makes-sense-from-a-business-perspective"></a>

Whether you're a startup or established company, having both web and mobile apps is a great competitive advantage. There are many stories of market leaders suddenly being overtaken because the competition were able to move faster or had more devices their solution was available on for their customers.

This stack makes it near effortless to enable extra platforms. It helps keep teams small and enables them to move fast when building new pages or features for phones, tablets and/or the web.

**More deliverables for less time invested in turn means flexibility in one or more of these areas:**

- ... negotiation room about budget or deadlines (in case of client work)
- ... 💰 to be distributed among the entire team
- ... 🕗 available for experimentation
- ... budget available to market the product

<details>
<summary>Show full 🕗🕗 to 💰💰💰 Comparison</summary>

---

Let's talk Return on Investment:

> 🕗 = time required = devs / teams / resources invested  
> 💰 = deliverable sale value = costs to build + profit margin  
> ROI = 🕗 -> _sold for_ -> 💰

Web only project ROI = 🕗🕗 -> 💰💰

- 🕗 Web Front-End 💰
- 🕗 General Back-End (REST / GraphQL + Templates / SSR) 💰

Native iOS + Android project ROI = 🕗🕗🕗 -> 💰💰💰

- 🕗 iOS App with Swift 💰
- 🕗 Android app with Java 💰
- 🕗 API Back-End (REST / GraphQL) 💰

React-Native Mobile App ROI = 🕗🕗 -> 💰💰 to 💰💰💰

- 🕗 iOS + Android App with RN 💰(💰)
- 🕗 API Back-End (REST / GraphQL) 💰

Expo Mobile + PWA ROI = 🕗🕗 ->💰💰 to 💰💰💰💰

- 🕗 iOS + Android + PWA with Expo & RN (Web without SSR) 💰(💰💰)
- 🕗 API Back-End (REST / GraphQL) 💰

> Now, things get _really_ interesting when you try to compare full cross-platform apps

Full Cross Platform with Separate Dev Teams ROI = 🕗🕗🕗🕗🕗🕗🕗 -> 💰💰💰💰💰💰💰

- 🕗 Web Front-End 💰
- 🕗 iOS App with Swift 💰
- 🕗 Android app with Java 💰
- 🕗 Windows App Dev Team 💰
- 🕗 MacOS App Dev Team 💰
- 🕗 Linux App Dev Team 💰
- 🕗 API Back-End (REST / GraphQL) 💰

Full Cross Platform with GREEN stack ROI = 🕗🕗 -> 💰💰 to 💰💰💰💰💰💰💰

- 🕗 Web (PWA & SSR & Web Vitals) + iOS + Android + Windows + MacOS + Linux 💰(💰💰💰💰💰)
- 🕗 Back-End (REST + GraphQL + SSR + Static Exports + ISSG + universal JS utils thanks to Next.js) 💰

#### Key takeaway: Always upsell more plaforms / devices the app could run on

---

</details>

## When not to use the GREEN stack? 🤷‍♂️ <a name="when-not-to-use-green-stack"></a>

The GREEN stack is unlikely to be the best fit when your project...

- ... will always be web only 👉 Use `next.js`
- ... will always be mobile only 👉 Use `Expo`
- ... will always be desktop only 👉 Use `Electron` + `React` / `Vue` / `Svelte`
- ... is very Bluetooth / AR / VR / XR heavy 👉 Go native with `Swift` / `Java`
- ... is a console game 👉 Use [`Unity`](https://unity.com/download) instead
- ... is not using React 👉 Use `Svelte` / `Vue` + `Ionic`
- ... has no real need for Server Rendering, SEO or Web-Vitals 👉 Use `Expo` (+ Web Support)
- ... is using React, but the project is too far along and has no budget, time or people to refactor 🤷‍♂️

If your project has required dependencies / SDKs / libraries that are either not available in JS, are not extractable to API calls or cannot function cross-platform, this may also not be a good solution for your use-case\*.

```
🛠 * However, for JS libs, you could always try adding cross platform support yourself with `patch-package`
```

## 📚 Relevant docs: <a name="relevant-docs"></a>

- [Yan Workspaces Docs](https://classic.yarnpkg.com/lang/en/docs/workspaces/)
- [Turborepo Docs](https://turborepo.org/docs)
- [Expo Docs](https://docs.expo.dev/)
- [Next.js Docs](https://nextjs.org/docs/getting-started)
- [React Native Docs](https://reactnative.dev/docs/getting-started)
- [React Navigation Docs](https://reactnavigation.org/docs/getting-started)
- [React-Native-Web Docs](https://necolas.github.io/react-native-web/docs/)
- [Apollo GraphQL Docs](https://www.apollographql.com/docs/)
- [Reanimated Docs](https://docs.swmansion.com/react-native-reanimated/docs)
- [Moti Docs](https://moti.fyi/)

</details>

---

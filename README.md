> :partying_face: TurboStrapi is now ready to use!

# TurboStrapi: The Strapi & Next.js Monorepo Starter

![TurboStrapi](https://github-production-user-asset-6210df.s3.amazonaws.com/36924392/277128068-6fc3f7df-0e57-45be-bf3c-90b2c0f6e646.gif)

TurboStrapi is not just another starter. It's your gateway to seamless web development, combining the powers of **Strapi**, **Next.js**, and **Turborepo** in a monorepo setup. Unleash your creativity and scale with ease!

## 📦 Stack

- **[Strapi](https://strapi.io/)**: Handle your content like never before.
- **[Next.js 14](https://nextjs.org/)**: For a blazing fast frontend experience.
- **[Turborepo](https://turbo.build/repo)**: Efficient monorepo management to keep things tidy.
- **[Tailwind CSS](https://tailwindcss.com/)**: Awesome utility-first CSS framework.

## ✨ Features

Discover the pre-configured goodies TurboStrapi brings to your table:

- 🧩 **Strapi**: Fully typed with basic content-types.
- 🔥 **Next.js 14**: Already connected to Strapi via an API service.
- 💼 **Turborepo**: Pre-configured, ready to go.
- 🎨 **Tailwind CSS**: Shared configuration ensuring consistent styles.
- 🌐 **Localization**: Multi-language Content support pre-configured.
- 🎡 **CVA & tailwind-merge**: Tailwind variants made easy.
- 🛠️ **Code Quality**: Out-of-the-box ESLint, Prettier, and TypeScript.
- 🚧📦 **Sample DB Seed**: Import demo data for a quick setup.
- 🚧🧪 **100% Test Coverage**: All implemented features are fully tested.

  > 🚧 WIP: Stay tuned!

## 🚀 Get Up and Running

1. **Grab the Code**

   ```bash
   git clone https://github.com/sawden/turbostrapi.git
   ```

2. **Setup Environment**

   Copy the example .env and adjust the variables:

   ```bash
   cp .env.example .env
   ```

   > The `.env` file at the root handles environment variables across all workspaces.

3. **Set Things Up**

   ```bash
   yarn
   ```

4. **Launch**

   Light up both Strapi and Next.js:

   ```bash
   yarn dev
   ```

5. **Witness Magic**

   Visit frontend [http://localhost:3000](http://localhost:3000) and backend [http://localhost:1337](http://localhost:1337).

6. **Read the Docs**

   Each workspace has its own `README.md` — Take a look before you start:

   - [Backend](apps/backend/README.md)
   - [Frontend](apps/frontend/README.md)

## 🗂️ Project Structure

```
root/
│
├── apps/
│   ├── backend/             ℹ️ Strapi Workspace
│   └── frontend/            ℹ️ Next.js Workspace
│
├── configs/
│   ├── tailwind-config/     ℹ️ Shared Tailwind Configuration
│   ├── eslint-config/       ℹ️ ESLint Configurations
│   └── ...
│
├── packages/
│   ├── cva/                 ℹ️ CVA setup with tailwind-merge
│   └── ui/                  ℹ️ React UI Library
│
├── turbo.json
├── README.md
└── ...
```

> This starter uses `@turbostrapi` as the package namespace. You can easily replace it globally through search and replace with a namespace of your choice.

## 🏎️ Remote Caching

Turborepo can use a technique known as [Remote Caching](https://turbo.build/repo/docs/core-concepts/remote-caching) to share cache artifacts across machines, enabling you to share build caches with your team and CI/CD pipelines.

By default, Turborepo will cache locally. To enable Remote Caching you will need an account with Vercel. If you don't have an account you can [create one](https://vercel.com/signup), then enter the following commands:

```
npx turbo login
```

This will authenticate the Turborepo CLI with your [Vercel account](https://vercel.com/docs/concepts/personal-accounts/overview).

Next, you can link your Turborepo to your Remote Cache by running the following command from the root of your Turborepo:

```
npx turbo link
```

## 💡 Contribute

TurboStrapi is better with your input. Got an enhancement or a bugfix? Dive in:

1. Fork it.
2. Create your feature branch.
3. Commit your changes.
4. Push to the branch.
5. Create a new Pull Request.

## 📄 Legalese

TurboStrapi is open-source and available under the MIT License. Dive into the [LICENSE](./LICENSE) for more details.

## Useful Links

- [strapi](https://github.com/strapi/strapi)
- [Turbo](https://github.com/vercel/turbo)
- [Next.js](https://github.com/vercel/next.js)
- [shadcn/ui](https://github.com/shadcn-ui/ui)
- [tailwindcss](https://github.com/tailwindlabs/tailwindcss)
- [heroicons](https://github.com/tailwindlabs/heroicons)

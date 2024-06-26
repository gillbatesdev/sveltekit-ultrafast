# sveltekit-ultrafast ⚡️

The `sveltekit-ultrafast` is a boilerplate for rapid prototyping of web applications which is easily deployable to Vercel or other effortless platforms.

## Why sveltekit-ultrafast?

⚡️ super fast application development

💸 effortless, cheap (or even free) deployment & maintenance

🧪 quick prototype = fast reitaration = quick idea validation

💨 highly performant app (Svelte drastically faster than React)

❤️‍🔥 developer-friendly, pleasant stack

---

With this boilerplate you can create (and effortlessly deploy) a fully-functioning MVP for which you can charge $ within days or even hours (depends on the idea).

Why waste more time on creating something no one will use and purchase?

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2Fgillbatesdev%2Fsveltekit-ultrafast)

## Contribution guide

In case you have any suggestions, feel free to create an issue on this repository or create a pull request for the changes that you'd like to see.

Also, if you love this work and it helped you make money, you can follow me on [Twitter](https://x.com/gillbatesdev) for more. And, please, share your story! I'd love to hear success/failure stories about your apps.

## Documentation

Each of the features have a `docs.md` file with setup guide:

- **blog**: `src/routes/blog/docs.md`
- **auth**: `src/routes/auth/docs.md`
- **analytics**: `src/routes/analytics/docs.md`
- **database**: `src/routes/database-example/docs.md`
- **payment**: `src/routes/payment/docs.md`

Additionally, documentation can be found here: [sveltekit-ultrafast.com/docs](https://sveltekit-ultrafast.com/docs).

---

## Technologies

### Main

- **TypeScript** (optional) - you can use TypeScript (recommended for type safety), but you don't have to; no errors will be thrown if you use both JavaScript and TypeScript in this app
- **SvelteKit** - fastest, easiest, cleanest front-end framework with SSR

### Styling

- **Tailwind CSS** - definitely fastest for rapid prototyping
- **DaisyUI** - most popular UI kit for Tailwind CSS, great components and nice UI
- **Custom UI component** - I've included `/lib/components/common` directory with "component wrappers" for DaisyUI which makes it really easy to modify the components globally; also, their design and functionality is being improved

### Database

For database, we use [Supabase](https://supabase.com/database) which provides hussle-free ways of utilizing PostgreSQL databases into web apps.

### Payments

Using Stripe for handling payments - most effortless to set up, it literally takes 5 minutes.

--

## Setup

### 1. Adjust prettier/eslint settings (optional)

If the prefer a different prettier/eslint configuration, feel free to adjust it:

- `.eslintrc.cjs` to update all the eslint rules
- `.prettierrc` for all the prettier code formatting rules

### 2. Update VSCode settings for optimal development experience (recommended)

Paste this in your `settings.json` in VSCode:

```JSON
  "editor.formatOnSave": true,
  "prettier.documentSelectors": ["**/*.svelte"],
  "[svelte]": {
    "editor.defaultFormatter": "svelte.svelte-vscode",
    "editor.formatOnSave": true
  },
```

This will automatically take care of the Prettier formatting based on the specified `.prettierrc` configuration.
This will make sure that all the code throughout your application is properly formatted so that you don't have to worry about that and make the entire development process much faster.

### 3. Install all the dependencies

Run `npm i` when in the `sveltekit-asap-boilerplate` directory.

### 4. Create a supabase project

Register your project on [Supabase](https://supabase.com/) if you plan to have authentication & database-related features.

Create an `.env` file and fill this with: `SUPABASE_PROJECT_URL, SUPABASE_PROJECT_API_KEY` which you can easily get after you create a free project on Supabase.

### 5. Next steps

Depending on your list of features, you can follow the `docs.md` files in each of the `/routes` directory or the [docs page](https://sveltekit-ultrafast.com/docs) to get started with this boilerplate.

### 6. Add your favicon

You can either add `favicon.[svg/png]` in your `static` directory and then add:

```HTML
<link rel="icon" href="%sveltekit.assets%favicon.png" />
```

or, for simplicity, you can replace the current emoji to set the emoji of your choice as your favicon.

```HTML
<link
    rel="icon"
    href="data:image/svg+xml,<svg xmlns=%22http://www.w3.org/2000/svg%22 viewBox=%220 0 100 100%22><text y=%22.9em%22 font-size=%2290%22>{PASTE YOUR EMOJI HERE}</text></svg>" />
```

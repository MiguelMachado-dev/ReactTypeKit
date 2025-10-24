# ReactTypeKit — Zed Snippets for React + TypeScript

![Dynamic JSON Badge](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fraw.githubusercontent.com%2FMiguelMachado-dev%2FReactTypeKit%2Fmain%2Fdownloads.json&query=downloads&style=for-the-badge&label=Downloads%20%40%20Zed&labelColor=%23181825&color=%23cba6f7)

A curated collection of Zed editor snippets to speed up React development in TypeScript: components, hooks, context, Redux Toolkit patterns, and more.

## 🚀 Features

* Snippets for functional components (arrow & function style)
* Typed `useState`, `useEffect`, `useMemo`, `useCallback`, `useReducer`, etc.
* ForwardRef components
* Custom hook template
* React Context boilerplate with provider + hook
* Redux Toolkit slice, store, typed hooks
* Interface / type / enum helpers

All built assuming you write React in TypeScript, so you get strong typing and consistent patterns.

## 📦 Installation (Zed)

1. Copy the snippet file (e.g. `react-ts-snippets.json` or `.zed-snippets`) into your Zed snippets folder
2. Restart Zed or reload snippets
3. Start using — e.g. type `rfc` to scaffold a typed functional component

*(If Zed supports publishing an extension, you can package this and install via marketplace.)*

## 🧰 Snippet Usage

Here are some sample prefixes and what they expand into:

| Prefix        | Expands Into                                    | Description                             |
| ------------- | ----------------------------------------------- | --------------------------------------- |
| `rfc`         | Arrow functional component with props interface | A modern component template             |
| `rff`         | Function-style component                        | Alternate component syntax              |
| `us`          | `useState<…>` boilerplate                       | Typed state hook                        |
| `uem`         | `useEffect(() => { … }, [])`                    | Effect that runs once on mount          |
| `useCallback` | `useCallback(() => { … }, [deps])`              | Memoized callback                       |
| `rctx`        | Context + Provider + custom hook boilerplate    | Setup for React Context in TS           |
| `rtslice`     | Redux Toolkit slice                             | Boilerplate for slices                  |
| `rtth`        | Typed Redux hooks                               | `useAppSelector`, `useAppDispatch` etc. |

> You can inspect the full snippet definitions (triggering texts, placeholders, etc.) inside the extension file.

## 📄 Example

Typing:

```
rfc
```

Might expand to:

```ts
interface MyComponentProps {
  title: string;
}

const MyComponent = ({ title }: MyComponentProps) => {
  return (
    <div>
      {title}
    </div>
  );
};

export default MyComponent;
```

Then you can tab through placeholders to rename component, props, types, etc.

## 💡 Tips & Customization

* You can rename or adjust snippet names/prefixes to match your coding style.
* Add your own snippet variations (e.g. for styled-components, Tailwind, etc.).
* Use snippet placeholders and tab stops to efficiently navigate through your template when inserted.
* Keep the file organized: group similar snippets together, and document custom ones.

## 📝 Acknowledgments & License

This extension is inspired by the Zed React TS snippets by [vishnuroshan](https://github.com/vishnuroshan/zed-react-ts-snippets).
You’re free to use, modify, and distribute — include your preferred license (MIT, Apache, etc.).

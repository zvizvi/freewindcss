# Freewind CSS

Use Tailwind's set values and units without installing Tailwind.

Bring the conventional units prepared by Tailwind in the usual way of writing CSS.

## Installation

Install with npm:

```shell
npm install freewindcss
```

Install with yarn:

```shell
yarn add freewindcss
```

## Examples

```scss
.element {
  width: var(--fw-4); // 1rem
  height: var(--fw-2); // 0.5rem
  margin: 0 auto var(--fw-2); // 0 auto 0.5rem
  font-size: var(--fw-text-sm); // 0.875rem
  line-height: var(--fw-leading-relaxed); // 1.625
  font-weight: var(--fw-font-thin); // 100
  background: var(--fw-indigo-400); // rgb(129, 140, 248)
  border-radius: var(--fw-rounded-md); // 0.375rem
  box-shadow: var(--fw-shadow-sm); // 0 1px 2px 0 rgb(0 0 0 / 0.05)
  transition: var(--fw-ease-in-out); // cubic-bezier(0.4, 0, 0.2, 1)
}
```

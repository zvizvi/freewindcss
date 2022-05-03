# 🍃 Freewind CSS

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

#### See a live demo on [Codesandbox.io](https://codesandbox.io/s/freewindcss-pfq17e)

## Documentation


<details open>
<summary>Index</summary>

- [Sizing and Spacing](#sizing-and-spacing)
  - [Negative sizing values](#negative-sizing-and-spacing-values)
- [Font Family](#font-family)
- [Font Size](#font-size)
- [Font Weight](#font-weight)
- [Letter Spacing](#letter-spacing)
- [Line Height](#line-height)
- [Border Radius](#border-radius)
- [Box Shadow](#box-shadow)
- [Blur Filter](#blur-filter)
- [Drop Shadow](#drop-shadow)
- [Columns](#columns)
- [Transition Timing](#transition-timing)
- [Colors](#colors)
  - [Colors transparency (alpha)](#color-opacity)
- [Animations](#animations)
- [Container Width](#container-width)
</details>


### Sizing and Spacing
#### Useful with the following properties; `margin`, `padding`, `height`, `width`, `top`, `right`, `bottom`, `left` Etc. for example:
```scss
element {
  right: var(--fw-2); // 8px
  width: var(--fw-10); // 40px
  padding: var(--fw-2) var(--fw-4); // 8px 16px
}
```

<details open>
<summary>Variables</summary>

```css
--fw-auto: auto;        // auto
--fw-full: 100%;        // 100%
--fw-0: 0;              // 0px
--fw-0\5: 0.125rem;     // 2px
--fw-1: 0.25rem;        // 4px
--fw-1\5: 0.375rem;     // 6px
--fw-2: 0.5rem;         // 8px
--fw-2\5: 0.625rem;     // 10px
--fw-3: 0.75rem;        // 12px
--fw-3\5: 0.875rem;     // 14px
--fw-4: 1rem;           // 16px
--fw-4\5: 1.125rem;     // 18px
--fw-5: 1.25rem;        // 20px
--fw-6: 1.5rem;         // 24px
--fw-7: 1.75rem;        // 28px
--fw-8: 2rem;           // 32px
--fw-9: 2.25rem;        // 36px
--fw-10: 2.5rem;        // 40px
--fw-11: 2.75rem;       // 44px
--fw-12: 3rem;          // 48px
--fw-13: 3.25rem;       // 52px
--fw-14: 3.5rem;        // 56px
--fw-15: 3.75rem;       // 60px
--fw-16: 4rem;          // 64px
--fw-17: 4.25rem;       // 68px
--fw-18: 4.5rem;        // 72px
--fw-19: 4.75rem;       // 76px
--fw-20: 5rem;          // 80px
--fw-24: 6rem;          // 96px
--fw-28: 7rem;          // 112px
--fw-32: 8rem;          // 128px
--fw-36: 9rem;          // 144px
--fw-40: 10rem;         // 160px
--fw-44: 11rem;         // 176px
--fw-48: 12rem;         // 192px
--fw-52: 13rem;         // 208px
--fw-56: 14rem;         // 224px
--fw-60: 15rem;         // 240px
--fw-64: 16rem;         // 256px
--fw-72: 18rem;         // 288px
--fw-80: 20rem;         // 320px
--fw-96: 24rem;         // 384px
```
</details>

#### Negative sizing and spacing values
For negative size values just use the previous variables with a double - before the variable id:
`--fw--1`, `--wf--1\5`, `--wf--full` and so on.

### Font Family
#### Can be used with the `font-family` property, for example:
```scss
element {
  font-family: var(--fw-font-serif); // ui-serif, Georgia, Cambria, "Times New Roman", Times, serif
}
```

<details open>
<summary>Variables</summary>

```scss
--fw-font-sans: ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, "Noto Sans", sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji";
--fw-font-serif: ui-serif, Georgia, Cambria, "Times New Roman", Times, serif;
--fw-font-mono: ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, "Liberation Mono", "Courier New", monospace;
```
</details>

### Font Size
#### Can be used with the `font-size` property, for example:
```scss
element {
  font-size: var(--fw-text-2xl); // 1.5rem
}
```

<details open>
<summary>Variables</summary>

```scss
--fw-text-xs: 0.75rem;
--fw-text-sm: 0.875rem;
--fw-text-base: 1rem;
--fw-text-lg: 1.125rem;
--fw-text-xl: 1.25rem;
--fw-text-2xl: 1.5rem;
--fw-text-3xl: 1.875rem;
--fw-text-4xl: 2.25rem;
--fw-text-5xl: 3rem;
--fw-text-6xl: 4rem;
```
</details>

### Font Weight
#### For example:
```scss
element {
  font-weight: var(--fw-font-semibold); // 600
}
```

<details open>
<summary>Variables</summary>

```scss
--fw-font-thin: 100;
--fw-font-extralight: 200;
--fw-font-light: 300;
--fw-font-normal: 400;
--fw-font-medium: 500;
--fw-font-semibold: 600;
--fw-font-bold: 700;
--fw-font-extrabold: 800;
--fw-font-black: 900;
```
</details>

### Letter Spacing
#### Using with `letter-spacing` property, for example:
```scss
element {
  letter-spacing: var(--fw-tracking-tight); // -0.025em
}
```

<details open>
<summary>Variables</summary>

```scss
--fw-tracking-tighter: -0.05em;
--fw-tracking-tight: -0.025em;
--fw-tracking-normal: 0;
--fw-tracking-wide: 0.025em;
--fw-tracking-wider: 0.05em;
--fw-tracking-widest: 0.1em;
```
</details>

### Line Height
#### Used with `line-height` property, for example:
```scss
element {
  line-height: var(--fw-leading-5); // 20px
}
```

<details open>
<summary>Variables</summary>

```scss
--fw-leading-3: 0.75rem; // 12px
--fw-leading-4: 1rem;    // 16px
--fw-leading-5: 1.25rem; // 20px
--fw-leading-6: 1.5rem;  // 24px
--fw-leading-7: 1.75rem; // 28px
--fw-leading-8: 2rem;    // 32px
--fw-leading-9: 2.25rem; // 36px
--fw-leading-10: 2.5rem; // 40px
--fw-leading-none: 1;
--fw-leading-tight: 1.25;
--fw-leading-snug: 1.375;
--fw-leading-normal: 1.5;
--fw-leading-relaxed: 1.625;
--fw-leading-loose: 2;
```
</details>

### Border Radius
#### For example:
```scss
element {
  border-radius: var(--fw-rounded-md); // 6px
}
```

<details open>
<summary>Variables</summary>

```scss
--fw-rounded-none: 0px;      // 0px
--fw-rounded-sm: 0.125rem;   // 2px
--fw-rounded: 0.25rem;       // 4px
--fw-rounded-md: 0.375rem;   // 6px
--fw-rounded-lg: 0.5rem;     // 8px
--fw-rounded-xl: 0.75rem;    // 12px
--fw-rounded-2xl: 1rem;      // 16px
--fw-rounded-3xl: 1.5rem;    // 24px
--fw-rounded-full: 9999px;   // 9999px
```
</details>

### Box Shadow
#### For example:
```scss
element {
  box-shadow: var(--fw-shadow-lg); // 0 10px 15px -3px rgb(0 0 0 / 0.1), 0 4px 6px -4px rgb(0 0 0 / 0.1)
}
```

<details open>
<summary>Variables</summary>

```scss
--fw-shadow-sm: 0 1px 2px 0 rgb(0 0 0 / 0.05);
--fw-shadow: 0 1px 3px 0 rgb(0 0 0 / 0.1), 0 1px 2px -1px rgb(0 0 0 / 0.1);
--fw-shadow-md: 0 4px 6px -1px rgb(0 0 0 / 0.1), 0 2px 4px -2px rgb(0 0 0 / 0.1);
--fw-shadow-lg: 0 10px 15px -3px rgb(0 0 0 / 0.1), 0 4px 6px -4px rgb(0 0 0 / 0.1);
--fw-shadow-xl: 0 20px 25px -5px rgb(0 0 0 / 0.1), 0 8px 10px -6px rgb(0 0 0 / 0.1);
--fw-shadow-2xl: 0 25px 50px -12px rgb(0 0 0 / 0.25);
--fw-shadow-inner: inset 0 2px 4px 0 rgb(0 0 0 / 0.05);
--fw-shadow-none: 0 0 #0000;
```
</details>

### Blur Filter
#### Used with `filter: blur(x)` or with `  backdrop-filter: blur(x)`, for example:
```scss
element {
  backdrop-filter: var(--fw-blur-md); // blur(12px)
}
```

<details open>
<summary>Variables</summary>

```scss
--fw-blur-none: blur(0);
--fw-blur-sm: blur(4px);
--fw-blur: blur(8px);
--fw-blur-md: blur(12px);
--fw-blur-lg: blur(16px);
--fw-blur-xl: blur(24px);
--fw-blur-2xl: blur(40px);
--fw-blur-3xl: blur(64px);
```
</details>

### Drop Shadow
#### Used with `filter: drop-shadow(x)`, for example:
```scss
element {
  filter: var(--fw-drop-shadow-sm); // drop-shadow(0 1px 1px rgb(0 0 0 / 0.05))
}
```

<details open>
<summary>Variables</summary>

```scss
--fw-drop-shadow-sm: drop-shadow(0 1px 1px rgb(0 0 0 / 0.05));
--fw-drop-shadow: drop-shadow(0 1px 2px rgb(0 0 0 / 0.1)) drop-shadow(0 1px 1px rgb(0 0 0 / 0.06));
--fw-drop-shadow-md: drop-shadow(0 4px 3px rgb(0 0 0 / 0.07)) drop-shadow(0 2px 2px rgb(0 0 0 / 0.06));
--fw-drop-shadow-lg: drop-shadow(0 10px 8px rgb(0 0 0 / 0.04)) drop-shadow(0 4px 3px rgb(0 0 0 / 0.1));
--fw-drop-shadow-xl: drop-shadow(0 20px 13px rgb(0 0 0 / 0.03)) drop-shadow(0 8px 5px rgb(0 0 0 / 0.08));
--fw-drop-shadow-2xl: drop-shadow(0 25px 25px rgb(0 0 0 / 0.15));
--fw-drop-shadow-none: drop-shadow(0 0 #0000);
```
</details>

### Columns
#### example:
```scss
element {
  columns: var(--fw-columns-3xl); // 768px
}
```

<details open>
<summary>Variables</summary>

```scss
--fw-columns-3xs: 16rem; // 256px
--fw-columns-2xs: 18rem; // 288px
--fw-columns-xs: 20rem;  // 320px
--fw-columns-sm: 24rem;  // 384px
--fw-columns-md: 28rem;  // 448px
--fw-columns-lg: 32rem;  // 512px
--fw-columns-xl: 36rem;  // 576px
--fw-columns-2xl: 42rem; // 672px
--fw-columns-3xl: 48rem; // 768px
--fw-columns-4xl: 56rem; // 896px
--fw-columns-5xl: 64rem; // 1024px
--fw-columns-6xl: 72rem; // 1152px
--fw-columns-7xl: 80rem; // 1280px
```
</details>

### Transition Timing
#### example:
```scss
element {
  transition-timing-function: var(--fw-ease-out); // cubic-bezier(0, 0, 0.2, 1)
}
```

<details open>
<summary>Variables</summary>

```scss
--fw-ease-linear: linear;
--fw-ease-in: cubic-bezier(0.4, 0, 1, 1);
--fw-ease-out: cubic-bezier(0, 0, 0.2, 1);
--fw-ease-in-out: cubic-bezier(0.4, 0, 0.2, 1);
```
</details>

### Colors
#### example:
```scss
element {
  color: var(--fw-slate-100); // rgb(241 245 249)
  background: var(--fw-fuchsia-500); // rgb(217 70 239)
}
```

<details open>
<summary>Variables</summary>

```clojure
--fw-black: rgb(0 0 0);             // #000000
--fw-white: rgb(255 255 255);       // #ffffff
--fw-slate-50: rgb(248 250 252);    // #f8fafc
--fw-slate-100: rgb(241 245 249);   // #f1f5f9
--fw-slate-200: rgb(226 232 240);   // #e2e8f0
--fw-slate-300: rgb(203 213 225);   // #cbd5e1
--fw-slate-400: rgb(148 163 184);   // #94a3b8
--fw-slate-500: rgb(100 116 139);   // #64748b
--fw-slate-600: rgb(71 85 105);     // #475569
--fw-slate-700: rgb(51 65 85);      // #334155
--fw-slate-800: rgb(30 41 59);      // #1e293b
--fw-slate-900: rgb(15 23 42);      // #0f172a
--fw-gray-50: rgb(249 250 251);     // #f9fafb
--fw-gray-100: rgb(243 244 246);    // #f3f4f6
--fw-gray-200: rgb(229 231 235);    // #e5e7eb
--fw-gray-300: rgb(209 213 219);    // #d1d5db
--fw-gray-400: rgb(156 163 175);    // #9ca3af
--fw-gray-500: rgb(107 114 128);    // #6b7280
--fw-gray-600: rgb(75 85 99);       // #4b5563
--fw-gray-700: rgb(55 65 81);       // #374151
--fw-gray-800: rgb(31 41 55);       // #1f2937
--fw-gray-900: rgb(17 24 39);       // #111827
--fw-zinc-50: rgb(250 250 250);     // #fafafa
--fw-zinc-100: rgb(244 244 245);    // #f4f4f5
--fw-zinc-200: rgb(228 228 231);    // #e4e4e7
--fw-zinc-300: rgb(212 212 216);    // #d4d4d8
--fw-zinc-400: rgb(161 161 170);    // #a1a1aa
--fw-zinc-500: rgb(113 113 122);    // #71717a
--fw-zinc-600: rgb(82 82 91);       // #52525b
--fw-zinc-700: rgb(63 63 70);       // #3f3f46
--fw-zinc-800: rgb(39 39 42);       // #27272a
--fw-zinc-900: rgb(24 24 27);       // #18181b
--fw-neutral-50: rgb(250 250 250);  // #fafafa
--fw-neutral-100: rgb(245 245 245); // #f5f5f5
--fw-neutral-200: rgb(229 229 229); // #e5e5e5
--fw-neutral-300: rgb(212 212 212); // #d4d4d4
--fw-neutral-400: rgb(163 163 163); // #a3a3a3
--fw-neutral-500: rgb(115 115 115); // #737373
--fw-neutral-600: rgb(82 82 82);    // #525252
--fw-neutral-700: rgb(64 64 64);    // #404040
--fw-neutral-800: rgb(38 38 38);    // #262626
--fw-neutral-900: rgb(23 23 23);    // #171717
--fw-stone-50: rgb(250 250 249);    // #fafaf9
--fw-stone-100: rgb(245 245 244);   // #f5f5f4
--fw-stone-200: rgb(231 229 228);   // #e7e5e4
--fw-stone-300: rgb(214 211 209);   // #d6d3d1
--fw-stone-400: rgb(168 162 158);   // #a8a29e
--fw-stone-500: rgb(120 113 108);   // #78716c
--fw-stone-600: rgb(87 83 78);      // #57534e
--fw-stone-700: rgb(68 64 60);      // #44403c
--fw-stone-800: rgb(41 37 36);      // #292524
--fw-stone-900: rgb(28 25 23);      // #1c1917
--fw-red-50: rgb(254 242 242);      // #fef2f2
--fw-red-100: rgb(254 226 226);     // #fee2e2
--fw-red-200: rgb(254 202 202);     // #fecaca
--fw-red-300: rgb(252 165 165);     // #fca5a5
--fw-red-400: rgb(248 113 113);     // #f87171
--fw-red-500: rgb(239 68 68);       // #ef4444
--fw-red-600: rgb(220 38 38);       // #dc2626
--fw-red-700: rgb(185 28 28);       // #b91c1c
--fw-red-800: rgb(153 27 27);       // #991b1b
--fw-red-900: rgb(127 29 29);       // #7f1d1d
--fw-orange-50: rgb(255 247 237);   // #fff7ed
--fw-orange-100: rgb(255 237 213);  // #ffedd5
--fw-orange-200: rgb(254 215 170);  // #fed7aa
--fw-orange-300: rgb(253 186 116);  // #fdba74
--fw-orange-400: rgb(251 146 60);   // #fb923c
--fw-orange-500: rgb(249 115 22);   // #f97316
--fw-orange-600: rgb(234 88 12);    // #ea580c
--fw-orange-700: rgb(194 65 12);    // #c2410c
--fw-orange-800: rgb(154 52 18);    // #9a3412
--fw-orange-900: rgb(124 45 18);    // #7c2d12
--fw-amber-50: rgb(255 251 235);    // #fffbeb
--fw-amber-100: rgb(254 243 199);   // #fef3c7
--fw-amber-200: rgb(253 230 138);   // #fde68a
--fw-amber-300: rgb(252 211 77);    // #fcd34d
--fw-amber-400: rgb(251 191 36);    // #fbbf24
--fw-amber-500: rgb(245 158 11);    // #f59e0b
--fw-amber-600: rgb(217 119 6);     // #d97706
--fw-amber-700: rgb(180 83 9);      // #b45309
--fw-amber-800: rgb(146 64 14);     // #92400e
--fw-amber-900: rgb(120 53 15);     // #78350f
--fw-yellow-50: rgb(254 252 232);   // #fefce8
--fw-yellow-100: rgb(254 249 195);  // #fef9c3
--fw-yellow-200: rgb(254 240 138);  // #fef08a
--fw-yellow-300: rgb(253 224 71);   // #fde047
--fw-yellow-400: rgb(250 204 21);   // #facc15
--fw-yellow-500: rgb(234 179 8);    // #eab308
--fw-yellow-600: rgb(202 138 4);    // #ca8a04
--fw-yellow-700: rgb(161 98 7);     // #a16207
--fw-yellow-800: rgb(133 77 14);    // #854d0e
--fw-yellow-900: rgb(113 63 18);    // #713f12
--fw-lime-50: rgb(247 254 231);     // #f7fee7
--fw-lime-100: rgb(236 252 203);    // #ecfccb
--fw-lime-200: rgb(217 249 157);    // #d9f99d
--fw-lime-300: rgb(190 242 100);    // #bef264
--fw-lime-400: rgb(163 230 53);     // #a3e635
--fw-lime-500: rgb(132 204 22);     // #84cc16
--fw-lime-600: rgb(101 163 13);     // #65a30d
--fw-lime-700: rgb(77 124 15);      // #4d7c0f
--fw-lime-800: rgb(63 98 18);       // #3f6212
--fw-lime-900: rgb(54 83 20);       // #365314
--fw-green-50: rgb(240 253 244);    // #f0fdf4
--fw-green-100: rgb(220 252 231);   // #dcfce7
--fw-green-200: rgb(187 247 208);   // #bbf7d0
--fw-green-300: rgb(134 239 172);   // #86efac
--fw-green-400: rgb(74 222 128);    // #4ade80
--fw-green-500: rgb(34 197 94);     // #22c55e
--fw-green-600: rgb(22 163 74);     // #16a34a
--fw-green-700: rgb(21 128 61);     // #15803d
--fw-green-800: rgb(22 101 52);     // #166534
--fw-green-900: rgb(20 83 45);      // #14532d
--fw-emerald-50: rgb(236 253 245);  // #ecfdf5
--fw-emerald-100: rgb(209 250 229); // #d1fae5
--fw-emerald-200: rgb(167 243 208); // #a7f3d0
--fw-emerald-300: rgb(110 231 183); // #6ee7b7
--fw-emerald-400: rgb(52 211 153);  // #34d399
--fw-emerald-500: rgb(16 185 129);  // #10b981
--fw-emerald-600: rgb(5 150 105);   // #059669
--fw-emerald-700: rgb(4 120 87);    // #047857
--fw-emerald-800: rgb(6 95 70);     // #065f46
--fw-emerald-900: rgb(6 78 59);     // #064e3b
--fw-teal-50: rgb(240 253 250);     // #f0fdfa
--fw-teal-100: rgb(204 251 241);    // #ccfbf1
--fw-teal-200: rgb(153 246 228);    // #99f6e4
--fw-teal-300: rgb(94 234 212);     // #5eead4
--fw-teal-400: rgb(45 212 191);     // #2dd4bf
--fw-teal-500: rgb(20 184 166);     // #14b8a6
--fw-teal-600: rgb(13 148 136);     // #0d9488
--fw-teal-700: rgb(15 118 110);     // #0f766e
--fw-teal-800: rgb(17 94 89);       // #115e59
--fw-teal-900: rgb(19 78 74);       // #134e4a
--fw-cyan-50: rgb(236 254 255);     // #ecfeff
--fw-cyan-100: rgb(207 250 254);    // #cffafe
--fw-cyan-200: rgb(165 243 252);    // #a5f3fc
--fw-cyan-300: rgb(103 232 249);    // #67e8f9
--fw-cyan-400: rgb(34 211 238);     // #22d3ee
--fw-cyan-500: rgb(6 182 212);      // #06b6d4
--fw-cyan-600: rgb(8 145 178);      // #0891b2
--fw-cyan-700: rgb(14 116 144);     // #0e7490
--fw-cyan-800: rgb(21 94 117);      // #155e75
--fw-cyan-900: rgb(22 78 99);       // #164e63
--fw-sky-50: rgb(240 249 255);      // #f0f9ff
--fw-sky-100: rgb(224 242 254);     // #e0f2fe
--fw-sky-200: rgb(186 230 253);     // #bae6fd
--fw-sky-300: rgb(125 211 252);     // #7dd3fc
--fw-sky-400: rgb(56 189 248);      // #38bdf8
--fw-sky-500: rgb(14 165 233);      // #0ea5e9
--fw-sky-600: rgb(2 132 199);       // #0284c7
--fw-sky-700: rgb(3 105 161);       // #0369a1
--fw-sky-800: rgb(7 89 133);        // #075985
--fw-sky-900: rgb(12 74 110);       // #0c4a6e
--fw-blue-50: rgb(239 246 255);     // #eff6ff
--fw-blue-100: rgb(219 234 254);    // #dbeafe
--fw-blue-200: rgb(191 219 254);    // #bfdbfe
--fw-blue-300: rgb(147 197 253);    // #93c5fd
--fw-blue-400: rgb(96 165 250);     // #60a5fa
--fw-blue-500: rgb(59 130 246);     // #3b82f6
--fw-blue-600: rgb(37 99 235);      // #2563eb
--fw-blue-700: rgb(29 78 216);      // #1d4ed8
--fw-blue-800: rgb(30 64 175);      // #1e40af
--fw-blue-900: rgb(30 58 138);      // #1e3a8a
--fw-indigo-50: rgb(238 242 255);   // #eef2ff
--fw-indigo-100: rgb(224 231 255);  // #e0e7ff
--fw-indigo-200: rgb(199 210 254);  // #c7d2fe
--fw-indigo-300: rgb(165 180 252);  // #a5b4fc
--fw-indigo-400: rgb(129 140 248);  // #818cf8
--fw-indigo-500: rgb(99 102 241);   // #6366f1
--fw-indigo-600: rgb(79 70 229);    // #4f46e5
--fw-indigo-700: rgb(67 56 202);    // #4338ca
--fw-indigo-800: rgb(55 48 163);    // #3730a3
--fw-indigo-900: rgb(49 46 129);    // #312e81
--fw-violet-50: rgb(245 243 255);   // #f5f3ff
--fw-violet-100: rgb(237 233 254);  // #ede9fe
--fw-violet-200: rgb(221 214 254);  // #ddd6fe
--fw-violet-300: rgb(196 181 253);  // #c4b5fd
--fw-violet-400: rgb(167 139 250);  // #a78bfa
--fw-violet-500: rgb(139 92 246);   // #8b5cf6
--fw-violet-600: rgb(124 58 237);   // #7c3aed
--fw-violet-700: rgb(109 40 217);   // #6d28d9
--fw-violet-800: rgb(91 33 182);    // #5b21b6
--fw-violet-900: rgb(76 29 149);    // #4c1d95
--fw-purple-50: rgb(250 245 255);   // #faf5ff
--fw-purple-100: rgb(243 232 255);  // #f3e8ff
--fw-purple-200: rgb(233 213 255);  // #e9d5ff
--fw-purple-300: rgb(216 180 254);  // #d8b4fe
--fw-purple-400: rgb(192 132 252);  // #c084fc
--fw-purple-500: rgb(168 85 247);   // #a855f7
--fw-purple-600: rgb(147 51 234);   // #9333ea
--fw-purple-700: rgb(126 34 206);   // #7e22ce
--fw-purple-800: rgb(107 33 168);   // #6b21a8
--fw-purple-900: rgb(88 28 135);    // #581c87
--fw-fuchsia-50: rgb(253 244 255);  // #fdf4ff
--fw-fuchsia-100: rgb(250 232 255); // #fae8ff
--fw-fuchsia-200: rgb(245 208 254); // #f5d0fe
--fw-fuchsia-300: rgb(240 171 252); // #f0abfc
--fw-fuchsia-400: rgb(232 121 249); // #e879f9
--fw-fuchsia-500: rgb(217 70 239);  // #d946ef
--fw-fuchsia-600: rgb(192 38 211);  // #c026d3
--fw-fuchsia-700: rgb(162 28 175);  // #a21caf
--fw-fuchsia-800: rgb(134 25 143);  // #86198f
--fw-fuchsia-900: rgb(112 26 117);  // #701a75
--fw-pink-50: rgb(253 242 248);     // #fdf2f8
--fw-pink-100: rgb(252 231 243);    // #fce7f3
--fw-pink-200: rgb(251 207 232);    // #fbcfe8
--fw-pink-300: rgb(249 168 212);    // #f9a8d4
--fw-pink-400: rgb(244 114 182);    // #f472b6
--fw-pink-500: rgb(236 72 153);     // #ec4899
--fw-pink-600: rgb(219 39 119);     // #db2777
--fw-pink-700: rgb(190 24 93);      // #be185d
--fw-pink-800: rgb(157 23 77);      // #9d174d
--fw-pink-900: rgb(131 24 67);      // #831843
--fw-rose-50: rgb(255 241 242);     // #fff1f2
--fw-rose-100: rgb(255 228 230);    // #ffe4e6
--fw-rose-200: rgb(254 205 211);    // #fecdd3
--fw-rose-300: rgb(253 164 175);    // #fda4af
--fw-rose-400: rgb(251 113 133);    // #fb7185
--fw-rose-500: rgb(244 63 94);      // #f43f5e
--fw-rose-600: rgb(225 29 72);      // #e11d48
--fw-rose-700: rgb(190 18 60);      // #be123c
--fw-rose-800: rgb(159 18 57);      // #9f1239
--fw-rose-900: rgb(136 19 55);      // #881337
```
</details>

### Colors transparency (alpha)
#### Use ```--fw-color-opacity``` variable to set the color transparency 

Each color rule in Freewindcss uses the ```--fw-color-opacity``` variable (which is initialized to 1) to determine the transparency of the color. Therefore to apply a color with transparency you have to set the variable ```--fw-color-opacity``` to the desired fraction number.  

Note that the variable ```--fw-color-opacity``` will be applied to the entire defined element, so two Freewindcss color rules cannot be applied to the same element with different transparency.

#### example:
```scss
element {
  --fw-color-opacity: 0.6;
  color: var(--fw-indigo-500); // rgba(99, 102, 241, 0.6)
  background-color: var(--fw-lime-300); // rgba(190, 242, 100, 0.6);
}
```

### Animations
#### example:
```scss
element {
  animation: var(--fw-animation-pulse); // fw-pulse 2s cubic-bezier(0.4, 0, 0.6, 1) infinite
}
```

<details open>
<summary>Variables</summary>

```scss
--fw-animation-spin: fw-spin 1s linear infinite;
--fw-animation-ping: fw-ping 1s cubic-bezier(0, 0, 0.2, 1) infinite;
--fw-animation-pulse: fw-pulse 2s cubic-bezier(0.4, 0, 0.6, 1) infinite;
--fw-animation-bounce: fw-bounce 1s infinite;
```
</details>

### Container Width
#### Can be used with the `width` or `max-width`, for example:
```scss
element {
  width: 100%;
  max-width: var(--fw-container-width);
}
```

The value of `--fw-container-width` will depend on the screen size:
```scss
@media (max-width: 640px) {
  --fw-container-width: 640px;
}

@media (max-width: 768px) {
  --fw-container-width: 768px;
}

@media (max-width: 1024px) {
  --fw-container-width: 1024px;
}

// or in a bigger screen:
--fw-container-width: 1280px;
```

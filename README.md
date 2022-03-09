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

#### Variables

<details open>
<summary>Show/Hide</summary>

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

#### Variables
```scss
--fw-font-sans: ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, "Noto Sans", sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji";
--fw-font-serif: ui-serif, Georgia, Cambria, "Times New Roman", Times, serif;
--fw-font-mono: ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, "Liberation Mono", "Courier New", monospace;
```

### Font Size
#### Can be used with the `font-size` property, for example:
```scss
element {
  font-size: var(--fw-text-2xl); // 1.5rem
}
```

#### Variables
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

### Font Weight
#### For example:
```scss
element {
  font-weight: var(--fw-font-semibold); // 600
}
```

#### Variables
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

### Letter Spacing
#### Using with `letter-spacing` property, for example:
```scss
element {
  letter-spacing: var(--fw-tracking-tight); // -0.025em
}
```

#### Variables
```scss
--fw-tracking-tighter: -0.05em;
--fw-tracking-tight: -0.025em;
--fw-tracking-normal: 0;
--fw-tracking-wide: 0.025em;
--fw-tracking-wider: 0.05em;
--fw-tracking-widest: 0.1em;
```

### Line Height
#### Used with `line-height` property, for example:
```scss
element {
  line-height: var(--fw-leading-5); // 20px
}
```

#### Variables
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

### Border Radius
#### For example:
```scss
element {
  border-radius: var(--fw-rounded-md); // 6px
}
```

#### Variables
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

### Box Shadow
#### For example:
```scss
element {
  box-shadow: var(--fw-shadow-lg); // 0 10px 15px -3px rgb(0 0 0 / 0.1), 0 4px 6px -4px rgb(0 0 0 / 0.1)
}
```

#### Variables
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

### Blur Filter
#### Used with `filter: blur(x)` or with `  backdrop-filter: blur(x)`, for example:
```scss
element {
  backdrop-filter: var(--fw-blur-md); // blur(12px)
}
```

#### Variables
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

### Drop Shadow
#### Used with `filter: drop-shadow(x)`, for example:
```scss
element {
  filter: var(--fw-drop-shadow-sm); // drop-shadow(0 1px 1px rgb(0 0 0 / 0.05))
}
```

#### Variables
```scss
--fw-drop-shadow-sm: drop-shadow(0 1px 1px rgb(0 0 0 / 0.05));
--fw-drop-shadow: drop-shadow(0 1px 2px rgb(0 0 0 / 0.1)) drop-shadow(0 1px 1px rgb(0 0 0 / 0.06));
--fw-drop-shadow-md: drop-shadow(0 4px 3px rgb(0 0 0 / 0.07)) drop-shadow(0 2px 2px rgb(0 0 0 / 0.06));
--fw-drop-shadow-lg: drop-shadow(0 10px 8px rgb(0 0 0 / 0.04)) drop-shadow(0 4px 3px rgb(0 0 0 / 0.1));
--fw-drop-shadow-xl: drop-shadow(0 20px 13px rgb(0 0 0 / 0.03)) drop-shadow(0 8px 5px rgb(0 0 0 / 0.08));
--fw-drop-shadow-2xl: drop-shadow(0 25px 25px rgb(0 0 0 / 0.15));
--fw-drop-shadow-none: drop-shadow(0 0 #0000);
```

### Columns
#### example:
```scss
element {
  columns: var(--fw-columns-3xl); // 768px
}
```

#### Variables

<details open>
<summary>Show/Hide</summary>

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

#### Variables
```scss
--fw-ease-linear: linear;
--fw-ease-in: cubic-bezier(0.4, 0, 1, 1);
--fw-ease-out: cubic-bezier(0, 0, 0.2, 1);
--fw-ease-in-out: cubic-bezier(0.4, 0, 0.2, 1);
```

### Colors
#### example:
```scss
element {
  color: var(--fw-slate-100); // rgb(241 245 249)
  background: var(--fw-fuchsia-500); // rgb(217 70 239)
}
```

#### Variables

<details open>
<summary>Show/Hide</summary>

```clojure
--fw-black: rgb(0 0 0);             // rgb(0 0 0)
--fw-white: rgb(255 255 255);       // rgb(255 255 255)
--fw-slate-50: rgb(248 250 252);    // rgb(248 250 252)
--fw-slate-100: rgb(241 245 249);   // rgb(241 245 249)
--fw-slate-200: rgb(226 232 240);   // rgb(226 232 240)
--fw-slate-300: rgb(203 213 225);   // rgb(203 213 225)
--fw-slate-400: rgb(148 163 184);   // rgb(148 163 184)
--fw-slate-500: rgb(100 116 139);   // rgb(100 116 139)
--fw-slate-600: rgb(71 85 105);     // rgb(71 85 105)
--fw-slate-700: rgb(51 65 85);      // rgb(51 65 85)
--fw-slate-800: rgb(30 41 59);      // rgb(30 41 59)
--fw-slate-900: rgb(15 23 42);      // rgb(15 23 42)
--fw-gray-50: rgb(249 250 251);     // rgb(249 250 251)
--fw-gray-100: rgb(243 244 246);    // rgb(243 244 246)
--fw-gray-200: rgb(229 231 235);    // rgb(229 231 235)
--fw-gray-300: rgb(209 213 219);    // rgb(209 213 219)
--fw-gray-400: rgb(156 163 175);    // rgb(156 163 175)
--fw-gray-500: rgb(107 114 128);    // rgb(107 114 128)
--fw-gray-600: rgb(75 85 99);       // rgb(75 85 99)
--fw-gray-700: rgb(55 65 81);       // rgb(55 65 81)
--fw-gray-800: rgb(31 41 55);       // rgb(31 41 55)
--fw-gray-900: rgb(17 24 39);       // rgb(17 24 39)
--fw-zinc-50: rgb(250 250 250);     // rgb(250 250 250)
--fw-zinc-100: rgb(244 244 245);    // rgb(244 244 245)
--fw-zinc-200: rgb(228 228 231);    // rgb(228 228 231)
--fw-zinc-300: rgb(212 212 216);    // rgb(212 212 216)
--fw-zinc-400: rgb(161 161 170);    // rgb(161 161 170)
--fw-zinc-500: rgb(113 113 122);    // rgb(113 113 122)
--fw-zinc-600: rgb(82 82 91);       // rgb(82 82 91)
--fw-zinc-700: rgb(63 63 70);       // rgb(63 63 70)
--fw-zinc-800: rgb(39 39 42);       // rgb(39 39 42)
--fw-zinc-900: rgb(24 24 27);       // rgb(24 24 27)
--fw-neutral-50: rgb(250 250 250);  // rgb(250 250 250)
--fw-neutral-100: rgb(245 245 245); // rgb(245 245 245)
--fw-neutral-200: rgb(229 229 229); // rgb(229 229 229)
--fw-neutral-300: rgb(212 212 212); // rgb(212 212 212)
--fw-neutral-400: rgb(163 163 163); // rgb(163 163 163)
--fw-neutral-500: rgb(115 115 115); // rgb(115 115 115)
--fw-neutral-600: rgb(82 82 82);    // rgb(82 82 82)
--fw-neutral-700: rgb(64 64 64);    // rgb(64 64 64)
--fw-neutral-800: rgb(38 38 38);    // rgb(38 38 38)
--fw-neutral-900: rgb(23 23 23);    // rgb(23 23 23)
--fw-stone-50: rgb(250 250 249);    // rgb(250 250 249)
--fw-stone-100: rgb(245 245 244);   // rgb(245 245 244)
--fw-stone-200: rgb(231 229 228);   // rgb(231 229 228)
--fw-stone-300: rgb(214 211 209);   // rgb(214 211 209)
--fw-stone-400: rgb(168 162 158);   // rgb(168 162 158)
--fw-stone-500: rgb(120 113 108);   // rgb(120 113 108)
--fw-stone-600: rgb(87 83 78);      // rgb(87 83 78)
--fw-stone-700: rgb(68 64 60);      // rgb(68 64 60)
--fw-stone-800: rgb(41 37 36);      // rgb(41 37 36)
--fw-stone-900: rgb(28 25 23);      // rgb(28 25 23)
--fw-red-50: rgb(254 242 242);      // rgb(254 242 242)
--fw-red-100: rgb(254 226 226);     // rgb(254 226 226)
--fw-red-200: rgb(254 202 202);     // rgb(254 202 202)
--fw-red-300: rgb(252 165 165);     // rgb(252 165 165)
--fw-red-400: rgb(248 113 113);     // rgb(248 113 113)
--fw-red-500: rgb(239 68 68);       // rgb(239 68 68)
--fw-red-600: rgb(220 38 38);       // rgb(220 38 38)
--fw-red-700: rgb(185 28 28);       // rgb(185 28 28)
--fw-red-800: rgb(153 27 27);       // rgb(153 27 27)
--fw-red-900: rgb(127 29 29);       // rgb(127 29 29)
--fw-orange-50: rgb(255 247 237);   // rgb(255 247 237)
--fw-orange-100: rgb(255 237 213);  // rgb(255 237 213)
--fw-orange-200: rgb(254 215 170);  // rgb(254 215 170)
--fw-orange-300: rgb(253 186 116);  // rgb(253 186 116)
--fw-orange-400: rgb(251 146 60);   // rgb(251 146 60)
--fw-orange-500: rgb(249 115 22);   // rgb(249 115 22)
--fw-orange-600: rgb(234 88 12);    // rgb(234 88 12)
--fw-orange-700: rgb(194 65 12);    // rgb(194 65 12)
--fw-orange-800: rgb(154 52 18);    // rgb(154 52 18)
--fw-orange-900: rgb(124 45 18);    // rgb(124 45 18)
--fw-amber-50: rgb(255 251 235);    // rgb(255 251 235)
--fw-amber-100: rgb(254 243 199);   // rgb(254 243 199)
--fw-amber-200: rgb(253 230 138);   // rgb(253 230 138)
--fw-amber-300: rgb(252 211 77);    // rgb(252 211 77)
--fw-amber-400: rgb(251 191 36);    // rgb(251 191 36)
--fw-amber-500: rgb(245 158 11);    // rgb(245 158 11)
--fw-amber-600: rgb(217 119 6);     // rgb(217 119 6)
--fw-amber-700: rgb(180 83 9);      // rgb(180 83 9)
--fw-amber-800: rgb(146 64 14);     // rgb(146 64 14)
--fw-amber-900: rgb(120 53 15);     // rgb(120 53 15)
--fw-yellow-50: rgb(254 252 232);   // rgb(254 252 232)
--fw-yellow-100: rgb(254 249 195);  // rgb(254 249 195)
--fw-yellow-200: rgb(254 240 138);  // rgb(254 240 138)
--fw-yellow-300: rgb(253 224 71);   // rgb(253 224 71)
--fw-yellow-400: rgb(250 204 21);   // rgb(250 204 21)
--fw-yellow-500: rgb(234 179 8);    // rgb(234 179 8)
--fw-yellow-600: rgb(202 138 4);    // rgb(202 138 4)
--fw-yellow-700: rgb(161 98 7);     // rgb(161 98 7)
--fw-yellow-800: rgb(133 77 14);    // rgb(133 77 14)
--fw-yellow-900: rgb(113 63 18);    // rgb(113 63 18)
--fw-lime-50: rgb(247 254 231);     // rgb(247 254 231)
--fw-lime-100: rgb(236 252 203);    // rgb(236 252 203)
--fw-lime-200: rgb(217 249 157);    // rgb(217 249 157)
--fw-lime-300: rgb(190 242 100);    // rgb(190 242 100)
--fw-lime-400: rgb(163 230 53);     // rgb(163 230 53)
--fw-lime-500: rgb(132 204 22);     // rgb(132 204 22)
--fw-lime-600: rgb(101 163 13);     // rgb(101 163 13)
--fw-lime-700: rgb(77 124 15);      // rgb(77 124 15)
--fw-lime-800: rgb(63 98 18);       // rgb(63 98 18)
--fw-lime-900: rgb(54 83 20);       // rgb(54 83 20)
--fw-green-50: rgb(240 253 244);    // rgb(240 253 244)
--fw-green-100: rgb(220 252 231);   // rgb(220 252 231)
--fw-green-200: rgb(187 247 208);   // rgb(187 247 208)
--fw-green-300: rgb(134 239 172);   // rgb(134 239 172)
--fw-green-400: rgb(74 222 128);    // rgb(74 222 128)
--fw-green-500: rgb(34 197 94);     // rgb(34 197 94)
--fw-green-600: rgb(22 163 74);     // rgb(22 163 74)
--fw-green-700: rgb(21 128 61);     // rgb(21 128 61)
--fw-green-800: rgb(22 101 52);     // rgb(22 101 52)
--fw-green-900: rgb(20 83 45);      // rgb(20 83 45)
--fw-emerald-50: rgb(236 253 245);  // rgb(236 253 245)
--fw-emerald-100: rgb(209 250 229); // rgb(209 250 229)
--fw-emerald-200: rgb(167 243 208); // rgb(167 243 208)
--fw-emerald-300: rgb(110 231 183); // rgb(110 231 183)
--fw-emerald-400: rgb(52 211 153);  // rgb(52 211 153)
--fw-emerald-500: rgb(16 185 129);  // rgb(16 185 129)
--fw-emerald-600: rgb(5 150 105);   // rgb(5 150 105)
--fw-emerald-700: rgb(4 120 87);    // rgb(4 120 87)
--fw-emerald-800: rgb(6 95 70);     // rgb(6 95 70)
--fw-emerald-900: rgb(6 78 59);     // rgb(6 78 59)
--fw-teal-50: rgb(240 253 250);     // rgb(240 253 250)
--fw-teal-100: rgb(204 251 241);    // rgb(204 251 241)
--fw-teal-200: rgb(153 246 228);    // rgb(153 246 228)
--fw-teal-300: rgb(94 234 212);     // rgb(94 234 212)
--fw-teal-400: rgb(45 212 191);     // rgb(45 212 191)
--fw-teal-500: rgb(20 184 166);     // rgb(20 184 166)
--fw-teal-600: rgb(13 148 136);     // rgb(13 148 136)
--fw-teal-700: rgb(15 118 110);     // rgb(15 118 110)
--fw-teal-800: rgb(17 94 89);       // rgb(17 94 89)
--fw-teal-900: rgb(19 78 74);       // rgb(19 78 74)
--fw-cyan-50: rgb(236 254 255);     // rgb(236 254 255)
--fw-cyan-100: rgb(207 250 254);    // rgb(207 250 254)
--fw-cyan-200: rgb(165 243 252);    // rgb(165 243 252)
--fw-cyan-300: rgb(103 232 249);    // rgb(103 232 249)
--fw-cyan-400: rgb(34 211 238);     // rgb(34 211 238)
--fw-cyan-500: rgb(6 182 212);      // rgb(6 182 212)
--fw-cyan-600: rgb(8 145 178);      // rgb(8 145 178)
--fw-cyan-700: rgb(14 116 144);     // rgb(14 116 144)
--fw-cyan-800: rgb(21 94 117);      // rgb(21 94 117)
--fw-cyan-900: rgb(22 78 99);       // rgb(22 78 99)
--fw-sky-50: rgb(240 249 255);      // rgb(240 249 255)
--fw-sky-100: rgb(224 242 254);     // rgb(224 242 254)
--fw-sky-200: rgb(186 230 253);     // rgb(186 230 253)
--fw-sky-300: rgb(125 211 252);     // rgb(125 211 252)
--fw-sky-400: rgb(56 189 248);      // rgb(56 189 248)
--fw-sky-500: rgb(14 165 233);      // rgb(14 165 233)
--fw-sky-600: rgb(2 132 199);       // rgb(2 132 199)
--fw-sky-700: rgb(3 105 161);       // rgb(3 105 161)
--fw-sky-800: rgb(7 89 133);        // rgb(7 89 133)
--fw-sky-900: rgb(12 74 110);       // rgb(12 74 110)
--fw-blue-50: rgb(239 246 255);     // rgb(239 246 255)
--fw-blue-100: rgb(219 234 254);    // rgb(219 234 254)
--fw-blue-200: rgb(191 219 254);    // rgb(191 219 254)
--fw-blue-300: rgb(147 197 253);    // rgb(147 197 253)
--fw-blue-400: rgb(96 165 250);     // rgb(96 165 250)
--fw-blue-500: rgb(59 130 246);     // rgb(59 130 246)
--fw-blue-600: rgb(37 99 235);      // rgb(37 99 235)
--fw-blue-700: rgb(29 78 216);      // rgb(29 78 216)
--fw-blue-800: rgb(30 64 175);      // rgb(30 64 175)
--fw-blue-900: rgb(30 58 138);      // rgb(30 58 138)
--fw-indigo-50: rgb(238 242 255);   // rgb(238 242 255)
--fw-indigo-100: rgb(224 231 255);  // rgb(224 231 255)
--fw-indigo-200: rgb(199 210 254);  // rgb(199 210 254)
--fw-indigo-300: rgb(165 180 252);  // rgb(165 180 252)
--fw-indigo-400: rgb(129 140 248);  // rgb(129 140 248)
--fw-indigo-500: rgb(99 102 241);   // rgb(99 102 241)
--fw-indigo-600: rgb(79 70 229);    // rgb(79 70 229)
--fw-indigo-700: rgb(67 56 202);    // rgb(67 56 202)
--fw-indigo-800: rgb(55 48 163);    // rgb(55 48 163)
--fw-indigo-900: rgb(49 46 129);    // rgb(49 46 129)
--fw-violet-50: rgb(245 243 255);   // rgb(245 243 255)
--fw-violet-100: rgb(237 233 254);  // rgb(237 233 254)
--fw-violet-200: rgb(221 214 254);  // rgb(221 214 254)
--fw-violet-300: rgb(196 181 253);  // rgb(196 181 253)
--fw-violet-400: rgb(167 139 250);  // rgb(167 139 250)
--fw-violet-500: rgb(139 92 246);   // rgb(139 92 246)
--fw-violet-600: rgb(124 58 237);   // rgb(124 58 237)
--fw-violet-700: rgb(109 40 217);   // rgb(109 40 217)
--fw-violet-800: rgb(91 33 182);    // rgb(91 33 182)
--fw-violet-900: rgb(76 29 149);    // rgb(76 29 149)
--fw-purple-50: rgb(250 245 255);   // rgb(250 245 255)
--fw-purple-100: rgb(243 232 255);  // rgb(243 232 255)
--fw-purple-200: rgb(233 213 255);  // rgb(233 213 255)
--fw-purple-300: rgb(216 180 254);  // rgb(216 180 254)
--fw-purple-400: rgb(192 132 252);  // rgb(192 132 252)
--fw-purple-500: rgb(168 85 247);   // rgb(168 85 247)
--fw-purple-600: rgb(147 51 234);   // rgb(147 51 234)
--fw-purple-700: rgb(126 34 206);   // rgb(126 34 206)
--fw-purple-800: rgb(107 33 168);   // rgb(107 33 168)
--fw-purple-900: rgb(88 28 135);    // rgb(88 28 135)
--fw-fuchsia-50: rgb(253 244 255);  // rgb(253 244 255)
--fw-fuchsia-100: rgb(250 232 255); // rgb(250 232 255)
--fw-fuchsia-200: rgb(245 208 254); // rgb(245 208 254)
--fw-fuchsia-300: rgb(240 171 252); // rgb(240 171 252)
--fw-fuchsia-400: rgb(232 121 249); // rgb(232 121 249)
--fw-fuchsia-500: rgb(217 70 239);  // rgb(217 70 239)
--fw-fuchsia-600: rgb(192 38 211);  // rgb(192 38 211)
--fw-fuchsia-700: rgb(162 28 175);  // rgb(162 28 175)
--fw-fuchsia-800: rgb(134 25 143);  // rgb(134 25 143)
--fw-fuchsia-900: rgb(112 26 117);  // rgb(112 26 117)
--fw-pink-50: rgb(253 242 248);     // rgb(253 242 248)
--fw-pink-100: rgb(252 231 243);    // rgb(252 231 243)
--fw-pink-200: rgb(251 207 232);    // rgb(251 207 232)
--fw-pink-300: rgb(249 168 212);    // rgb(249 168 212)
--fw-pink-400: rgb(244 114 182);    // rgb(244 114 182)
--fw-pink-500: rgb(236 72 153);     // rgb(236 72 153)
--fw-pink-600: rgb(219 39 119);     // rgb(219 39 119)
--fw-pink-700: rgb(190 24 93);      // rgb(190 24 93)
--fw-pink-800: rgb(157 23 77);      // rgb(157 23 77)
--fw-pink-900: rgb(131 24 67);      // rgb(131 24 67)
--fw-rose-50: rgb(255 241 242);     // rgb(255 241 242)
--fw-rose-100: rgb(255 228 230);    // rgb(255 228 230)
--fw-rose-200: rgb(254 205 211);    // rgb(254 205 211)
--fw-rose-300: rgb(253 164 175);    // rgb(253 164 175)
--fw-rose-400: rgb(251 113 133);    // rgb(251 113 133)
--fw-rose-500: rgb(244 63 94);      // rgb(244 63 94)
--fw-rose-600: rgb(225 29 72);      // rgb(225 29 72)
--fw-rose-700: rgb(190 18 60);      // rgb(190 18 60)
--fw-rose-800: rgb(159 18 57);      // rgb(159 18 57)
--fw-rose-900: rgb(136 19 55);      // rgb(136 19 55)
```
</details>

### Animations
#### example:
```scss
element {
  animation: var(--fw-animation-pulse); // fw-pulse 2s cubic-bezier(0.4, 0, 0.6, 1) infinite;
}
```

#### Variables
```scss
--fw-animation-spin: fw-spin 1s linear infinite;
--fw-animation-ping: fw-ping 1s cubic-bezier(0, 0, 0.2, 1) infinite;
--fw-animation-pulse: fw-pulse 2s cubic-bezier(0.4, 0, 0.6, 1) infinite;
--fw-animation-bounce: fw-bounce 1s infinite;
```

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

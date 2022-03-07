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

## Documentation

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

### Font Family
#### Can be used withe the `font-family` property, for example:
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

### Font Sizes
#### Can be used withe the `font-size` property, for example:
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
  border-radius: var(--fw-rounded-md) // 6px
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

### Box Shadows
#### For example:
```scss
element {
  box-shadow: var(--fw-shadow-lg) // 0 10px 15px -3px rgb(0 0 0 / 0.1), 0 4px 6px -4px rgb(0 0 0 / 0.1)
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
  backdrop-filter: var(--fw-blur-md) // blur(12px)
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
  filter: var(--fw-drop-shadow-sm) // drop-shadow(0 1px 1px rgb(0 0 0 / 0.05))
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
  columns: var(--fw-columns-3xl) // 768px
}
```

#### Variables
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

### Transition Timing
#### example:
```scss
element {
  transition-timing-function: var(--fw-ease-out) // cubic-bezier(0, 0, 0.2, 1)
}
```

#### Variables
```scss
--fw-ease-linear: linear;
--fw-ease-in: cubic-bezier(0.4, 0, 1, 1);
--fw-ease-out: cubic-bezier(0, 0, 0.2, 1);
--fw-ease-in-out: cubic-bezier(0.4, 0, 0.2, 1);
```

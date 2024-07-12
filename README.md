# yardley.ca

Written by hand with TailwindCSS [https://tailwindcss.com/] for styling.

When developing, replace the stylesheet line with this:

```
<script src="https://cdn.tailwindcss.com"></script>
<script>
  tailwind.config = {
    theme: {
      extend: {
        fontFamily: {
          sans: ["Raleway", "sans-serif"],
          serif: ["Hepta Slab", "serif"],
        },
      },
    },
  }
</script>
```

Run this command when done to update the minified CSS file:

```
npx tailwindcss -i styles.css -o output.css --minify
```

Then replace the above with the original stylesheet line:

```
<link href="output.css" rel="stylesheet">
```

Check in and you're set!

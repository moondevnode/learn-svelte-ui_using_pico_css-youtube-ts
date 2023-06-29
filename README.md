# learn-svelte-ui_using_pico_css-youtube-ts

> [Source](https://github.com/moondevnode/learn-svelte-ui_using_pico_css-youtube-ts)


> [Why Pico Is My Favorite CSS Framework For Svelte(Youtube)](https://www.youtube.com/watch?v=-n84EMKIXQM)

[Blog](https://joyofcode.xyz/using-pico-css-with-svelte)

[Github](https://github.com/mattcroat/joy-of-code/tree/main/posts/using-pico-css-with-svelte)

> References
- [Picocss Documentation](https://picocss.com/docs/)
- [Picocss Github](https://github.com/picocss/pico)
- [Picocss Theme Default](https://github.com/picocss/pico/blob/master/css/themes/default.css)


# Timestamps

0:00 Intro
0:37 What is Pico.css?
2:12 Pico Setup
2:37 Looking At The Documentation
5:49 Example Site
7:38 Customizization Using CSS Variables
12:40 Customize Pico
17:51 Outro


> References

[Picocss > Docs > Customization](https://picocss.com/docs/customization.html)


# Install

```bash
# init app
bootapp -l node -u moondevnode -n learn-svelte-ui_using_pico_css-youtube-ts -d "Why Pico Is My Favorite CSS Framework For Svelte(https://www.youtube.com/watch?v=-n84EMKIXQM)" -t svelte-kit-ts

npm i @picocss/pico

# build
yarn dev
```


# Edit

> `src/routes/+layout.svelte`

```svelte
<script lang="ts">
  import '@picocss/pico'
  import '../app.css'
</script>

<slot />
```

> `src/app.css`

```css
:root {
  --primary: #d81b60;
}
```

> `src/routes/+page.svelte`

```svelte
<button >Button</button>
<input type="submit">
<a href="#" role="button">Link</a>
```


# run

```bash
yarn dev --open
```
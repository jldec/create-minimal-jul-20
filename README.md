# RedwoodSDK Minimal Starter

- This project repo was created with `pnpm create rwsdk -t minimal`
- A [Button](https://github.com/jldec/create-minimal-jul-20/blob/main/src/app/pages/Button.tsx) component (with 'use client') was added to the Home page.
- The project was then deplyed at https://create-minimal-jul-20.jldec.workers.dev/ using

```sh
NODE_ENV=development pnpm release
```

A client-side error occurs because of a request for https://create-minimal-jul-20.jldec.workers.dev/src/app/pages/Button.tsx which returns a 404 with `content-type: text/html`

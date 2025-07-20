# RedwoodSDK Minimal Starter

Repro for https://github.com/redwoodjs/sdk/issues/607

- This project repo was created with `pnpm create rwsdk -t minimal`
- A [Button](https://github.com/jldec/create-minimal-jul-20/blob/main/src/app/pages/Button.tsx) component (with 'use client') was added to the Home page.
- The project was then deployed at https://create-minimal-jul-20.jldec.workers.dev/ using

```sh
NODE_ENV=development pnpm release
```

A client-side error occurs because of a request for https://create-minimal-jul-20.jldec.workers.dev/src/app/pages/Button.tsx which returns a 404 with `content-type: text/html`

<img width="1304" height="804" alt="Screenshot 2025-07-20 at 13 22 11" src="https://github.com/user-attachments/assets/b7cbd942-c8c0-4fac-8adc-e6b30bb00155" />

# For an overview visit [pwrs.app](https://pwrs.app/)

To get started with the development you'll need the [rust toolchain](https://rustup.rs/), then you can start the host with `cargo run`
Available features:
* `sw` - includes the service worker
* `oauth` - replaces custom auth with google (requires env vars or `.env` with `GOOGLE_CLIENT_ID` and `GOOGLE_CLIENT_SECRET`!)  

TODO:
* user storage => gluesql?
* custom + oauth registration
* custom login
* move + adjust content
* built-in https (+ cert generation for debug?) 

Notes:
* WRY - awesome but I decided to focus on PWA thing, seems to have better platform support. 
* WASI - awesome but early. Need wider library support and more system APIs(at least full TLS) to get real.
* Maud - questionable but I love the rusty minimalistic syntax.
* SCSS - simple to start and scalable for complex projects, does not enforce anything. 
* TypeScript - type and memory safety all the way down.
* Axum - elegance and possibility to use without runtime for the SW.
* GlueSQL - uniform and familiar interface over any storage even on the client.
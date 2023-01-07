# @mails


```sh
yarn add @mails/template-name
```

## Templates

- one-time-password
  - signup code
  - login code
- welcome email


## Usage

```ts
import { template } from "@mails/email"

const client = template("my-app/otp-for-login")

function sendOtp(){
  client.withData({
      username: "Alice",
      code: "0XX-2dS"
    })
    .to("alice@acme.com")
    .send();
}
```

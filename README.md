# PCI Proxy Payment Component Demo

A small, dependency-free demo of the PCI Proxy Payment Component. It loads the
component from the Datatrans sandbox, lets you change its common configuration
options, and displays lifecycle events next to the payment form.

[Open the live demo](https://datatrans.github.io/pci-proxy-component-demo/)

> This project is for sandbox testing only. It imports the component from
> `pay.sandbox.datatrans.com` and is not configured for production payments.

## What the demo covers

- Mounting and unmounting the Payment Component
- Selecting a supported locale
- Enabling and configuring Click to Pay
- Toggling debug mode
- Handling `ready`, `error`, and `payment-complete` events
- Following a redirect returned for 3-D Secure authentication

## Prerequisites

- A transaction ID created in the Datatrans sandbox

The demo does not create transactions itself. Create the transaction through a server-to-server call.

## Try a payment

1. Enter a sandbox transaction ID.
2. Adjust the locale, Click to Pay, and debug settings as needed.
3. Select **Mount** to load the payment form.
4. Complete the sandbox payment and watch the **Events** panel for callbacks.
5. If the result contains a 3-D Secure redirect, use the button shown in the
   event entry to continue.
6. Select **Unmount** to reset the component and try another configuration.

For configuration options, API details, and the server-side transaction flow,
see the [PCI Proxy Payment Component documentation](https://docs.pci-proxy.com/docs/component).

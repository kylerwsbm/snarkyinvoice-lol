# SnarkyInvoice.lol

SnarkyInvoice.lol is a tongue‑in‑cheek invoicing tool designed to help you send overly official looking invoices for petty reasons. Need to bill a friend for “emotional damage” or a roommate for “forgetting to Venmo”? This little web app has you covered.

## Features

* **React App** – Built with a simple React front end (loaded via CDN), no backend required.
* **Friendly Form** – Enter the sender and recipient names, a reason for the invoice, a suggested amount in USD, adjust the “Petty Level” (0–100) and decide whether to include a ridiculous ultimatum.
* **Snark Engine** – Generates a message by combining your inputs with a random snarky template. Tone and vocabulary change based on the Petty Level slider.
* **Random Reasons** – Stuck on a reason? Click “Need inspiration?” to populate the reason field with a random petty suggestion.
* **Petty Meter** – A live descriptor (Polite, Saucy, Unhinged) appears next to the slider so you know exactly how over‑the‑top your invoice will be.
* **Playful Design** – A colourful doodle pattern in the header and witty tooltips throughout the form keep things light while you bill with spite.
* **Share Button** – Instantly share your invoice using the Web Share API on supported devices. If sharing isn’t available, the invoice text is copied to your clipboard so you can paste it anywhere.

## Getting Started

This repository is a simple static site—no build tools are required. To develop locally:

1. Clone the repo and open `index.html` in your browser. Because React and other libraries are pulled from CDNs, you can work without running a server. If you prefer, serve the files with a simple web server (e.g. `npx http-server .`).
2. Edit `index.html` and the embedded script to tweak the behaviour or styling.

## Deployment

This site can be deployed directly to any static hosting provider. For this MVP, we recommend Netlify:

1. Log into Netlify and click **New site from Git**.
2. Choose this repository, keep the default build settings (no build command is required because it’s static) and deploy.
3. After deployment, go to **Domain Management** and add the custom domain `snarkyinvoice.lol`. (Assuming the domain’s DNS already points to Netlify.)

## Future Enhancements

- **Richer sharing options** – The current share button sends a simple text representation of the invoice. A future version could generate an image of the invoice (using a library like `html2canvas`) and include it as an attachment when sharing.
- **Payment integration** – When we’re ready to get serious, integrate [Stripe](https://stripe.com/) to accept real payments—just make sure your friends are good sports!
- **Persistence** – Save invoice history in local storage or a database so you can keep tabs on all your petty billing.
- **Build tools** – Replace the CDN‑loaded React with a proper bundler like Vite once package registry access is available.

## Disclaimer

This project is for humour and educational purposes only. Use at your own risk—and don’t actually expect anyone to pay you for “emotional damage”… unless they deserve it. Send petty bills with maximum sass!
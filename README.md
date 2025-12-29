# PrintQRcards.com 🖨️

**High-fidelity, print-ready QR cards for the physical world.**

The reality of QR codes is that they are meant for the physical world. While most web components are designed to live strictly in a browser, `PrintQRcards.com` bridges the gap between digital data and physical utility. This project provides a specialized workflow to turn digital strings into professional assets that actually survive the printing process. 🛠️

## The Engineering Challenge: Designing for the Printer 📄

Most web development treats printing as an afterthought, often resulting in layouts that collapse or disappear when sent to paper. This project addresses the "Print Handshake" through a deliberate technical shift:

* **Print-First Architecture** 🏗️: The codebase utilizes a dedicated `@media print` orchestration layer. When the user triggers a print command, the application reconfigures into a document-first layout, stripping away the interactive web UI to ensure a clean, stable physical result.
* **Architectural Evolution** 🧬: Originally built as a Web Component showcase, the project was refactored into a high-performance Vanilla TypeScript architecture. Moving away from the Shadow DOM was a strategic choice to ensure maximum CSS transparency and reliability across various printer drivers.
* **Tiling System** 📋: Rather than leaving the layout to the whims of the printer's settings, the application includes logic to repeat and tile cards across a single sheet, maximizing paper utility for the user.

## Project Roadmap 🧪

* **Foundation** 🧱: Complete the migration from the original JavaScript component to the new TypeScript-driven logic and verify the Parcel build pipeline.
* **Local UI to Print Pipeline** 🛠️: Wire up a basic HTML form to the QR generator and ensure the `@media print` styles correctly isolate the card on a physical page.
* **Deployment** 🚀: Connect the repository to Netlify to establish a live staging environment.
* **Sheet Logic Implementation** 📏: Develop the CSS Grid-based "Sheet Mode" to allow for multiple cards per page without breaking the printer's margins.

## Technical Stack 💻

* **Language**: TypeScript (Strongly typed for reliable data-to-visual mapping).
* **Build Tool**: Parcel (Modern, zero-config bundling).
* **QR Engine**: `qrcode` (NPM).
* **Deployment**: Automated CI/CD via Netlify. 🏁
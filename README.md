# TON Deeplink Generator

## Live Demo

Check out the live version of the TON Deeplink Generator:

[TON Deeplink Generator Live Service](https://veebull.github.io/tontastic-deeplink-generator/)

## Table of Contents

- [TON Deeplink Generator](#ton-deeplink-generator)
  - [Live Demo](#live-demo)
  - [Table of Contents](#table-of-contents)
  - [Introduction](#introduction)
  - [Features](#features)
  - [Installation](#installation)
  - [Usage](#usage)
  - [Component Structure](#component-structure)
  - [Customization](#customization)
    - [Theming](#theming)
    - [Styling](#styling)
    - [Localization](#localization)
  - [Future Enhancements](#future-enhancements)
  - [Contributing](#contributing)
  - [Contact](#contact)

## Introduction

The TON Deeplink Generator is a powerful React component that allows users to create deep links for The Open Network (TON) blockchain. This tool simplifies the process of generating deep links for various TON-related operations, such as transfers and donations, making it easier for developers and users to interact with TON-based applications.

## Features

- **Prefix Selection**: Choose between `ton://` and `https://app.tonkeeper.com/` prefixes.
- **Operation Type**: Select between 'Transfer' and 'Donate' operations.
- **Address Input**: Enter the TON wallet address for the transaction.
- **Amount Input**:
  - Manual input with TON symbol display
  - Increase/decrease buttons for fine-tuning
  - Slider for quick adjustments
  - Preset amount buttons (5, 10, 100 TON)
- **Optional Text**: Add a message or comment to the transaction.
- **Binary Data Support**: Include base64-encoded binary data for advanced use cases.
- **Deeplink Generation**: Create a deep link based on the input parameters.
- **QR Code Generation**: Automatically generate a QR code for the created deep link.
- **Copy to Clipboard**: Easily copy the generated deep link.
- **Responsive Design**: Optimized for desktop, tablet, and mobile views.
- **Theme Toggle**: Switch between light and dark themes.
- **Local Storage**: Remember user's last inputs for convenience.

## Installation

1. Clone the repository:
   ```
   git clone https://github.com/your-repo/ton-deeplink-generator.git
   ```
2. Install dependencies:
   ```
   cd ton-deeplink-generator
   npm install
   ```
3. Ensure you have all required dependencies, including:
   - React
   - qrcode.react
   - lucide-react
   - @radix-ui/react-select
   - @radix-ui/react-slider
   - @radix-ui/react-tooltip
   - @radix-ui/react-collapsible

## Usage

Import the `TonDeeplinkGenerator` component into your React application:

```jsx
import { TonDeeplinkGenerator } from './path-to-component/TonDeeplinkGenerator';

function App() {
  return (
    <div className='App'>
      <TonDeeplinkGenerator />
    </div>
  );
}
```

## Component Structure

The `TonDeeplinkGenerator` component is structured as follows:

- Card container with header, content, and footer
- Two-column layout for inputs (on larger screens)
- Collapsible section for binary data input
- Generated deeplink display with copy button and QR code

## Customization

### Theming

The component uses a theme provider. You can customize the theme by modifying the theme context or CSS variables.

### Styling

The component uses Tailwind CSS classes. You can override these classes or extend the Tailwind configuration to customize the appearance.

### Localization

To support multiple languages, you can wrap the component with a localization provider and replace the hardcoded strings with localized versions.

## Future Enhancements

1. **Multiple Cryptocurrency Support**: Extend the generator to support other cryptocurrencies beyond TON.
2. **Transaction History**: Implement a feature to track and display previously generated deep links.
3. **Wallet Integration**: Add direct integration with popular TON wallets for seamless transactions.
4. **Advanced Validation**: Implement more robust input validation, especially for TON addresses and amounts.
5. **Custom Presets**: Allow users to save and quickly access custom presets for frequently used configurations.
6. **API Integration**: Integrate with TON blockchain APIs to fetch real-time data, such as wallet balances or transaction status.
7. **Internationalization**: Add support for multiple languages to make the tool accessible to a global audience.
8. **Analytics**: Implement usage analytics to track popular features and improve user experience.
9. **Mobile App**: Develop a standalone mobile application version of the generator.
10. **Browser Extension**: Create a browser extension for quick access to the generator from any webpage.

## Contributing

We welcome contributions to the TON Deeplink Generator! Please follow these steps to contribute:

1. Fork the repository
2. Create a new branch: `git checkout -b feature-branch-name`
3. Make your changes and commit them: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin feature-branch-name`
5. Submit a pull request

Please ensure your code adheres to the existing style and includes appropriate tests.

## Contact

For support or inquiries, please reach out via Telegram: [@arveer](https://t.me/arveer)

---

This project is open-source and not officially affiliated with the TON Foundation. Use at your own discretion and always verify generated deep links before use in production environments.

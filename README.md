# Divi WooPay Express Fix


 ## Overview
This repository offers a solution for a common issue encountered with WooCommerce's WooPay Express Checkout feature when used alongside Woo checkout modules in the Divi theme on WordPress. Specifically, it addresses the problem where multiple instances of the single-click payment express button element are incorrectly inserted at multiple locations on the checkout page. The WooPay Express script seems to be injecting them before every Woo checkout custom module.

The script provided in this repository ensures that only one functional express payment section, complete with an 'or' separator, is displayed at a user-specified location on the checkout page.


## How It Works

- **Hiding Redundant Buttons:** Initially, all instances of the WooPay Express buttons are hidden using CSS.
- **Waiting for Initialization:** The script waits for the first payment button to be initialized by WooPay's JavaScript.
- **Relocation and Display:** Once initialized, the script relocates this button and the 'or' separator to the location of a Divi code module placed by the user on the checkout page.

## Installation and Usage

1. **Insert Code in Divi Module:**

   - Edit your checkout page using Divi's page builder.
   - Add a new code module to the location where you want the WooPay Express button to appear.
   - Copy and paste the entire script (CSS and JavaScript) into this code module.

2. **Important Note:**

   - This fix should only be applied to the checkout page. It is not needed on product or cart pages, as WooPay Express functions correctly in those contexts.

3. **Customization (Optional):**
   - You may adjust the CSS and JavaScript as necessary to fit your specific theme or checkout page layout.

## Disclaimer
This script is provided as a quick fix for a specific issue encountered with WooCommerce's WooPay Express and Divi on WordPress. While it has been tested in certain scenarios, it is not guaranteed to work for every setup or configuration. The script may require customization to fit different themes or specific checkout page layouts.

We encourage users to test the script thoroughly in a development or staging environment before applying it to a live site. This is to ensure compatibility and to avoid any potential disruptions to your checkout process.

Please consider this solution as a temporary workaround rather than a permanent fix. We recommend keeping an eye out for updates from WooCommerce and Divi that may address this issue natively in the future.



## License

This project is distributed under the MIT License. See `LICENSE` for more information.

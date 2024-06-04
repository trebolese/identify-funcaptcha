# identify-funcaptcha
Usually funcaptcha require extra data called blob data, api domain and more. This tutorial will help you identify these.


## Understanding FunCaptcha
FunCaptcha is a security solution that uses a variety of advanced technologies to enhance security and user experience, including:

- **Behavioral Analysis**: This feature tracks user behavior during the challenge, such as mouse movements and click patterns, to differentiate between humans and bots.
- **Dynamic Challenges**: The challenges are constantly updated and differ each time, making it more difficult for bots to learn and solve them.
- **Adaptive Mechanisms**: The system adjusts the challenge's difficulty based on the user's risk profile and behavior, ensuring minimal disruption for legitimate users.
- **Device Fingerprinting**: It gathers and analyzes device and browser information to identify potential threats.
- **Machine Learning**: It uses machine learning models to analyze large amounts of data and improve the accuracy of distinguishing between human and automated traffic.

## Identifying FunCaptcha Usage with CapSolver Extension

In addition to finding the FunCaptcha Site Key, it may sometimes be necessary to determine if FunCaptcha is in use.

### Steps to Detect FunCaptcha Parameters:

1. **Installation**:
   * For Chrome users, install the [Captcha Solver Auto Solve](https://chrome.google.com/webstore/detail/captcha-solver-auto-bypas/pgojnojmmhpofjgdmaebadhbocahppod) extension.
   * For Firefox users, install the [Captcha Solver Auto Solve](https://addons.mozilla.org/en-US/firefox/addon/capsolver-captcha-solver/) extension.

2. **CapSolver Setup**:
   * Go to [CapSolver](https://www.capsolver.com/).
   * Press "F12" on your keyboard to open the developer tools.
   * Go to the **CapSolver Captcha Detector** tab.

3. **Detection**:
   * Keep the CapSolver panel open and visit the website where you want to trigger the CAPTCHA.
   * Trigger the captcha.
   * Note: **Do not close** the CapSolver panel before triggering the CAPTCHA.

### Identifying FunCaptcha Parameters:

The parameters for FunCaptcha that can be detected are:

* Website URL
* Site Key
* funcaptcha
* funcaptcha api js subdomain
* data blob

Once the CAPTCHA parameters are detected, CapSolver will provide a JSON detailing how to submit the captcha parameters to their service.

### Identifying FunCaptcha Usage:

1. **Open Developer Tools**:
   Press `F12` to open the developer tools or right-click on the webpage and select "Inspect".
 
2. **Open the CapSolver Panel**:
   Go to the Captcha Detector Panel.

3. **Trigger the FunCaptcha**:
   Perform the action that triggers the FunCaptcha on the webpage.

4. **Check the CapSolver Panel**:
   Look at the CapSolver Captcha Detector tab in the developer tools. If the `FunCaptcha` parameter is set to `true`, then FunCaptcha is being used on the site.

By following these steps, you can easily determine if FunCaptcha is being used on a website. Always use such tools responsibly and ethically, respecting the terms of service of the websites you interact with. For further assistance, you can contact CapSolver via email at [support@capsolver.com](mailto:support@capsolver.com).

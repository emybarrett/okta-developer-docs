---
title: Preview, test, and troubleshoot
---
The external service example is now ready with code to receive and respond to an Okta call. The Okta org is now set up to call the external service using a Registration Inline hook.

In your Okta org, you can preview the request and response JSON right from the Developer console. You can also test the code directly with self-registering users.

### Preview 

To preview the Registration Inline hook:

1. Navigate to Inline Hooks (Workflow > Inline Hooks) in your Developer console.
2. Click on the Registration Inline hook name (in this example, Guide Registration Hook Code).
3. Click the Preview tab.
4. Select a user from your org in the first block titled "Configure Inline Hook request".
5. From the "Preview example Inline Hook request" block, click "Generate Request".
    You should see the user's request information in JSON format that is sent to the external service.
6. From the "View service's response" block, click "View Response".
    You will see the response from your external service in JSON format, which either allows or denies the self-registration.

### Test

To run test your Registration Inline Hook, go to the Okta sign-in page for your Okta org, and attempt to self-register.

- If you use an allowable email domain, the user registration goes through.
- If you use an incorrect email domain, the user registration is denied; review the error message, which displays the error summary from the external service code and is passed back to Okta.

### Troubleshoot

Use Glitch's log feature to review and troublshoot your external service code:

1. In the Glitch project's left-hand folder navigation pane, click "Tools" at the bottom of the pane.
2. Click "Logs".

A log pane appears that displays all `console.log()` output. Some console output code is available in the sample code.

<NextSectionLink/>

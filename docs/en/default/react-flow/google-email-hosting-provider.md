---
type: page
title: Google email hosting provider
seoTitle: Google email hosting provider
seoDescription: What is SMPT mail hosting?
slug: google-email-hosting-provider
order: 29
status: published
---


# Google email hosting provider

## What is SMTP mail hosting?

With SMTP mail hosting, you can connect an external email hosting provider and use your personal, authorized business email as the sender in all "Send email" actions. Find more detailed information in [this article](https://help.devit.software/en/article/react-flow-connectors-8urln8/#1-color204a87react-flow-connectors).

## How to set up a Google provider?

1.  Open React Flow → open the **Connectors** section and click **SMTP connector**.

![Select SMTP connector](https://cdn.heymantle.com/docs/screenshots/2a9f7d8d-8d15-4722-b3e3-e52b84aee869/select-smtp_8j6dzb.png)

2.  (optional) Enter the name and description of the connector.
3.  In the Providers section, click **Choose provider** and select **Google**.
4.  Fill in the fields with the following information:

*   Host: [smtp.gmail.com](https://smtp.gmail.com)
*   Port: 587
*   Username: enter your email
*   Password: generate an app password in your Google account. See the detailed guide below.
*   Email: enter your email.
*   Security: TLS

![Enter connection details](https://cdn.heymantle.com/docs/screenshots/b6025855-1243-40b6-ac66-e88ade7e7881/google-email-hosting-provider_17dmhxc.png)

5.  Click **Test** in the upper-right corner.
6.  **Save** the connector.

## Generate app password

Note: Before generating an app password, make sure you have configured two-factor authentication.

1.  Log in to your Google account → click **Manage your Google account** in the upper-right corner.
2.  Open the **Security** section → click **2-Step Verification**.

![Click on 2-Step Verification](https://cdn.heymantle.com/docs/screenshots/2377b3af-4108-46c8-b8ae-3260ca57b955/google-security-verification_jmmftw.png)

3.  Enable 2-Step Verification and generate an app password by [following this link](https://myaccount.google.com/apppasswords?pli=1&rapt=AEjHL4Pax5NzPTUdQmzN71pedy0i7PcpciGX9TiGLf_jpD9vuXHYirSNoIuZ-2K3gEnTu9vLfQZsK2Q947c_ErnLOxPIlINzGc4fLp0ho3J_lTTyC__QMuk).
4.  Enter the app name in the field that appears → click **Generate**.

![](https://cdn.heymantle.com/docs/screenshots/8aa26238-595a-49ac-846e-b6e7c2ab4cb2/create-app-password_fp75w.png)

5.  Copy the generated password → return to React Flow and paste the app password into the **Password** field.

## Useful link

*   Learn more about all [Available React Flow connectors](/react-flow/react-flow-connectors).

## Suggested articles

*   [React Flow Connectors](https://help.devit.software/en/article/react-flow-connectors-8urln8/#1-color204a87react-flow-connectors)
*   [Components of the workflow](/react-flow/components-of-the-workflow)

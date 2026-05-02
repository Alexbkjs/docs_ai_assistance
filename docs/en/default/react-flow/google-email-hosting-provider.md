---
type: page
title: Google email hosting provider
seoTitle: Google email hosting provider
seoDescription: What is SMPT mail hosting?
slug: google-email-hosting-provider
order: 29
status: published
---

Articles on: [React Flow](/en/category/react-flow-2kjdy9/)

# Google email hosting provider

# Google email hosting provider

****In this article:****

*   [What is SMPT mail hosting?](#1-what-is-smpt-mail-hosting)
*   [How to set up a Google provider?](#1-how-to-set-up-a-google-provider)
*   [Generate app password](#1-generate-app-password)

# ✔️ What is SMTP mail hosting?

With SMTP mail hosting you can connect external email hosting provider and use your personal authorized business email as the sender in all "Send email" actions. Find more detailed information in [this article](https://help.devit.software/en/article/react-flow-connectors-8urln8/#1-color204a87react-flow-connectors)

# ✔️ How to set up a Google provider?

1.  Enter React Flow -> open the ****Connectors**** section and click on ****SMTP connector****.

![Select SMTP connector](https://cdn.heymantle.com/docs/screenshots/2a9f7d8d-8d15-4722-b3e3-e52b84aee869/select-smtp_8j6dzb.png)

2.  (optional) Enter the name and description of the connector.
3.  In the Providers section click on Choose provider and select ****Google****.
4.  Fill the appeared fields with the following info:

*   Host: [smtp.gmail.com](https://smtp.gmail.com)
*   Port: 587
*   Username: enter your email
*   Password: you need to generate app password in your Google account. Below you can find a detailed guide how to generate app password.
*   Email: enter your email.
*   Security: TLS

![Enter connection details](https://cdn.heymantle.com/docs/screenshots/b6025855-1243-40b6-ac66-e88ade7e7881/google-email-hosting-provider_17dmhxc.png)

5.  Click on ****Test**** in the upper-right corner.
6.  ****Save**** connector.

# ✔️ Generate app password

Note: Before you start generating an app password, make sure that you configured a two-factor authentication.

1.  To generate app password log in to your Google account -> click on ****Manage your Google account**** in the upper-right corner.
2.  Enter the ****Security**** section -> click on ****2-Step Verification****.

![Click on 2-Step Verification](https://cdn.heymantle.com/docs/screenshots/2377b3af-4108-46c8-b8ae-3260ca57b955/google-security-verification_jmmftw.png)

3.  Click Turn on 2-Step Verification and generate app password by [following this link](https://myaccount.google.com/apppasswords?pli=1&rapt=AEjHL4Pax5NzPTUdQmzN71pedy0i7PcpciGX9TiGLf_jpD9vuXHYirSNoIuZ-2K3gEnTu9vLfQZsK2Q947c_ErnLOxPIlINzGc4fLp0ho3J_lTTyC__QMuk).
4.  In the appeared field enter the name of the app -> click ****Generate****.

![](https://cdn.heymantle.com/docs/screenshots/8aa26238-595a-49ac-846e-b6e7c2ab4cb2/create-app-password_fp75w.png)

5.  Copy generated password -> get back to React Flow and paste app password to the ****Password**** field.

# ✔️ Useful link

*   Learn more about all [Available React Flow connectors](/react-flow-connectors).

## Suggested articles

*   [React Flow Connectors](https://help.devit.software/en/article/react-flow-connectors-8urln8/#1-color204a87react-flow-connectors)
*   [Components of the workflow](/components-of-the-workflow)

Updated on: 02/03/2026
---
title: "Secrets"
weight: 100
---

A secret [vRealize Automation](https://www.vmware.com/products/vrealize-automation.html) Cloud Assembly property is a reusable, encrypted value that [project](/Infrastructure/Administration/Projects/) users may add to their [cloud templates](/Design/Cloud_Templates/) designs.

Secure access keys and credentials are typical examples of secret properties. Once created and saved, a secret property value can never be unencrypted or read.

{{< img src="/Infrastructure/Administration/Secrets/secrets-view.png" alt="Secrets View " >}}

You can manage [vRealize Automation](https://www.vmware.com/products/vrealize-automation.html) Cloud Assembly's secret with project administrator role privileges.

1. Click New Secret.
2. Select the [project](/Infrastructure/Administration/Projects/).
3. Enter a unique property name for the secret, without spaces or special characters.
The name is the visible identifier for the secret.
4. Enter the secret value.
When typing, the value is obscured by default, which protects it if the screen is shared.

If needed, you can click the eye symbol to reveal and verify a value. After it is saved though, a secret value becomes encrypted in the database and can never be re-exposed.

Optionally, enter a longer description of the secret property.

5. Click Create.

{{< img src="/Infrastructure/Administration/Secrets/secrets-new.png" alt="Add new Secrets " >}}

[project](/Infrastructure/Administration/Projects/) users may add a secret property as a binding in [cloud templates](/Design/Cloud_Templates/)  code.

Note that starting to type the <strong><i>'${secret.</i></strong> characters reveals a selection list of secrets that have been created for the project.

{{< img src="/Infrastructure/Administration/Secrets/secrets-cloudtemplate.png" alt="Use Secrets in Cloud Templates " >}}

You can learn more in the following use case blogs:

[Cloud Assembly and ABX Secrets (and how to use them for installing vRealize SaltStack Minion Agents)](https://blogs.vmware.com/management/2021/02/cloud-assembly-and-abx-secrets.html)

[vRealize Automation Cloud Assembly’s new feature Secure Properties](https://blogs.vmware.com/management/2021/02/ca-secure-properties.html)


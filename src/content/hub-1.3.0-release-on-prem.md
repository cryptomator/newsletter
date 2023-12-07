## 🎉 Cryptomator Hub 1.3.0

As you may have noticed, Cryptomator Hub launched with version 1.0.0 more than a year ago. Since then, you have upgraded your instance up to 8 times to version 1.2.2 without required interaction on your part.

We have just released Cryptomator Hub 1.3.0 which introduces an `Account Key` for users. This update, while necessary and beneficial, will require active participation from users. That’s why we are reaching out to you today.

## ‼️ To prepare for the update
1. Read all sections of this email carefully
1. Ensure that the `Vault Recovery Keys` and `Vault Admin Passwords` are backed up
1. Inform your users about the upcoming update
1. Update Cryptomator (Desktop) to version 1.11.0 (recommended)
1. Update Cryptomator Hub (Server) to 1.3.0

## ℹ Preparation is Key
Before we apply the update to your Hub instance, ensure every vault admin secures a backup of their Vault Recovery Keys and Vault Admin Passwords. ⚠️ Doubling down on this step is critical; your backups are your safety net. Without them, our hands are tied.

## ⬆ Updating Cryptomator Hub (Server) to 1.3.0

If you're an administrator of a self-hosted Cryptomator Hub instance, follow these steps to update Cryptomator Hub:

1. [Back up the database](https://docs.cryptomator.org/en/latest/hub/setup/#backup). **:warning: The importance of a working backup cannot be overstated.**
2. Refresh your container image to the latest version: `ghcr.io/cryptomator/hub:1.3.0`
    - Skip this step if you're using the `stable` tag. We will update the `stable` tag to point to the new version in a couple of weeks.
3. Implement the changes within your container orchestrator. Monitor for healthy pod statuses before proceeding.

## ⬆ Updating Cryptomator (Desktop) to 1.11.0
Updating the Cryptomator desktop application is recommended for all users, but not technically required for now. Vaults can still be unlocked using an old version. This backward compatibility provides flexibility for a gradual rollout of the updated app. Nevertheless, making changes to access, incl. adding new members to a vault and adding new devices, requires Cryptomator 1.11.0 or higher.

## 🔑 Introducing Account Keys
With the updated app, users will encounter a two-step migration on their first unlock attempt:

1. Secure and store their new personal Account Key. ⚠️ It’s crucial for future logins from other devices.
1. Use the Account Key to link their Cryptomator device to their account.

This procedure is a one-time requirement for every user. It allows users to self-manage linked devices and vault owners to more easily manage access without having to frequently regrant permissions each time a user logs in from a new device.

## 👤 Claiming Vault Ownership and Granting Access
After updating to Hub 1.3.0, vault owners (formerly known as vault admins) are prompted to claim their vault again using the Vault Admin Password. Initially, only one user can claim ownership. Subsequently, this primary owner can grant ownership rights to others, thus eliminating the need to share and also have the Vault Admin Password.

Once vault members have navigated through the account migration, vault owners should refresh vault permissions. This action will securely distribute the necessary vault keys to the users.

Upon reclaim, the Vault Admin Password becomes obsolete. You may destroy any copies of it. Compromised Vault Admin Passwords don’t pose a threat to the security of the vault.

## 📚 Documentation

Please have a look into our documentation to see the [Account Key](https://docs.cryptomator.org/en/latest/hub/your-account/) in action, the new [Vault Management](https://docs.cryptomator.org/en/latest/hub/vault-management/) and the changes regarding [Vault Access](https://docs.cryptomator.org/en/latest/hub/access-vault/).

If you have any questions, please do not hesitate to contact us at hub@cryptomator.org

Happy crypting!
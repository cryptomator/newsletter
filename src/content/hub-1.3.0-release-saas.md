## 🎉 Cryptomator Hub 1.3.0

As you may have noticed, Cryptomator Hub launched with version 1.0.0 more than a year ago. Since then, we have upgraded your instance up to 8 times to version 1.2.2 without any downtime or required interaction on your part.

We have just released Cryptomator Hub 1.3.0 which introduces an `Account Key` for users. This update, while necessary and beneficial, will require active participation from users. That’s why we are reaching out to you today.

## ‼️ To prepare for the update
1. Read all sections of this email carefully
1. Choose a time slot for the update
1. Ensure that the `Vault Recovery Keys` and `Vault Admin Passwords` are backed up
1. Inform your users about the upcoming update
1. Update Cryptomator (Desktop) to version 1.11.0 (recommended)

## ℹ Preparation is Key
Before we apply the update to your Hub instance, ensure every vault admin secures a backup of their Vault Recovery Keys and Vault Admin Passwords. ⚠️ Doubling down on this step is critical; your backups are your safety net. Without them, our hands are tied.

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

## 📅 Schedule the Update
As mentioned at the beginning of this mail, we do not want to update your instance without any possible preparation on your part. We are offering the following timeframes for the update, and you can choose the one that suits you best:

1. 2023-01-17 09:00 UTC
1. 2023-01-17 21:00 UTC
1. 2023-01-19 09:00 UTC
1. 2023-01-19 21:00 UTC
1. 2023-01-24 09:00 UTC
1. 2023-01-24 21:00 UTC
1. 2023-01-26 09:00 UTC
1. 2023-01-26 21:00 UTC

Please reply to this mail by 2023-01-15 23:59 UTC with the time slot that works best for you.
Otherwise the update will be scheduled for the last time slot 2023-01-26 21:00 UTC.

## 📚 Documentation

Please have a look into our documentation to see the [Account Key](https://docs.cryptomator.org/en/latest/hub/your-account/) in action, the new [Vault Management](https://docs.cryptomator.org/en/latest/hub/vault-management/) and the changes regarding [Vault Access](https://docs.cryptomator.org/en/latest/hub/access-vault/).

If you have any questions, please do not hesitate to contact us at hub@cryptomator.org

Happy crypting!
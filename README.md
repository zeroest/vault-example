
# Vault

[[Refer] How to set up High Availability Vault with Consul backend?](https://www.opcito.com/blogs/how-to-set-up-high-availability-vault-with-consul-backend)

The above screenshot shows the first screen that appears after the initial deployment. Key Shares is basically the number of keys that you want and Threshold is the number of keys needed to be entered to unseal your vault. At least 5 Key Sharez and 2 Key Thresholds are recommended for good security. Also, make sure to download this content securely somewhere. It also provides the root authentication token.

Please securely distribute the keys below. When the Vault is re-sealed, restarted, or stopped, you must provide at least 3 of these keys to unseal it again. Vault does not store the master key. Without at least 3 keys, your Vault will remain permanently sealed.

Initial root token
- s.OwrY5VsuaM6BUwU7WXWPKOAH

Key
- a6jH/aWS5vgvPT/vRjxpLnn530YmVkQgVsCHqpURF++o
- 1sg0fIABeCHYEm3LcqkLqiv9PpNUS9KHCOJ6+cw5scAT
- 4mzl0bxRAAGneheToBTvAUM5HppeYFhok7VlHmvDUMJ6
- H+QqrM9gvsEhDHepI22JPk7ADFLjhkcDPwsSLfViwgTW
- dkd7JGkUT+lDiA/pJyBGCGTIIseU3vCmGfLgSCxCursM

---

Vault is sealed

Unseal Vault by entering portions of the unseal key. This can be done via multiple mechanisms on multiple computers. Once all portions are entered, the root key will be decrypted and Vault will unseal.

[[Doc] Seal/Unseal](https://www.vaultproject.io/docs/concepts/seal)
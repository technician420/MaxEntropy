# MaxEntropy
Cryptographic backups of the most important files on my computer.
Here is a tip, if I'm confident uploading my databases online (manual sync), then
I'm confident it will withhold brute force attacks by hackers. That probably means I use
strong passwords.

KFandPW_old.kdbx
AES-256
Argon2d
Rounds: 10
Memory: 1024 MiB
Parallelism: 8 threads

The database stores the keyfile required to mount 2025TS.kbdx. It also includes old passwords. (depreciated)

2025TS.kdbx
Twofish-256
Argon2d
Rounds: 2
Memory: 19 MiB
Parallelism: 1 thread

This is the bread and butter database used to store all my personal information, including my bank account.
KDF might be low, but consider this, without the keyfile, you are looking to brute force the whole keyspace.
In order to access the keyfile, you have to brute force KFandPW_old.kdbx.

VeracryptRescueEncrypted.7z
Type in the ZIP password to extract the bootloader rescue disk to get the cryptographic keys required to attack
my Windows system.

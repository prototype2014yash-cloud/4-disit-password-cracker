# 4-disit-password-cracker
secret_pin = "5486"  # Your own test PIN (4 digits)

attempts = 0

for i in range(10000):
    guess = str(i).zfill(4)  # Makes 0000, 0001, ..., 9999
    attempts += 1

    if guess == secret_pin:
        print("PIN found:", guess)
        print("Attempts:", attempts)
        break
